---
title: 126 Kesalahan Mendapatkan Kotak Surat di OWA?
ms.author: chrisda
author: chrisda
manager: dansimp
ms.date: 04/21/2020
ms.audience: Admin
ms.topic: article
ms.service: o365-administration
ROBOTS: NOINDEX, NOFOLLOW
localization_priority: Normal
ms.collection: Adm_O365
ms.custom:
- "126"
- "1600020"
ms.assetid: e85bffec-e5ad-418a-8561-dab6257e1864
ms.openlocfilehash: 6bab821aaa3b50c365ef5d25a61bca195c76d7ce
ms.sourcegitcommit: e552d65aac79433a911723412bf1252d20d3f0da
ms.translationtype: MT
ms.contentlocale: id-ID
ms.lasthandoff: 03/30/2021
ms.locfileid: "51426665"
---
# <a name="getting-a-mailbox-not-found-error-in-outlook-on-the-web"></a>Mendapatkan kotak surat tidak menemukan kesalahan di Outlook di web?

Jika Anda menggunakan Outlook di web dan  terjadi kesalahan ketika mendapatkan Kotak Surat tidak dapat ditemukan, akun yang Anda gunakan untuk menyambungkan ke Outlook di web tidak memiliki lisensi Exchange Online, sehingga tidak ada kotak surat yang terkait dengan akun tersebut. Admin dapat menetapkan lisensi ke akun Anda dengan mengikuti langkah-langkah berikut:

1. Buka pusat [admin Microsoft 365](https://portal.office.com/adminportal/home#/homepage) lalu masuk ke **Pengguna** **aktif** di bawah bagian Pengguna, lalu pilih pengguna yang melihat kesalahan.

2. Di halaman pengguna yang terbuka,  masuk ke bagian Lisensi  dan Aplikasi, pilih nilai Lokasi yang sesuai, dan tetapkan lisensi yang berisi Exchange Online (perluas lisensi untuk melihat detailnya). Bila Anda sudah selesai, klik **Simpan perubahan.**

Dalam beberapa kasus, jika lisensi sudah ditetapkan ke akun pengguna, menghapus dan menetapkan ulang lisensi akan membantu mengatasi masalah tersebut dan mendapatkannya dengan benar disediakan dalam sistem: 

- Periksa untuk melihat apakah langganan M365 Exchange Online (dan lainnya, jika ada) yang sedang berjalan dan belum kedaluwarsa baru-baru ini.

Setelah memastikan bahwa langganan anda belum kedaluwarsa dan lisensi yang valid telah ditetapkan ke akun pengguna, perlu waktu hingga 24 jam agar lisensi tersedia, sehingga Anda mungkin harus menunggu hingga masalah Anda atasi. Untuk informasi selengkapnya, [lihat Menetapkan dan mengelola lisensi.](https://docs.microsoft.com/deployoffice/overview-licensing-activation-microsoft-365-apps#assign-and-manage-licenses)