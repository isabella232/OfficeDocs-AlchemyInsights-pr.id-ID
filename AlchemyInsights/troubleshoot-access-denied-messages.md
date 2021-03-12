---
title: Memecahkan masalah pesan Akses ditolak
ms.author: pebaum
author: pebaum
ms.date: 04/21/2020
ms.audience: ITPro
ms.topic: article
ms.service: o365-administration
ROBOTS: NOINDEX, NOFOLLOW
localization_priority: Normal
ms.assetid: d678b57a-53ad-4414-9423-d8726a0c532f
ms.openlocfilehash: 6c8ad84123fb58b73b9c378592ce970997893ea2
ms.sourcegitcommit: 0eb4f9bde53395b5fd4b5cd4ffc56ca96db91298
ms.translationtype: MT
ms.contentlocale: id-ID
ms.lasthandoff: 03/10/2021
ms.locfileid: "50704897"
---
# <a name="troubleshoot-access-denied-messages"></a><span data-ttu-id="bb1cf-102">Memecahkan masalah pesan Akses ditolak</span><span class="sxs-lookup"><span data-stu-id="bb1cf-102">Troubleshoot Access Denied messages</span></span>

<span data-ttu-id="bb1cf-103">Jika seseorang mendapat pesan "Akses ditolak" ke folder bersama di SharePoint, administrator kumpulan situs mungkin telah mengaktifkan "mode penguncian izin pengguna akses terbatas".</span><span class="sxs-lookup"><span data-stu-id="bb1cf-103">If someone got an "Access Denied" message to a shared folder in SharePoint, the site collection administrator might have enabled "Limited-access user permission lockdown mode."</span></span> <span data-ttu-id="bb1cf-104">Untuk menonaktifkannya:</span><span class="sxs-lookup"><span data-stu-id="bb1cf-104">To turn this off:</span></span> 
  
1. <span data-ttu-id="bb1cf-105">Telusuri ke situs, klik ikon pengaturan, lalu klik **pengaturan situs**.</span><span class="sxs-lookup"><span data-stu-id="bb1cf-105">Browse to the site, click the Settings icon, and then click **Site Settings**.</span></span>
    
2. <span data-ttu-id="bb1cf-106">Di bawah **administrasi kumpulan situs**, klik **fitur kumpulan situs**.</span><span class="sxs-lookup"><span data-stu-id="bb1cf-106">Under **Site Collection Administration**, click **Site collection features**.</span></span>
    
3. <span data-ttu-id="bb1cf-107">Di samping **mode penguncian izin pengguna dengan akses terbatas**, klik **Nonaktifkan**.</span><span class="sxs-lookup"><span data-stu-id="bb1cf-107">Next to **Limited-access user permission lockdown mode**, click **Deactivate**.</span></span>
    
<span data-ttu-id="bb1cf-108">Pesan Akses ditolak juga bisa terjadi untuk folder bersama jika situs adalah situs penerbitan.</span><span class="sxs-lookup"><span data-stu-id="bb1cf-108">An Access Denied message can also occur for shared folders if the site is a publishing site.</span></span> <span data-ttu-id="bb1cf-109">Untuk informasi, lihat [Akses ditolak ketika mengakses folder bersama](https://answers.microsoft.com/windows/forum/windows_7-files/access-denied-to-share-folder/79fae49d-cddf-4845-8ac8-c141884d85fb).</span><span class="sxs-lookup"><span data-stu-id="bb1cf-109">For info, see [Access Denied when accessing a shared folder](https://answers.microsoft.com/windows/forum/windows_7-files/access-denied-to-share-folder/79fae49d-cddf-4845-8ac8-c141884d85fb).</span></span>
  
<span data-ttu-id="bb1cf-110">Jika seseorang mendapat pesan "Akses ditolak" saat mencoba menampilkan permintaan akses, pengguna harus ditambahkan sebagai administrator kumpulan situs atau anggota grup pemilik untuk situs tersebut.</span><span class="sxs-lookup"><span data-stu-id="bb1cf-110">If a someone got an "Access Denied" message when trying to view access requests, the user needs to be added as either a site collection administrator or a member of the Owners group for the site.</span></span> <span data-ttu-id="bb1cf-111">Untuk informasi selengkapnya, lihat [Daftar akses ditolak untuk mengakses permintaan](https://go.microsoft.com/fwlink/?linkid=2004220).</span><span class="sxs-lookup"><span data-stu-id="bb1cf-111">For more info, see [Access Denied to Access Requests list](https://go.microsoft.com/fwlink/?linkid=2004220).</span></span>
  
<span data-ttu-id="bb1cf-112">Jika pengguna mendapat pesan "Akses ditolak" setelah dihapus dari direktori aktif di tempat lalu ditambahkan kembali, lihat [Akses ditolak saat akun pengguna disinkronkan ke Microsoft 365](https://go.microsoft.com/fwlink/?linkid=2004318).</span><span class="sxs-lookup"><span data-stu-id="bb1cf-112">If a user got an "Access Denied" message after they were removed from Active Directory on-premises and then added back, see [Access Denied when a user account is synced to Microsoft 365](https://go.microsoft.com/fwlink/?linkid=2004318).</span></span>
  

