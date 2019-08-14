---
title: Pesan 2491 alert email dari kebijakan 'Terkirim Phish karena pengguna atau penyewa menimpa'
ms.author: chrisda
author: chrisda
manager: dansimp
ms.date: ''
ms.audience: ITPro
ms.topic: article
ROBOTS: NOINDEX, NOFOLLOW
localization_priority: Normal
ms.custom: 2491
ms.assetid: ''
ms.openlocfilehash: 456b186ecea59422c791c79d4df056ad8446bc70
ms.sourcegitcommit: 7c90dcc570d32ebd968e3e4e816a7b482890b3a4
ms.translationtype: MT
ms.contentlocale: id-ID
ms.lasthandoff: 08/13/2019
ms.locfileid: "36391340"
---
# <a name="alert-email-messages-from-the-phish-delivered-due-to-tenant-or-user-override-policy"></a>Email pemberitahuan pesan dari 'Terkirim Phish karena pengguna atau penyewa menimpa' kebijakan

Kebijakan alert default bernama "Phish disampaikan karena menimpa penyewa atau pengguna" telah digulirkan untuk penyewa dengan lisensi Office 365 ATP P1 dan P2. Jika Anda menerima peringatan ini, berikut adalah langkah-langkah untuk menyelidiki:

1. Dari pesan peringatan, klik **Lihat waspada** untuk pergi ke halaman **peringatan** dalam & keamanan Compliance Center.

2. Pilih waspada untuk melihat pilihan untuk **tampilan daftar pesan** atau **Pesan Lihat dalam Explorer**. Kedua pilihan ini membawa Anda ke rincian pesan, termasuk pesan ID. Perhatikan bahwa ancaman Explorer link secara otomatis akan menyaring pesan yang sesuai kriteria waspada. Anda mungkin perlu menyesuaikan tanggal filter di Explorer ancaman.

Pesan phishing disampaikan karena menimpa dikonfigurasi secara manual:

- Diperbolehkan pengirim atau domain yang ditetapkan oleh pengguna.

- Diperbolehkan pengirim atau domain yang ditetapkan oleh admin dalam kebijakan anti spam.

- Alamat IP yang diizinkan dalam kebijakan filter koneksi.

- Mail aliran aturan (juga dikenal sebagai aturan transport) yang dikonfigurasi untuk membolehkan pesan di.

Jika Anda yakin pesan salah ditandai sebagai phish, menggunakan Outlook [laporan pesan Tambah-in](https://support.office.com/article/b5caa9f1-cdf3-4443-af8c-ff724ea719d2) untuk mengirimkan pesan sampel ke Microsoft.
