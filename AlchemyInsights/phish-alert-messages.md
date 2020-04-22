---
title: 2491 pesan email peringatan dari ' Phish disampaikan karena penghuni atau pengguna menimpa ' kebijakan
ms.author: chrisda
author: chrisda
manager: dansimp
ms.date: 04/21/2020
ms.audience: ITPro
ms.topic: article
ROBOTS: NOINDEX, NOFOLLOW
localization_priority: Normal
ms.custom: 2491
ms.assetid: ''
ms.openlocfilehash: 2e4efd504304da757687e697ff23374aeea31851
ms.sourcegitcommit: 55eff703a17e500681d8fa6a87eb067019ade3cc
ms.translationtype: MT
ms.contentlocale: id-ID
ms.lasthandoff: 04/22/2020
ms.locfileid: "43758931"
---
# <a name="alert-email-messages-from-the-phish-delivered-due-to-tenant-or-user-override-policy"></a>Pesan email peringatan dari ' Phish disampaikan karena penyewa atau pengguna menimpa ' kebijakan

Kebijakan peringatan default bernama "dikirim phish karena penghuni atau pengguna menimpa" telah diluncurkan ke penyewa dengan Office 365 ATP P1 dan P2 lisensi. Jika Anda menerima peringatan ini, berikut adalah langkah untuk menyelidiki:

1. Dari pesan peringatan, klik **Lihat peringatan** untuk membuka halaman **peringatan** di pusat kepatuhan & keamanan.

2. Pilih peringatan untuk melihat pilihan untuk melihat **Daftar pesan** atau **melihat pesan di Explorer**. Kedua pilihan ini akan membawa Anda ke rincian pesan, yang mencakup ID pesan. Perhatikan bahwa tautan Threat Explorer akan secara otomatis menyaring pesan yang sesuai dengan kriteria peringatan. Anda mungkin perlu menyesuaikan filter tanggal di Threat Explorer.

Pesan phishing dikirim karena menimpa dikonfigurasi secara manual:

- Pengirim atau domain yang diizinkan yang ditetapkan oleh pengguna.

- Pengirim atau domain yang diizinkan yang ditetapkan oleh admin dalam kebijakan anti-spam.

- Alamat IP yang diizinkan dalam kebijakan filter sambungan.

- Aturan aliran e-mail (juga dikenal sebagai aturan transport) yang dikonfigurasi untuk membolehkan pesan.

Jika Anda yakin pesan salah ditandai sebagai Phish, gunakan Outlook [pesan laporan Add-in](https://support.office.com/article/b5caa9f1-cdf3-4443-af8c-ff724ea719d2) untuk mengirimkan sampel pesan ke Microsoft.
