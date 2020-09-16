---
title: Memperbaiki kesalahan 0x8004de40 di OneDrive
ms.author: pebaum
author: pebaum
ms.date: 04/21/2020
ms.audience: ITPro
ms.topic: article
ms.service: o365-administration
ROBOTS: NOINDEX, NOFOLLOW
localization_priority: Normal
ms.assetid: ''
ms.openlocfilehash: b9bd6dff48f78063e3d47f5fe2f834f59eb9868a
ms.sourcegitcommit: c6692ce0fa1358ec3529e59ca0ecdfdea4cdc759
ms.translationtype: MT
ms.contentlocale: id-ID
ms.lasthandoff: 09/14/2020
ms.locfileid: "47745133"
---
# <a name="fix-0x8004de40-error-in-onedrive"></a><span data-ttu-id="54d5b-102">Memperbaiki kesalahan 0x8004de40 di OneDrive</span><span class="sxs-lookup"><span data-stu-id="54d5b-102">Fix 0x8004de40 error in OneDrive</span></span>

<span data-ttu-id="54d5b-103">Jika Anda menerima kesalahan 0x8004de40 dengan OneDrive:</span><span class="sxs-lookup"><span data-stu-id="54d5b-103">If you receive an 0x8004de40 error with OneDrive:</span></span>

- <span data-ttu-id="54d5b-104">Reboot komputer yang terpengaruh saat tersambung ke domain direktori Acitve Anda.</span><span class="sxs-lookup"><span data-stu-id="54d5b-104">Reboot the affected computer while connected to your Acitve Directory domain.</span></span>
- <span data-ttu-id="54d5b-105">Jika reboot tidak memperbaiki masalah, berhenti bergabung dan bergabung kembali dengan perangkat Anda dari Azure AD.</span><span class="sxs-lookup"><span data-stu-id="54d5b-105">If a reboot doesn't fix the issue, unjoin and rejoin your device from Azure AD.</span></span> 

<span data-ttu-id="54d5b-106">**Catatan**: Anda harus berada di jaringan perusahaan Anda saat melakukan langkah-langkah ini.</span><span class="sxs-lookup"><span data-stu-id="54d5b-106">**Note**: You should be on your corporate network while performing these steps.</span></span> <span data-ttu-id="54d5b-107">Jangan melakukan langkah-langkah ini saat Anda tidak bisa menyambungkan ke infrastruktur perusahaan Anda (misalnya, saat bepergian).</span><span class="sxs-lookup"><span data-stu-id="54d5b-107">Don't perform these steps when you aren't able to connect to your corporate infrastructure (for example, while traveling).</span></span> 

- <span data-ttu-id="54d5b-108">Buka wantian perintah yang ditinggikan.</span><span class="sxs-lookup"><span data-stu-id="54d5b-108">Open an elevated command prompt.</span></span> 
- <span data-ttu-id="54d5b-109">Untuk membuka wantian perintah yang ditinggikan, klik- **mulai**, klik kanan **prompt perintah**, lalu klik **Jalankan sebagai administrator**.</span><span class="sxs-lookup"><span data-stu-id="54d5b-109">To open an elevated command prompt, click - **Start**, right-click **Command Prompt**, and then click **Run as administrator**.</span></span>
- <span data-ttu-id="54d5b-110">Ketik *dsregcmd/Leave* dan tekan **Enter**.</span><span class="sxs-lookup"><span data-stu-id="54d5b-110">Type *dsregcmd /leave* and press **Enter**.</span></span>
- <span data-ttu-id="54d5b-111">Bila sudah selesai, ketikkan *dsregcmd/Join* dan tekan **Enter**.</span><span class="sxs-lookup"><span data-stu-id="54d5b-111">When complete, type *dsregcmd /join* and press **Enter**.</span></span>
- <span data-ttu-id="54d5b-112">Setelah selesai, tutup wantian perintah.</span><span class="sxs-lookup"><span data-stu-id="54d5b-112">When complete, close the command prompt.</span></span>
- <span data-ttu-id="54d5b-113">Hidupkan ulang komputer, dan masuk ke OneDrive.</span><span class="sxs-lookup"><span data-stu-id="54d5b-113">Reboot the computer, and log into OneDrive.</span></span>