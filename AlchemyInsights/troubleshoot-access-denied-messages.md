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
ms.openlocfilehash: 3550081a12379f73725253214a2c2d44974ab740
ms.sourcegitcommit: c6692ce0fa1358ec3529e59ca0ecdfdea4cdc759
ms.translationtype: MT
ms.contentlocale: id-ID
ms.lasthandoff: 09/14/2020
ms.locfileid: "47690786"
---
# <a name="troubleshoot-access-denied-messages"></a><span data-ttu-id="f089a-102">Memecahkan masalah pesan Akses ditolak</span><span class="sxs-lookup"><span data-stu-id="f089a-102">Troubleshoot Access Denied messages</span></span>

<span data-ttu-id="f089a-103">Jika seseorang mendapat pesan "Akses ditolak" ke folder bersama di SharePoint, administrator kumpulan situs mungkin telah mengaktifkan "mode penguncian izin pengguna akses terbatas".</span><span class="sxs-lookup"><span data-stu-id="f089a-103">If someone got an "Access Denied" message to a shared folder in SharePoint, the site collection administrator might have enabled "Limited-access user permission lockdown mode."</span></span> <span data-ttu-id="f089a-104">Untuk menonaktifkannya:</span><span class="sxs-lookup"><span data-stu-id="f089a-104">To turn this off:</span></span> 
  
1. <span data-ttu-id="f089a-105">Telusuri ke situs, klik ikon pengaturan, lalu klik **pengaturan situs**.</span><span class="sxs-lookup"><span data-stu-id="f089a-105">Browse to the site, click the Settings icon, and then click **Site Settings**.</span></span>
    
2. <span data-ttu-id="f089a-106">Di bawah **administrasi kumpulan situs**, klik **fitur kumpulan situs**.</span><span class="sxs-lookup"><span data-stu-id="f089a-106">Under **Site Collection Administration**, click **Site collection features**.</span></span>
    
3. <span data-ttu-id="f089a-107">Di samping **mode penguncian izin pengguna dengan akses terbatas**, klik **Nonaktifkan**.</span><span class="sxs-lookup"><span data-stu-id="f089a-107">Next to **Limited-access user permission lockdown mode**, click **Deactivate**.</span></span>
    
<span data-ttu-id="f089a-108">Pesan Akses ditolak juga bisa terjadi untuk folder bersama jika situs adalah situs penerbitan.</span><span class="sxs-lookup"><span data-stu-id="f089a-108">An Access Denied message can also occur for shared folders if the site is a publishing site.</span></span> <span data-ttu-id="f089a-109">Untuk informasi, lihat [Akses ditolak ketika mengakses folder bersama](https://go.microsoft.com/fwlink/?linkid=2004317).</span><span class="sxs-lookup"><span data-stu-id="f089a-109">For info, see [Access Denied when accessing a shared folder](https://go.microsoft.com/fwlink/?linkid=2004317).</span></span>
  
<span data-ttu-id="f089a-110">Jika seseorang mendapat pesan "Akses ditolak" saat mencoba menampilkan permintaan akses, pengguna harus ditambahkan sebagai administrator kumpulan situs atau anggota grup pemilik untuk situs tersebut.</span><span class="sxs-lookup"><span data-stu-id="f089a-110">If a someone got an "Access Denied" message when trying to view access requests, the user needs to be added as either a site collection administrator or a member of the Owners group for the site.</span></span> <span data-ttu-id="f089a-111">Untuk informasi selengkapnya, lihat [Daftar akses ditolak untuk mengakses permintaan](https://go.microsoft.com/fwlink/?linkid=2004220).</span><span class="sxs-lookup"><span data-stu-id="f089a-111">For more info, see [Access Denied to Access Requests list](https://go.microsoft.com/fwlink/?linkid=2004220).</span></span>
  
<span data-ttu-id="f089a-112">Jika pengguna mendapat pesan "Akses ditolak" setelah dihapus dari direktori aktif di tempat lalu ditambahkan kembali, lihat [Akses ditolak saat akun pengguna disinkronkan ke Microsoft 365](https://go.microsoft.com/fwlink/?linkid=2004318).</span><span class="sxs-lookup"><span data-stu-id="f089a-112">If a user got an "Access Denied" message after they were removed from Active Directory on-premises and then added back, see [Access Denied when a user account is synced to Microsoft 365](https://go.microsoft.com/fwlink/?linkid=2004318).</span></span>
  

