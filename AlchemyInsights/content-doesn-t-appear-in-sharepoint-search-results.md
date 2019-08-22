---
title: Konten tidak muncul dalam hasil pencarian SharePoint
ms.author: tlarsen
author: tklarsen
ms.date: 1/8/2019
ms.audience: ITPro
ms.topic: article
ROBOTS: NOINDEX, NOFOLLOW
localization_priority: Normal
ms.custom:
- "750"
- "5300017"
ms.assetid: 693db84f-2737-4c21-b027-4ab3d121b4a8
ms.openlocfilehash: ffb6bf349f9e8c2323186a8fc3183325d1d7e1bf
ms.sourcegitcommit: 1d98db8acb9959aba3b5e308a567ade6b62da56c
ms.translationtype: MT
ms.contentlocale: id-ID
ms.lasthandoff: 08/22/2019
ms.locfileid: "36517034"
---
# <a name="content-doesnt-appear-in-sharepoint-search-results"></a>Konten tidak muncul dalam hasil pencarian SharePoint

Ikuti langkah pemecahan masalah ketika konten yang diharapkan tidak muncul dalam hasil pencarian:
  
1. Memeriksa **situs** yang berisi konten diharapkan diatur untuk memungkinkan konten yang muncul dalam hasil pencarian. Ikuti langkah-langkah dalam [menunjukkan konten situs dalam hasil pencarian](https://docs.microsoft.com/sharepoint/make-site-content-searchable#show-content-on-a-site-in-search-results).

2. Periksa **Daftar** atau **Perpustakaan** yang berisi konten diharapkan diatur untuk memungkinkan konten yang muncul dalam hasil pencarian. Ikuti langkah-langkah di [Tampilkan isi dari daftar atau Perpustakaan dalam hasil pencarian](https://docs.microsoft.com/sharepoint/make-site-content-searchable#show-content-from-lists-or-libraries-in-search-results).

3. Memverifikasi bahwa halaman, dokumen, atau tata letak halaman kustom diterbitkan sebagai **versi Mayor.** Ikuti langkah 3 dalam [pencarian tidak kembali semua hasil dalam SharePoint Online](https://go.microsoft.com/fwlink/?linkid=874525).

4. Pastikan bahwa pengguna memiliki **izin** untuk melihat konten. Ikuti langkah-langkah dalam [pemahaman tingkat izin di SharePoint](https://docs.microsoft.com/sharepoint/understanding-permission-levels).
    
5. Jika skema Cari telah berubah dengan menambahkan properti dikelola baru, dengan mengedit properti yang dikelola atau dengan menghapus properti yang dikelola kemudian meminta merangkak dan mengindeks ulang akan diperlukan. **Kembali indeks** konten dengan mengikuti langkah-langkah di [secara manual meminta merangkak dan mengindeks ulang situs, Perpustakaan atau daftar](https://docs.microsoft.com/sharepoint/crawl-site-content). Ini mungkin memakan waktu cukup lama, tunggu selama 24 jam sebelum memeriksa hasil lagi.

Untuk selengkapnya, lihat [mengaktifkan konten di situs harus dicari](https://docs.microsoft.com/sharepoint/make-site-content-searchable). 
  
