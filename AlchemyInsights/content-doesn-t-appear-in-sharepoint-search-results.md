---
title: Konten tidak muncul di hasil pencarian SharePoint
ms.author: tlarsen
author: tklarsen
ms.date: 04/21/2020
ms.audience: ITPro
ms.topic: article
ROBOTS: NOINDEX, NOFOLLOW
localization_priority: Normal
ms.custom:
- "750"
- "5300017"
ms.assetid: 693db84f-2737-4c21-b027-4ab3d121b4a8
ms.openlocfilehash: a21e0047b41390f740f9e13d31cba32b13990151
ms.sourcegitcommit: 55eff703a17e500681d8fa6a87eb067019ade3cc
ms.translationtype: MT
ms.contentlocale: id-ID
ms.lasthandoff: 04/22/2020
ms.locfileid: "43705664"
---
# <a name="content-doesnt-appear-in-sharepoint-search-results"></a>Konten tidak muncul di hasil pencarian SharePoint

Ikuti langkah pemecahan masalah ini saat konten yang diharapkan tidak muncul di hasil penelusuran:
  
1. Periksa apakah **situs** yang berisi konten yang diharapkan diatur untuk membolehkan konten ditampilkan di hasil pencarian. Ikuti langkah di [menampilkan konten di situs di hasil penelusuran](https://docs.microsoft.com/sharepoint/make-site-content-searchable#show-content-on-a-site-in-search-results).

2. Periksa apakah **Daftar** atau **Perpustakaan** yang berisi konten yang diharapkan diatur untuk mengizinkan konten ditampilkan di hasil pencarian. Ikuti langkah di [menampilkan konten dari daftar atau Perpustakaan di hasil penelusuran](https://docs.microsoft.com/sharepoint/make-site-content-searchable#show-content-from-lists-or-libraries-in-search-results).

3. Pastikan bahwa halaman, dokumen, atau tata letak halaman kustom diterbitkan sebagai **versi utama.** Ikuti langkah 3 di [pencarian tidak mengembalikan semua hasil di SharePoint online](https://go.microsoft.com/fwlink/?linkid=874525).

4. Verifikasi bahwa pengguna memiliki **izin** untuk melihat konten. Ikuti langkah dalam [memahami tingkat izin di SharePoint](https://docs.microsoft.com/sharepoint/understanding-permission-levels).
    
5. Jika skema pencarian telah diubah dengan menambahkan properti terkelola baru, dengan mengedit properti terkelola, atau dengan menghapus properti terkelola, maka permintaan perayapan dan indeks ulang akan diperlukan. **Mengindeks ulang** konten dengan mengikuti langkah [secara manual meminta perayapan dan mengindeks ulang situs, Perpustakaan, atau daftar](https://docs.microsoft.com/sharepoint/crawl-site-content). Ini mungkin memakan waktu beberapa saat, tunggu 24 jam sebelum memeriksa hasilnya lagi.

Untuk informasi lebih lanjut, lihat [mengaktifkan konten di situs untuk dapat ditelusuri](https://docs.microsoft.com/sharepoint/make-site-content-searchable). 
  
