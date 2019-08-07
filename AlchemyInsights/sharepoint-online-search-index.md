---
title: Pencarian di SharePoint Online
ms.author: efrene
author: efrene
ms.audience: ITPro
ms.topic: article
ROBOTS: NOINDEX, NOFOLLOW
localization_priority: Normal
ms.assetid: fe00f4c0-44d5-49d4-9db0-a62698bcd1d1
ms.openlocfilehash: fc49978fbd2c07381dae83061b1a1868cd1df0d0
ms.sourcegitcommit: 327a2c77afc2ff3d67d3aaaea1a92068a3c4bb1f
ms.translationtype: MT
ms.contentlocale: id-ID
ms.lasthandoff: 08/06/2019
ms.locfileid: "36059255"
---
# <a name="search-in-sharepoint-online"></a>Pencarian di SharePoint Online

Konten harus merangkak dan ditambahkan ke indeks pencarian bagi pengguna untuk menemukan apa yang mereka mencari di SharePoint Online. Konten secara otomatis merangkak berdasarkan pada jadwal yang ditetapkan merangkak (jadwal merangkak tidak berubah). Crawler mengambil konten yang telah berubah sejak terakhir merangkak dan pembaruan indeks. Untuk memastikan konten merangkak dan indeks diperbarui, perhatikan yang berikut ini:

- Pastikan konten dapat ditemukan dengan [membuat konten situs dapat dicari](https://docs.microsoft.com/sharepoint/make-site-content-searchable).

- Ketika Anda telah mengubah properti yang dikelola, atau ketika Anda telah mengubah pemetaan merangkak dan berhasil properti, situs harus kembali merangkak sebelum perubahan akan tercermin dalam indeks pencarian. 

    Karena perubahan yang dibuat pada schema Cari, dan tidak ke situs sebenarnya, crawler akan secara otomatis kembali indeks situs. 

    Untuk info lebih lanjut, lihat [manual meminta merangkak dan mengindeks ulang situs, Perpustakaan atau daftar](https://docs.microsoft.com/sharepoint/crawl-site-conten).

- Tunggu minimal 24 jam setelah secara manual meminta merangkak dan penuh kembali indeks untuk melihat jika Anda masih mengalami masalah. 

    Jika lebih dari 24 jam telah berlalu sejak memulai merangkak dan mengindeks ulang penuh, silahkan log kasus dukungan. Dalam banyak kasus, kami sudah bekerja pada sebuah solusi. Mohon berikan setidaknya 24 jam untuk menyelesaikan solusi.

>[! Penting!]: jika sebuah situs, dokumen (Perpustakaan) atau daftar dihapus dan masih menunjukkan di hasil pencarian, pengguna akan menerima **Kesalahan 404 File tidak ditemukan** ketika mencoba untuk mengaksesnya. Masalah ini harus login sebagai kasus dukungan untuk investigasi lebih lanjut. 



