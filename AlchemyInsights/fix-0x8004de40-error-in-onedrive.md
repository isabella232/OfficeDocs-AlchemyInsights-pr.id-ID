---
title: Memperbaiki 0x8004de40 di OneDrive
ms.author: pebaum
author: pebaum
ms.date: 04/21/2020
ms.audience: ITPro
ms.topic: article
ms.service: o365-administration
ROBOTS: NOINDEX, NOFOLLOW
localization_priority: Normal
ms.assetid: ''
ms.openlocfilehash: 0edb3e19b5dea240c9f2846dc503e65d92113cb7
ms.sourcegitcommit: 477cce131dc4a3c212ab18a8763a50b2f3bb20b1
ms.translationtype: MT
ms.contentlocale: id-ID
ms.lasthandoff: 04/09/2021
ms.locfileid: "51649751"
---
# <a name="fix-0x8004de40-error-in-onedrive"></a><span data-ttu-id="4a320-102">Memperbaiki 0x8004de40 di OneDrive</span><span class="sxs-lookup"><span data-stu-id="4a320-102">Fix 0x8004de40 error in OneDrive</span></span>

<span data-ttu-id="4a320-103">Jika Anda menjalankan Windows 7 dan menerima kesalahan ini, Perbarui untuk mengaktifkan [TLS 1.1 dan TLS 1.2](https://support.microsoft.com/topic/update-to-enable-tls-1-1-and-tls-1-2-as-default-secure-protocols-in-winhttp-in-windows-c4bd73d2-31d7-761e-0178-11268bb10392)sebagai protokol aman default di WinHTTP di Windows .</span><span class="sxs-lookup"><span data-stu-id="4a320-103">If you're running Windows 7 and receive this error, [Update to enable TLS 1.1 and TLS 1.2 as default secure protocols in WinHTTP in Windows](https://support.microsoft.com/topic/update-to-enable-tls-1-1-and-tls-1-2-as-default-secure-protocols-in-winhttp-in-windows-c4bd73d2-31d7-761e-0178-11268bb10392).</span></span>

<span data-ttu-id="4a320-104">Jika menjalankan Windows 10, dan Anda menerima pesan kesalahan 0x8004de40 OneDrive:</span><span class="sxs-lookup"><span data-stu-id="4a320-104">If you're running Windows 10, and you receive an 0x8004de40 error with OneDrive:</span></span>

- <span data-ttu-id="4a320-105">Me-reboot komputer yang terpengaruh saat tersambung ke domain Direktori Acitve Anda.</span><span class="sxs-lookup"><span data-stu-id="4a320-105">Reboot the affected computer while connected to your Acitve Directory domain.</span></span>
- <span data-ttu-id="4a320-106">Jika mulai ulang tidak memperbaiki masalah, sambungkan kembali dan bergabung kembali ke perangkat Anda dari Azure AD.</span><span class="sxs-lookup"><span data-stu-id="4a320-106">If a reboot doesn't fix the issue, unjoin and rejoin your device from Azure AD.</span></span> 

<span data-ttu-id="4a320-107">**Catatan:** Anda harus berada di jaringan perusahaan Anda sambil melakukan langkah-langkah ini.</span><span class="sxs-lookup"><span data-stu-id="4a320-107">**Note**: You should be on your corporate network while performing these steps.</span></span> <span data-ttu-id="4a320-108">Jangan lakukan langkah-langkah ini saat Anda tidak tersambung ke infrastruktur perusahaan (misalnya, saat berpergian).</span><span class="sxs-lookup"><span data-stu-id="4a320-108">Don't perform these steps when you aren't connected to your corporate infrastructure (for example, while traveling).</span></span> 

1. <span data-ttu-id="4a320-109">Buka prompt perintah yang ditinggikan dengan **memilih Mulai**, klik kanan **Prompt Perintah**, lalu pilih Jalankan **sebagai administrator**.</span><span class="sxs-lookup"><span data-stu-id="4a320-109">Open an elevated command prompt by selecting **Start**, right-click **Command Prompt**, and then select **Run as administrator**.</span></span>

1. <span data-ttu-id="4a320-110">Ketik *dsregcmd /leave* dan tekan **Enter**.</span><span class="sxs-lookup"><span data-stu-id="4a320-110">Type *dsregcmd /leave* and press **Enter**.</span></span>

1. <span data-ttu-id="4a320-111">Bila sudah selesai, *ketik dsregcmd /join* lalu tekan **Enter**.</span><span class="sxs-lookup"><span data-stu-id="4a320-111">When complete, type *dsregcmd /join* and press **Enter**.</span></span>

1. <span data-ttu-id="4a320-112">Setelah selesai, tutup prompt perintah.</span><span class="sxs-lookup"><span data-stu-id="4a320-112">When complete, close the command prompt.</span></span>

1. <span data-ttu-id="4a320-113">Me-reboot komputer, dan masuk ke OneDrive.</span><span class="sxs-lookup"><span data-stu-id="4a320-113">Reboot the computer, and log into OneDrive.</span></span>