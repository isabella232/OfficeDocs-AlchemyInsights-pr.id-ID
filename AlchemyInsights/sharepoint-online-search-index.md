---
title: Cari di SharePoint online
ms.author: pebaum
author: pebaum
ms.audience: ITPro
ms.topic: article
ROBOTS: NOINDEX, NOFOLLOW
localization_priority: Normal
ms.assetid: fe00f4c0-44d5-49d4-9db0-a62698bcd1d1
ms.openlocfilehash: c4ff98f0cf928834c803542340b32da15a40d583
ms.sourcegitcommit: 0f0186044a3597e42ad14c32ca58e7224344dcfa
ms.translationtype: MT
ms.contentlocale: id-ID
ms.lasthandoff: 12/15/2019
ms.locfileid: "40044046"
---
# <a name="content-crawling-and-indexing-in-sharepoint-online"></a>Konten merangkak dan indeks di SharePoint online

Konten harus dirayapi dan ditambahkan ke indeks pencarian bagi pengguna untuk menemukan apa yang mereka Cari di SharePoint online. Konten secara otomatis dirayapi berdasarkan jadwal perayapan yang telah ditetapkan sebelumnya (jadwal perayapan tidak dapat diubah). Crawler mengambil konten yang telah berubah sejak Crawl terakhir dan memperbarui indeks. Untuk memastikan konten dirayapi dan indeks diperbarui, Perhatikan hal berikut:

- Pastikan konten dapat ditemukan dengan [membuat konten situs dicari](https://docs.microsoft.com/sharepoint/make-site-content-searchable).

- Bila Anda telah mengubah properti terkelola, atau bila Anda telah mengubah pemetaan properti yang dirayapi dan terkelola, situs harus dirayapi ulang sebelum perubahan Anda akan terlihat di indeks penelusuran. 

    Karena perubahan yang dibuat di skema pencarian, dan bukan ke situs aktual, perayap tidak akan secara otomatis mengindeks ulang situs. 

    Untuk info selengkapnya, lihat [secara manual meminta perayapan dan mengindeks ulang situs, Perpustakaan, atau daftar](https://docs.microsoft.com/sharepoint/crawl-site-conten).

- Tunggu minimal 24 jam setelah meminta perayapan dan indeks ulang penuh secara manual untuk mengetahui apakah Anda masih mengalami masalah. 

    Jika lebih dari 24 jam telah berlalu sejak Anda memulai Crawl dan Full Re-index, silakan log kasus dukungan. Dalam banyak kasus, kami telah bekerja pada solusi. Tolong beri kami setidaknya 24 jam untuk menyelesaikan solusi.

> [!IMPORTANT]
> Jika situs, dokumen (Perpustakaan), atau daftar telah dihapus dan masih menunjukkan di hasil pencarian, pengguna akan menerima **galat 404 file tidak ditemukan** ketika mencoba untuk mengaksesnya. Masalah ini harus dicatat sebagai kasus dukungan untuk penyelidikan lebih lanjut. 



