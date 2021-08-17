---
title: Konten tidak muncul dalam hasil SharePoint pencarian
ms.author: tlarsen
author: tklarsen
ms.date: 04/21/2020
ms.audience: ITPro
ms.topic: article
ms.service: o365-administration
ROBOTS: NOINDEX, NOFOLLOW
localization_priority: Normal
ms.custom:
- "750"
- "5300017"
ms.assetid: 693db84f-2737-4c21-b027-4ab3d121b4a8
ms.openlocfilehash: ca03c31def64e43935d734a17735b10373e5ca85b5f4ea0f0e886b9ea39884cd
ms.sourcegitcommit: b5f7da89a650d2915dc652449623c78be6247175
ms.translationtype: MT
ms.contentlocale: id-ID
ms.lasthandoff: 08/05/2021
ms.locfileid: "54081613"
---
# <a name="content-doesnt-appear-in-sharepoint-search-results"></a>Konten tidak muncul dalam hasil SharePoint pencarian

Ikuti langkah pemecahan masalah ini jika konten yang diharapkan tidak muncul dalam hasil pencarian:
  
1. Periksa bahwa **situs yang** berisi konten yang diharapkan diatur untuk memungkinkan konten muncul dalam hasil pencarian. Ikuti langkah-langkah [dalam Memperlihatkan konten pada situs di hasil pencarian](https://docs.microsoft.com/sharepoint/make-site-content-searchable#show-content-on-a-site-in-search-results).

2. Periksa apakah daftar **atau** **pustaka yang** berisi konten yang diharapkan diatur untuk memungkinkan konten muncul dalam hasil pencarian. Ikuti langkah-langkah [dalam Memperlihatkan konten dari daftar atau pustaka dalam hasil pencarian](https://docs.microsoft.com/sharepoint/make-site-content-searchable#show-content-from-lists-or-libraries-in-search-results).

3. Verifikasi bahwa halaman, dokumen, atau tata letak halaman kustom diterbitkan sebagai **versi Utama.** Ikuti langkah 3 [dalam Pencarian tidak mengembalikan semua hasil dalam pencarian SharePoint Online.](https://go.microsoft.com/fwlink/?linkid=874525)

4. Verifikasi bahwa pengguna memiliki **izin** untuk menampilkan konten. Ikuti langkah-langkah [dalam Memahami tingkat izin di SharePoint](https://docs.microsoft.com/sharepoint/understanding-permission-levels).
    
5. If the search schema has been changed by adding a new managed property, by editing a managed property, or by removing a managed property then requesting a crawl and re-index will be required. **Re-index** the content by following the steps in [Manually request crawling and re-indexing of a site, a library or a list](https://docs.microsoft.com/sharepoint/crawl-site-content). Ini mungkin memakan waktu, tunggu 24 jam sebelum memeriksa kembali hasilnya.

Untuk informasi selengkapnya, [lihat Mengaktifkan konten di situs agar dapat dicari.](https://docs.microsoft.com/sharepoint/make-site-content-searchable) 
  
