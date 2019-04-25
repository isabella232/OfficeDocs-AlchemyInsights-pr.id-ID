---
title: sama seperti nama file terbaik
ms.author: pebaum
author: pebaum
manager: jackiesm
ms.date: 4/27/2018
ms.audience: Admin
ms.topic: article
ROBOTS: NOINDEX, NOFOLLOW
localization_priority: Normal
ms.collection: Adm_O365
ms.custom: ''
ms.assetid: (guid of old soc version if any)
ms.openlocfilehash: 37398436435fb72cb5c8dca2d0798b86a0c8ccc9
ms.sourcegitcommit: 9d78905c512192ffc4675468abd2efc5f2e4baf4
ms.translationtype: MT
ms.contentlocale: id-ID
ms.lasthandoff: 04/23/2019
ms.locfileid: "32366334"
---
# <a name="required-alchemy-header-h1-h2s-dont-work"></a>Diperlukan Alkimia Header H1, H2's tidak bekerja.
Best Practices dan pedoman untuk authoring Alkimia:

1. **Tidak sarang Alkimia wawasan dalam folder**- ini akan merusak struktur url. Kami melihat ke memperbaiki ini.
1. File dalam **AlchemyInsights** folder harus memiliki nama file huruf kecil dengan tanda hubung untuk ruang ex. ***bagaimana-untuk-Aktifkan--penahanan litigasi***.
    1. Termasuk aturan ID atau ember ID dari [portal Alkimia mitra](https://alchemyportal.azurewebsites.net) di bidang ms.custom. mantan. ***Ms.Custom: 100021***
1. Menggunakan sisa metadata di bagian atas dari file ini sebagai template Anda.
1. Di [portal mitra Alkimia](https://alchemyportal.azurewebsites.net), menavigasi ke bagian **judul wawasan pelanggan:** dan menggunakannya sebagai awal titik untuk judul H1 Anda untuk wawasan. 
    > [!NOTE]
    > Alkimia wawasan harus memiliki hanya satu H1 di bagian atas atau mereka akan istirahat dalam produksi. H2s tidak membuat begitu menggunakan **bold** atau lain Konvensi untuk menandai bagian terpisah.
1. Selanjutnya, mengisi di dalam tubuh teks menggunakan bahan rancangan di bagian Customer wawasan halaman aturan Alkimia
    1. Bullet daftar baik-baik saja
    1. Nomor Daftar terlalu
    1. **Tebal** dan *miring* adalah OK
    1. Link harus selalu menjadi salah satu **"link web" / eksternal** OR **deep-link ke elemen UI**, tidak internal link.
    1. Gambar tidak secara resmi didukung saat ini, tetapi itu adalah pada peta jalan.

Dan ini benar-benar sudah agak terlalu lama. Praktek terbaik adalah sekitar 400 karakter---

Setelah konten Anda siap, menariknya ke cabang hidup. Kemudian, pergi ke [portal mitra Alkimia](https://alchemyportal.azurewebsites.net) dan masukkan nama file ke bidang url. M