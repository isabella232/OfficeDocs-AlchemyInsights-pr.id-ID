---
title: Perbaiki kesalahan 0x8004de40 di OneDrive
ms.author: pebaum
author: pebaum
ms.date: 6/20/2019
ms.audience: ITPro
ms.topic: article
ROBOTS: NOINDEX, NOFOLLOW
localization_priority: Normal
ms.assetid: ''
ms.openlocfilehash: 48b29f57763ca22a71a23b2afddcac0e8e8a95db
ms.sourcegitcommit: 0f0186044a3597e42ad14c32ca58e7224344dcfa
ms.translationtype: MT
ms.contentlocale: id-ID
ms.lasthandoff: 12/15/2019
ms.locfileid: "40052040"
---
# <a name="fix-0x8004de40-error-in-onedrive"></a><span data-ttu-id="a7b58-102">Perbaiki kesalahan 0x8004de40 di OneDrive</span><span class="sxs-lookup"><span data-stu-id="a7b58-102">Fix 0x8004de40 error in OneDrive</span></span>

<span data-ttu-id="a7b58-103">Jika Anda menerima galat 0x8004de40 dengan OneDrive:</span><span class="sxs-lookup"><span data-stu-id="a7b58-103">If you receive an 0x8004de40 error with OneDrive:</span></span>

- <span data-ttu-id="a7b58-104">Reboot komputer yang terpengaruh saat tersambung ke domain direktori Acitve Anda.</span><span class="sxs-lookup"><span data-stu-id="a7b58-104">Reboot the affected computer while connected to your Acitve Directory domain.</span></span>
- <span data-ttu-id="a7b58-105">Jika reboot tidak memperbaiki masalah, keluar dan bergabung kembali perangkat Anda dari Azure AD.</span><span class="sxs-lookup"><span data-stu-id="a7b58-105">If a reboot doesn't fix the issue, unjoin and rejoin your device from Azure AD.</span></span> 

<span data-ttu-id="a7b58-106">**Catatan**: Anda harus berada di jaringan korporat Anda saat melakukan langkah ini.</span><span class="sxs-lookup"><span data-stu-id="a7b58-106">**Note**: You should be on your corporate network while performing these steps.</span></span> <span data-ttu-id="a7b58-107">Jangan lakukan langkah ini ketika Anda tidak dapat terhubung ke infrastruktur perusahaan Anda (misalnya, saat bepergian).</span><span class="sxs-lookup"><span data-stu-id="a7b58-107">Don't perform these steps when you aren't able to connect to your corporate infrastructure (for example, while traveling).</span></span> 

- <span data-ttu-id="a7b58-108">Buka wantian perintah yang ditinggikan.</span><span class="sxs-lookup"><span data-stu-id="a7b58-108">Open an elevated command prompt.</span></span> 
- <span data-ttu-id="a7b58-109">Untuk membuka wantian perintah yang ditinggikan, klik- **mulai**, klik kanan **wantian perintah**, dan kemudian klik **Jalankan sebagai administrator**.</span><span class="sxs-lookup"><span data-stu-id="a7b58-109">To open an elevated command prompt, click - **Start**, right-click **Command Prompt**, and then click **Run as administrator**.</span></span>
- <span data-ttu-id="a7b58-110">Ketik *dsregcmd/Leave* dan tekan **Enter**.</span><span class="sxs-lookup"><span data-stu-id="a7b58-110">Type *dsregcmd /leave* and press **Enter**.</span></span>
- <span data-ttu-id="a7b58-111">Setelah selesai, ketik *dsregcmd/Join* dan tekan **Enter**.</span><span class="sxs-lookup"><span data-stu-id="a7b58-111">When complete, type *dsregcmd /join* and press **Enter**.</span></span>
- <span data-ttu-id="a7b58-112">Setelah selesai, tutup wantian perintah.</span><span class="sxs-lookup"><span data-stu-id="a7b58-112">When complete, close the command prompt.</span></span>
- <span data-ttu-id="a7b58-113">Reboot komputer, dan masuk ke OneDrive.</span><span class="sxs-lookup"><span data-stu-id="a7b58-113">Reboot the computer, and log into OneDrive.</span></span>