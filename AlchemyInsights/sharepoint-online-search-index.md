---
title: Mengelola pencarian kamus di SharePoint Online
ms.author: kirks
author: Techwriter40
ms.audience: ITPro
ms.topic: article
ROBOTS: NOINDEX, NOFOLLOW
localization_priority: Normal
ms.assetid: fe00f4c0-44d5-49d4-9db0-a62698bcd1d1
ms.openlocfilehash: c2960093bb1cfb649c26528c9f671e6d720ff237
ms.sourcegitcommit: 241e21b6da226563bf70bdb1f5bad3d91c38cd2c
ms.translationtype: MT
ms.contentlocale: id-ID
ms.lasthandoff: 06/05/2019
ms.locfileid: "34736056"
---
# <a name="search-in-sharepoint-online"></a>Pencarian di SharePoint Online

Konten harus merangkak dan ditambahkan ke indeks pencarian bagi pengguna untuk menemukan apa yang mereka mencari di SharePoint Online. Konten secara otomatis merangkak berdasarkan pada jadwal yang ditetapkan merangkak (jadwal merangkak tidak berubah). Crawler mengambil konten yang telah berubah sejak terakhir merangkak dan pembaruan indeks. Untuk memastikan konten merangkak dan indeks diperbarui, ikuti langkah berikut.

Pastikan konten dapat ditemukan dengan membuat konten situs dapat dicari. Untuk info lebih lanjut, lihat [mengaktifkan konten di situs harus dicari](https://docs.microsoft.com/en-us/sharepoint/make-site-content-searchable).

Ketika Anda telah mengubah properti yang dikelola, atau ketika Anda telah mengubah pemetaan merangkak dan berhasil properti, situs harus kembali merangkak sebelum perubahan akan tercermin dalam indeks pencarian. 

Karena perubahan yang dibuat pada schema Cari, dan tidak ke situs sebenarnya, crawler akan secara otomatis kembali indeks situs. 

Untuk info lebih lanjut, lihat [manual meminta merangkak dan mengindeks ulang situs, Perpustakaan atau daftar](https://docs.microsoft.com/en-us/sharepoint/crawl-site-conten).

 Tunggu minimal 24 jam setelah secara manual meminta merangkak dan penuh kembali indeks untuk melihat jika Anda masih mengalami masalah. 

Jika lebih dari 24 jam telah berlalu sejak memulai merangkak dan mengindeks ulang penuh, silahkan log kasus dukungan. Dalam banyak kasus, kami sudah bekerja pada sebuah solusi. Mohon berikan setidaknya 24 jam untuk menyelesaikan solusi.

**Penting**: jika sebuah situs, dokumen (Perpustakaan) atau daftar dihapus dan masih menunjukkan di hasil pencarian, pengguna akan menerima kesalahan 404 File tidak ditemukan ketika mencoba untuk mengakses. Masalah ini harus login sebagai kasus dukungan untuk investigasi lebih lanjut. 



