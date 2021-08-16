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
ms.openlocfilehash: aca0371dad9ba43fa21b0df8e50f1b8ee536528af90d6bda401995c6e5796be4
ms.sourcegitcommit: b5f7da89a650d2915dc652449623c78be6247175
ms.translationtype: MT
ms.contentlocale: id-ID
ms.lasthandoff: 08/05/2021
ms.locfileid: "54056493"
---
# <a name="getting-a-mailbox-not-found-error-in-outlook-on-the-web"></a>Mendapatkan kotak surat tidak menemukan kesalahan di Outlook di web?

Jika Anda menggunakan Outlook di web dan mendapatkan kesalahan  Kotak Surat tidak dapat ditemukan, akun yang digunakan untuk menyambungkan ke Outlook di web tidak memiliki lisensi Exchange Online sehingga, tidak ada kotak surat yang terkait dengan akun tersebut. Admin dapat menetapkan lisensi ke akun Anda dengan mengikuti langkah-langkah berikut:

1. Buka [pusat admin Microsoft 365](https://portal.office.com/adminportal/home#/homepage) masuk ke **Pengguna aktif** di **bawah bagian** Pengguna, dan pilih pengguna yang melihat kesalahan.

2. Di halaman pengguna yang terbuka,  masuk ke bagian Lisensi  dan Aplikasi, pilih nilai Lokasi yang sesuai, dan tetapkan lisensi yang berisi Exchange Online (perluas lisensi untuk melihat detailnya). Bila Anda sudah selesai, klik **Simpan perubahan.**

Dalam beberapa kasus, jika lisensi sudah ditetapkan ke akun pengguna, menghapus dan menetapkan ulang lisensi akan membantu mengatasi masalah tersebut dan mendapatkannya dengan benar disediakan dalam sistem: 

- Periksa apakah langganan M365 Exchange Online (dan lainnya, jika ada) yang sedang dilakukan dan belum berakhir baru-baru ini.

Setelah memastikan bahwa langganan anda belum kedaluwarsa dan lisensi yang valid telah ditetapkan ke akun pengguna, perlu waktu hingga 24 jam agar lisensi tersedia, sehingga Anda mungkin harus menunggu hingga masalah Anda atasi. Untuk informasi selengkapnya, [lihat Menetapkan dan mengelola lisensi.](https://docs.microsoft.com/deployoffice/overview-licensing-activation-microsoft-365-apps#assign-and-manage-licenses)