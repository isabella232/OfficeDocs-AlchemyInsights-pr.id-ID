---
title: Pencarian di SharePoint Online
ms.author: efrene
author: efrene
ms.audience: ITPro
ms.topic: article
ROBOTS: NOINDEX, NOFOLLOW
localization_priority: Normal
ms.assetid: fe00f4c0-44d5-49d4-9db0-a62698bcd1d1
ms.openlocfilehash: 3c3f6384172b2b4d59db6059618572db11059228
ms.sourcegitcommit: 1d98db8acb9959aba3b5e308a567ade6b62da56c
ms.translationtype: MT
ms.contentlocale: id-ID
ms.lasthandoff: 08/22/2019
ms.locfileid: "36507634"
---
# <a name="content-crawling-and-indexing-in-sharepoint-online"></a>Konten menperayapan dan mengindeks dalam SharePoint Online

Konten harus merangkak dan ditambahkan ke indeks pencarian bagi pengguna untuk menemukan apa yang mereka mencari di SharePoint Online. Konten secara otomatis merangkak berdasarkan pada jadwal yang ditetapkan merangkak (jadwal merangkak tidak berubah). Crawler mengambil konten yang telah berubah sejak terakhir merangkak dan pembaruan indeks. Untuk memastikan konten merangkak dan indeks diperbarui, perhatikan yang berikut ini:

- Pastikan konten dapat ditemukan dengan [membuat konten situs dapat dicari](https://docs.microsoft.com/sharepoint/make-site-content-searchable).

- Ketika Anda telah mengubah properti yang dikelola, atau ketika Anda telah mengubah pemetaan merangkak dan berhasil properti, situs harus kembali merangkak sebelum perubahan akan tercermin dalam indeks pencarian. 

    Karena perubahan yang dibuat pada schema Cari, dan tidak ke situs sebenarnya, crawler akan secara otomatis kembali indeks situs. 

    Untuk info lebih lanjut, lihat [manual meminta merangkak dan mengindeks ulang situs, Perpustakaan atau daftar](https://docs.microsoft.com/sharepoint/crawl-site-conten).

- Tunggu minimal 24 jam setelah secara manual meminta merangkak dan penuh kembali indeks untuk melihat jika Anda masih mengalami masalah. 

    Jika lebih dari 24 jam telah berlalu sejak memulai merangkak dan mengindeks ulang penuh, silahkan log kasus dukungan. Dalam banyak kasus, kami sudah bekerja pada sebuah solusi. Mohon berikan setidaknya 24 jam untuk menyelesaikan solusi.

> [!IMPORTANT]
> Jika sebuah situs, dokumen (Perpustakaan), atau daftar dihapus dan masih menunjukkan di hasil pencarian, pengguna akan menerima **Kesalahan 404 File tidak ditemukan** ketika mencoba untuk mengaksesnya. Masalah ini harus login sebagai kasus dukungan untuk investigasi lebih lanjut. 



