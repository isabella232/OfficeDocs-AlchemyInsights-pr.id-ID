---
title: Perbaiki kesalahan 0x8004de40 di OneDrive
ms.author: pebaum
author: Techwriter40
ms.date: 6/20/2019
ms.audience: ITPro
ms.topic: article
ROBOTS: NOINDEX, NOFOLLOW
localization_priority: Normal
ms.assetid: ''
ms.openlocfilehash: aa0e0a63ac1e365a7cdce018626740446040a664
ms.sourcegitcommit: a65d196d00adb70045af5caca9828fe44b951f61
ms.translationtype: MT
ms.contentlocale: id-ID
ms.lasthandoff: 09/04/2019
ms.locfileid: "36755851"
---
# <a name="fix-0x8004de40-error-in-onedrive"></a><span data-ttu-id="cbcbe-102">Perbaiki kesalahan 0x8004de40 di OneDrive</span><span class="sxs-lookup"><span data-stu-id="cbcbe-102">Fix 0x8004de40 error in OneDrive</span></span>

<span data-ttu-id="cbcbe-103">Jika Anda menerima galat 0x8004de40 dengan OneDrive:</span><span class="sxs-lookup"><span data-stu-id="cbcbe-103">If you receive an 0x8004de40 error with OneDrive:</span></span>

- <span data-ttu-id="cbcbe-104">Reboot komputer yang terpengaruh saat tersambung ke domain direktori Acitve Anda.</span><span class="sxs-lookup"><span data-stu-id="cbcbe-104">Reboot the affected computer while connected to your Acitve Directory domain.</span></span>
- <span data-ttu-id="cbcbe-105">Jika reboot tidak memperbaiki masalah, keluar dan bergabung kembali perangkat Anda dari Azure AD.</span><span class="sxs-lookup"><span data-stu-id="cbcbe-105">If a reboot doesn't fix the issue, unjoin and rejoin your device from Azure AD.</span></span> 

<span data-ttu-id="cbcbe-106">**Catatan**: Anda harus berada di jaringan korporat Anda saat melakukan langkah ini.</span><span class="sxs-lookup"><span data-stu-id="cbcbe-106">**Note**: You should be on your corporate network while performing these steps.</span></span> <span data-ttu-id="cbcbe-107">Jangan lakukan langkah ini ketika Anda tidak dapat terhubung ke infrastruktur perusahaan Anda (misalnya, saat bepergian).</span><span class="sxs-lookup"><span data-stu-id="cbcbe-107">Don't perform these steps when you aren't able to connect to your corporate infrastructure (for example, while traveling).</span></span> 

- <span data-ttu-id="cbcbe-108">Buka wantian perintah yang ditinggikan.</span><span class="sxs-lookup"><span data-stu-id="cbcbe-108">Open an elevated command prompt.</span></span> 
- <span data-ttu-id="cbcbe-109">Untuk membuka wantian perintah yang ditinggikan, klik- **mulai**, klik kanan **wantian perintah**, dan kemudian klik **Jalankan sebagai administrator**.</span><span class="sxs-lookup"><span data-stu-id="cbcbe-109">To open an elevated command prompt, click - **Start**, right-click **Command Prompt**, and then click **Run as administrator**.</span></span>
- <span data-ttu-id="cbcbe-110">Ketik *dsregcmd/Leave* dan tekan **Enter**.</span><span class="sxs-lookup"><span data-stu-id="cbcbe-110">Type *dsregcmd /leave* and press **Enter**.</span></span>
- <span data-ttu-id="cbcbe-111">Setelah selesai, ketik *dsregcmd/Join* dan tekan **Enter**.</span><span class="sxs-lookup"><span data-stu-id="cbcbe-111">When complete, type *dsregcmd /join* and press **Enter**.</span></span>
- <span data-ttu-id="cbcbe-112">Setelah selesai, tutup wantian perintah.</span><span class="sxs-lookup"><span data-stu-id="cbcbe-112">When complete, close the command prompt.</span></span>
- <span data-ttu-id="cbcbe-113">Reboot komputer, dan masuk ke OneDrive.</span><span class="sxs-lookup"><span data-stu-id="cbcbe-113">Reboot the computer, and log into OneDrive.</span></span>