---
title: Memecahkan masalah sinkronisasi sandi
ms.author: pebaum
author: pebaum
manager: mnirkhe
ms.date: 3/20/2018
ms.audience: Admin
ms.topic: article
ROBOTS: NOINDEX, NOFOLLOW
localization_priority: Priority
ms.collection: Adm_O365
ms.custom: Adm_O365
ms.assetid: 1cba32c4-37ce-4ec1-9e58-8d3440b53d57
ms.openlocfilehash: c71fce8621057093d23891c26f7b0285fdc8b9ed
ms.sourcegitcommit: d6ea5e9458a2b8ceaab3ac4bd483e1130b9a398a
ms.translationtype: MT
ms.contentlocale: id-ID
ms.lasthandoff: 01/15/2019
ms.locfileid: "28295235"
---
# <a name="troubleshoot-password-synchronization"></a><span data-ttu-id="5c701-102">Memecahkan masalah sinkronisasi sandi</span><span class="sxs-lookup"><span data-stu-id="5c701-102">Troubleshoot password synchronization</span></span>

<span data-ttu-id="5c701-103">Untuk mengatasi masalah yang mana tidak ada password disinkronisasi dengan Azure iklan menghubungkan versi 1.1.614.0 atau yang lebih baru:</span><span class="sxs-lookup"><span data-stu-id="5c701-103">To troubleshoot issues where no passwords are synchronized with Azure AD Connect version 1.1.614.0 or later:</span></span>
  
1. <span data-ttu-id="5c701-104">Buka sesi Windows PowerShell yang baru pada server Azure iklan menghubungkan Anda dengan pilihan **Jalankan sebagai Administrator** .</span><span class="sxs-lookup"><span data-stu-id="5c701-104">Open a new Windows PowerShell session on your Azure AD Connect server with the **Run as Administrator** option.</span></span> 
    
2. <span data-ttu-id="5c701-105">Menjalankan **Set-executionpolicy tidak RemoteSigned** atau **tak Set-executionpolicy tidak dibatasi**.</span><span class="sxs-lookup"><span data-stu-id="5c701-105">Run **Set-ExecutionPolicy RemoteSigned** or **Set-ExecutionPolicy Unrestricted**.</span></span> 
    
3. <span data-ttu-id="5c701-106">Mulai wizard Azure iklan terhubung.</span><span class="sxs-lookup"><span data-stu-id="5c701-106">Start the Azure AD Connect wizard.</span></span>
    
4. <span data-ttu-id="5c701-107">Menavigasi ke \*\* tambahan tugas \*\* halaman, pilih \*\* mengatasi masalah \*\*, lalu klik **berikutnya**.</span><span class="sxs-lookup"><span data-stu-id="5c701-107">Navigate to the \*\* Additional Tasks \*\* page, select \*\* Troubleshoot \*\*, and click **Next**.</span></span> 
    
5. <span data-ttu-id="5c701-108">Pada halaman Troubleshooting, klik menu **peluncuran untuk mulai mengatasi masalah** di PowerShell.</span><span class="sxs-lookup"><span data-stu-id="5c701-108">On the Troubleshooting page, click **Launch to start the troubleshooting** menu in PowerShell.</span></span> 
    
6. <span data-ttu-id="5c701-109">Di menu utama, pilih **Memecahkan sandi sinkronisasi**.</span><span class="sxs-lookup"><span data-stu-id="5c701-109">In the main menu, select **Troubleshoot Password Synchronization**.</span></span> 
    
7. <span data-ttu-id="5c701-110">Dalam sub menu, pilih **sinkronisasi Password tidak bekerja sama sekali**.</span><span class="sxs-lookup"><span data-stu-id="5c701-110">In the sub menu, select **Password Synchronization does not work at all**.</span></span> 
    
 <span data-ttu-id="5c701-111">**Memahami hasil tugas pemecahan masalah**</span><span class="sxs-lookup"><span data-stu-id="5c701-111">**Understand the results of the troubleshooting task**</span></span>
  
<span data-ttu-id="5c701-112">Pemecahan masalah tugas melakukan pemeriksaan yang berikut:</span><span class="sxs-lookup"><span data-stu-id="5c701-112">The troubleshooting task performs the following checks:</span></span>
  
- <span data-ttu-id="5c701-113">Memvalidasi bahwa fitur sinkronisasi password diaktifkan untuk penyewa Azure iklan Anda.</span><span class="sxs-lookup"><span data-stu-id="5c701-113">Validates that the password synchronization feature is enabled for your Azure AD tenant.</span></span>
    
- <span data-ttu-id="5c701-114">Memvalidasi bahwa server Azure iklan terhubung tidak berada di pementasan mode.</span><span class="sxs-lookup"><span data-stu-id="5c701-114">Validates that the Azure AD Connect server is not in staging mode.</span></span>
    
- <span data-ttu-id="5c701-115">Untuk setiap ada lokal Active Directory connector (yang berhubungan dengan forest Active Directory yang ada):</span><span class="sxs-lookup"><span data-stu-id="5c701-115">For each existing on-premises Active Directory connector (which corresponds to an existing Active Directory forest):</span></span>
    
- 
  - <span data-ttu-id="5c701-116">Memvalidasi bahwa fitur sinkronisasi password diaktifkan.</span><span class="sxs-lookup"><span data-stu-id="5c701-116">Validates that the password synchronization feature is enabled.</span></span>
    
  - <span data-ttu-id="5c701-117">Pencarian untuk sandi sinkronisasi detak jantung peristiwa di log peristiwa Windows aplikasi.</span><span class="sxs-lookup"><span data-stu-id="5c701-117">Searches for password synchronization heartbeat events in the Windows Application Event logs.</span></span>
    
  - <span data-ttu-id="5c701-118">Untuk setiap domain Active Directory di bawah konektor Active Directory lokal:</span><span class="sxs-lookup"><span data-stu-id="5c701-118">For each Active Directory domain under the on-premises Active Directory connector:</span></span>
    
  - <span data-ttu-id="5c701-119">Memvalidasi bahwa domain dapat dicapai dari server Azure iklan terhubung.</span><span class="sxs-lookup"><span data-stu-id="5c701-119">Validates that the domain is reachable from the Azure AD Connect server.</span></span>
    
  - <span data-ttu-id="5c701-120">Memvalidasi bahwa account Active Directory Domain Services (AD DS) yang digunakan oleh konektor Active Directory lokal memiliki benar username, password, dan izin yang diperlukan untuk sinkronisasi password.</span><span class="sxs-lookup"><span data-stu-id="5c701-120">Validates that the Active Directory Domain Services (AD DS) accounts used by the on-premises Active Directory connector has the correct username, password, and permissions required for password synchronization.</span></span>
    
<span data-ttu-id="5c701-121">Untuk bantuan lebih lanjut pemecahan masalah sinkronisasi sandi, lihat [mengatasi masalah sinkronisasi password dengan Azure iklan menyambung sinkronisasi](https://docs.microsoft.com/en-us/azure/active-directory/connect/active-directory-aadconnectsync-troubleshoot-password-synchronization).</span><span class="sxs-lookup"><span data-stu-id="5c701-121">For more help troubleshooting password sync, see [Troubleshoot password synchronization with Azure AD Connect sync](https://docs.microsoft.com/en-us/azure/active-directory/connect/active-directory-aadconnectsync-troubleshoot-password-synchronization).</span></span>
  
