---
title: 2491 Peringatkan pesan email dari kebijakan 'Pengelabuan Dikirim karena penyewa atau pengesamping pengguna'
ms.author: chrisda
author: chrisda
manager: dansimp
ms.date: 04/21/2020
ms.audience: ITPro
ms.topic: article
ms.service: o365-administration
ROBOTS: NOINDEX, NOFOLLOW
localization_priority: Normal
ms.custom: 2491
ms.assetid: ''
ms.openlocfilehash: 90b078147bbb1e60cba0a2de6e49a862469f93aa
ms.sourcegitcommit: ab75f66355116e995b3cb5505465b31989339e28
ms.translationtype: MT
ms.contentlocale: id-ID
ms.lasthandoff: 08/13/2021
ms.locfileid: "58316361"
---
# <a name="alert-email-messages-from-the-phish-delivered-due-to-tenant-or-user-override-policy"></a>Memberitahukan pesan email dari kebijakan 'Pengelabuan Dikirim karena penyewa atau pengesampuan pengguna'

Kebijakan pemberitahuan default yang bernama **Phish Dikirimkan** karena penyewa atau pengesampuan pengguna tersedia di organisasi dengan Pertahanan Microsoft untuk lisensi Office 365 P1 dan P2. Jika Anda menerima pemberitahuan ini, berikut langkah-langkah untuk menyelidikinya:

1. Dari pesan pemberitahuan, klik **Tampilkan Pemberitahuan** untuk masuk ke **halaman Pemberitahuan** di Pertahanan Microsoft 365 Pemberitahuan.

2. Pilih pemberitahuan untuk melihat opsi Tampilkan daftar **pesan atau** Tampilkan pesan **di Explorer**. Kedua opsi ini membawa Anda ke detail pesan, yang mencakup ID Pesan. Perhatikan bahwa link Threat Explorer akan otomatis memfilter pesan yang cocok dengan kriteria pemberitahuan. Anda mungkin perlu menyesuaikan filter tanggal di Threat Explorer.

Pesan pengelabuan (phishing) dikirimkan karena pengelabuan yang dikonfigurasi secara manual:

- Pengirim atau kumpulan domain yang diperbolehkan oleh pengguna.
- Pengirim atau domain yang diperbolehkan diatur oleh admin dalam kebijakan anti spam.
- Alamat IP yang diperbolehkan dalam kebijakan filter koneksi.
- Aturan aliran email (juga dikenal sebagai aturan transpor) yang dikonfigurasi untuk mengizinkan pesan masuk.

Jika Anda yakin bahwa pesan salah ditandai sebagai pengelabuan, gunakan [Pengiriman admin](https://docs.microsoft.com/microsoft-365/security/office-365-security/admin-submission) untuk melaporkan pesan ke Microsoft.

Pengguna dapat menggunakan add-in Pesan Laporan atau [add-in Pengelabuan](https://docs.microsoft.com/microsoft-365/security/office-365-security/enable-the-report-message-add-in) Laporan Outlook mengirimkan sampel pesan ke Microsoft.
