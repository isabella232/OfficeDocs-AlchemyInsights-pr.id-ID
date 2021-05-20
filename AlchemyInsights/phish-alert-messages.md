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
ms.openlocfilehash: 2b373423cf3e63b76a62465dd62076c023580e94
ms.sourcegitcommit: f4866e94918c7b591ad0cd3b58169d340bcc7f00
ms.translationtype: MT
ms.contentlocale: id-ID
ms.lasthandoff: 05/19/2021
ms.locfileid: "52544581"
---
# <a name="alert-email-messages-from-the-phish-delivered-due-to-tenant-or-user-override-policy"></a>Memberitahukan pesan email dari kebijakan 'Pengelabuan Dikirim karena penyewa atau pengesampuan pengguna'

Kebijakan pemberitahuan default bernama "Phish Delivered due to tenant or user override" telah diluncurkan kepada penyewa dengan Pertahanan Microsoft untuk lisensi Office 365 P1 dan P2. Jika Anda menerima pemberitahuan ini, berikut langkah-langkah untuk menyelidikinya:

1. Dari pesan pemberitahuan, klik **Tampilkan Pemberitahuan** untuk masuk ke **halaman Pemberitahuan** di Pusat & Kepatuhan.

2. Pilih pemberitahuan untuk melihat opsi Tampilkan daftar **pesan atau** Tampilkan pesan **di Explorer**. Kedua opsi ini membawa Anda ke detail pesan, yang mencakup ID Pesan. Perhatikan bahwa link Threat Explorer akan otomatis memfilter pesan yang cocok dengan kriteria pemberitahuan. Anda mungkin perlu menyesuaikan filter tanggal di Threat Explorer.

Pesan pengelabuan (phishing) dikirimkan karena pengelabuan yang dikonfigurasi secara manual:

- Pengirim atau kumpulan domain yang diperbolehkan oleh pengguna.

- Pengirim atau domain yang diperbolehkan diatur oleh admin dalam kebijakan anti spam.

- Alamat IP yang diperbolehkan dalam kebijakan filter koneksi.

- Aturan aliran email (juga dikenal sebagai aturan transpor) yang dikonfigurasi untuk mengizinkan pesan masuk.

Jika Anda yakin bahwa pesan tidak ditandai sebagai pengelabuan (phish), gunakan [add-in](https://support.office.com/article/b5caa9f1-cdf3-4443-af8c-ff724ea719d2) Outlook Report Message untuk mengirimkan sampel pesan ke Microsoft.
