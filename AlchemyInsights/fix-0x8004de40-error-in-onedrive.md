---
title: Memperbaiki kesalahan 0x8004de40 di OneDrive
ms.author: kirks
author: Techwriter40
ms.date: 6/20/2019
ms.audience: ITPro
ms.topic: article
ROBOTS: NOINDEX, NOFOLLOW
localization_priority: Normal
ms.assetid: ''
ms.openlocfilehash: 2256fb66cb7a4e2adcff9fda16a80c87e2997f0c
ms.sourcegitcommit: 8f6a1be929b275faa295ba8aeeae17898a47c3b0
ms.translationtype: MT
ms.contentlocale: id-ID
ms.lasthandoff: 06/21/2019
ms.locfileid: "35133980"
---
# <a name="fix-0x8004de40-error-in-onedrive"></a><span data-ttu-id="2f03e-102">Memperbaiki kesalahan 0x8004de40 di OneDrive</span><span class="sxs-lookup"><span data-stu-id="2f03e-102">Fix 0x8004de40 error in OneDrive</span></span>

<span data-ttu-id="2f03e-103">Jika Anda menerima kesalahan 0x8004de40 dengan OneDrive:</span><span class="sxs-lookup"><span data-stu-id="2f03e-103">If you receive an 0x8004de40 error with OneDrive:</span></span>

- <span data-ttu-id="2f03e-104">Reboot komputer terkena saat terhubung ke domain Acitve direktori.</span><span class="sxs-lookup"><span data-stu-id="2f03e-104">Reboot the affected computer while connected to your Acitve Directory domain.</span></span>
- <span data-ttu-id="2f03e-105">Jika reboot tidak mengatasi masalah tersebut, keluar dan bergabung kembali perangkat Anda dari iklan Azure.</span><span class="sxs-lookup"><span data-stu-id="2f03e-105">If a reboot doesn't fix the issue, unjoin and rejoin your device from Azure AD.</span></span> 

<span data-ttu-id="2f03e-106">**Catatan**: Anda harus berada di jaringan perusahaan Anda sambil melakukan langkah-langkah berikut.</span><span class="sxs-lookup"><span data-stu-id="2f03e-106">**Note**: You should be on your corporate network while performing these steps.</span></span> <span data-ttu-id="2f03e-107">Tidak melakukan langkah-langkah berikut ketika Anda tidak dapat terhubung ke infrastruktur perusahaan Anda (misalnya, saat bepergian).</span><span class="sxs-lookup"><span data-stu-id="2f03e-107">Don't perform these steps when you aren't able to connect to your corporate infrastructure (for example, while traveling).</span></span> 

- <span data-ttu-id="2f03e-108">Buka ditinggikan command prompt.</span><span class="sxs-lookup"><span data-stu-id="2f03e-108">Open an elevated command prompt.</span></span> 
- <span data-ttu-id="2f03e-109">Untuk membuka ditinggikan command prompt, klik - **Start**, klik kanan **Prompt Perintah**, dan kemudian klik **Jalankan sebagai administrator**.</span><span class="sxs-lookup"><span data-stu-id="2f03e-109">To open an elevated command prompt, click - **Start**, right-click **Command Prompt**, and then click **Run as administrator**.</span></span>
- <span data-ttu-id="2f03e-110">Ketik *dsregcmd /leave* dan tekan **Enter**.</span><span class="sxs-lookup"><span data-stu-id="2f03e-110">Type *dsregcmd /leave* and press **Enter**.</span></span>
- <span data-ttu-id="2f03e-111">Ketika selesai, *ketik/Join dsregcmd* dan tekan **Enter**.</span><span class="sxs-lookup"><span data-stu-id="2f03e-111">When complete, type *dsregcmd /join* and press **Enter**.</span></span>
- <span data-ttu-id="2f03e-112">Setelah selesai, tutup command prompt.</span><span class="sxs-lookup"><span data-stu-id="2f03e-112">When complete, close the command prompt.</span></span>
- <span data-ttu-id="2f03e-113">Reboot komputer, dan login ke OneDrive.</span><span class="sxs-lookup"><span data-stu-id="2f03e-113">Reboot the computer, and log into OneDrive.</span></span>