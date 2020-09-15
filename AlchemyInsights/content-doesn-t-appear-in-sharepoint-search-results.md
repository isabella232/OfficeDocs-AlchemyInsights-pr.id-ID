---
title: Konten tidak muncul di hasil pencarian SharePoint
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
ms.openlocfilehash: a57711434d653f5d5667776916c9251bba2370e6
ms.sourcegitcommit: c6692ce0fa1358ec3529e59ca0ecdfdea4cdc759
ms.translationtype: MT
ms.contentlocale: id-ID
ms.lasthandoff: 09/14/2020
ms.locfileid: "47713133"
---
# <a name="content-doesnt-appear-in-sharepoint-search-results"></a>Konten tidak muncul di hasil pencarian SharePoint

Ikuti langkah pemecahan masalah ini jika konten yang diharapkan tidak muncul di hasil pencarian:
  
1. Periksa bahwa **situs** yang berisi konten yang diharapkan diatur untuk memperbolehkan konten muncul di hasil pencarian. Ikuti langkah-langkah dalam [memperlihatkan konten di situs dalam hasil pencarian](https://docs.microsoft.com/sharepoint/make-site-content-searchable#show-content-on-a-site-in-search-results).

2. Periksa bahwa **Daftar** atau **pustaka** yang berisi konten yang diharapkan diatur untuk memperbolehkan konten muncul di hasil pencarian. Ikuti langkah-langkah dalam [memperlihatkan konten dari daftar atau pustaka dalam hasil pencarian](https://docs.microsoft.com/sharepoint/make-site-content-searchable#show-content-from-lists-or-libraries-in-search-results).

3. Verifikasi bahwa tata letak halaman, dokumen, atau halaman kustom diterbitkan sebagai **versi utama.** Ikuti langkah 3 di [pencarian tidak mengembalikan semua hasil di SharePoint online](https://go.microsoft.com/fwlink/?linkid=874525).

4. Verifikasi bahwa pengguna memiliki **izin** untuk menampilkan konten. Ikuti langkah-langkah dalam [memahami tingkat izin di SharePoint](https://docs.microsoft.com/sharepoint/understanding-permission-levels).
    
5. Jika skema pencarian telah diubah dengan menambahkan properti yang dikelola baru, dengan mengedit properti yang dikelola, atau dengan menghapus properti yang dikelola, maka meminta Crawl dan mengindeks ulang akan diperlukan. **Mengindeks ulang** konten dengan mengikuti langkah-langkah dalam [permintaan secara manual merayapi dan mengindeks ulang situs, pustaka atau daftar](https://docs.microsoft.com/sharepoint/crawl-site-content). Ini mungkin memakan waktu beberapa saat, tunggu 24 jam sebelum memeriksa hasilnya lagi.

Untuk informasi selengkapnya, lihat [mengaktifkan konten di situs yang akan dicari](https://docs.microsoft.com/sharepoint/make-site-content-searchable). 
  
