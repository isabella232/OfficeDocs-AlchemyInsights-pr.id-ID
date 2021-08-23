---
title: Apakah Anda ingin melaporkan spam positif palsu ke Microsoft?
ms.author: chrisda
author: chrisda
manager: dansimp
ms.audience: ITPro
ms.topic: article
ms.service: o365-administration
ROBOTS: NOINDEX, NOFOLLOW
localization_priority: Normal
ms.custom:
- "975"
- "666"
- "3100019"
ms.openlocfilehash: d3897f24ce9a967b08a3fd15a2fdedbb3fe2a22d
ms.sourcegitcommit: f05d4caa0e657ee74d6b6e9abc88488f17d740fe
ms.translationtype: MT
ms.contentlocale: id-ID
ms.lasthandoff: 08/19/2021
ms.locfileid: "58396618"
---
# <a name="do-you-have-legitimate-messages-being-marked-as-spam"></a>Apakah Anda memiliki pesan sah yang ditandai sebagai spam?

Ini membuat frustasi saat email yang sah berakhir di folder Sampah atau di Karantina. Pertimbangkan alasan paling umum untuk positif palsu berikut:

**Penggantian penyewa (yang paling umum)** Fitur ini sepenuhnya berada di dalam kontrol Untuk memulihkan.

Kirimkan pesan di Pertahanan Microsoft 365 untuk analisis kebijakan dan aturan yang mempengaruhi; detail kembaliscan tersedia dalam waktu beberapa menit.
Tinjau atau ubah kebijakan atau aturan sebagaimana berlaku. 

**Menimpa Pengguna Akhir (umum)** Fitur ini sepenuhnya berada di dalam kontrol Untuk memulihkan. 

Kirimkan pesan di Pertahanan Microsoft 365 untuk analisis kebijakan dan aturan yang mempengaruhi; detail kembaliscan tersedia dalam waktu beberapa menit. 

Jika pesan diblokir karena dikirim dari alamat dalam daftar Pengirim yang Diblokir oleh pengguna, header menyertakan Putusan Pemfilteran Spam "SFV:BLK".

**Autentikasi email pengirim** Perbaikan dilakukan sebagian dari kontrol Anda.

Kirim pesan untuk menganalisis kegagalan dalam autentikasi email pengirim pada saat pengiriman; hasil tersedia dalam satu hari. 

Jika memiliki infrastruktur pengiriman, tinjau cara meratanya dengan SPF, DKIM, dan DMARC untuk memastikan bahwa sistem email tujuan mempercayai pesan yang dikirim dari domain Anda. Alternatifnya, hubungi pengirim untuk mengatasi konfigurasi DNS mereka.

**Pemfilteran Microsoft** Perbaikan dilakukan sebagian dari kontrol Anda.

Mengirimkan pesan dan melaporkan pesan tersebut sebagai aman; hasil pemindaian kembali tersedia dalam sehari. Gunakan Daftar Perbolehkan/Blokir Penyewa ketika Anda tidak setuju dengan pemfilteran putusan dalam situasi tertentu. Namun, Anda sebaiknya jangan melewati pemfilteran Microsoft secara permanen. 

Untuk informasi selengkapnya, lihat:

- Aktifkan pengguna akhir Anda untuk mengirimkan pesan ke Microsoft. Microsoft menggunakan pengiriman ini untuk meningkatkan efektivitas teknologi proteksi email, dan muncul dalam laporan pengiriman untuk Anda gunakan sebagai petunjuk untuk memperbarui kebijakan. 

- Untuk menonton video singkat tentang mengirimkan pesan untuk analisis, lihat [Mengirim pesan untuk analisis](https://go.microsoft.com/fwlink/?linkid=2166435).

- [Menggunakan Kiriman Admin untuk mengirimkan spam, phish, URL, dan file yang dicurigai sebagai spam, URL, dan file ke Microsoft](https://docs.microsoft.com/microsoft-365/security/office-365-security/admin-submission)

- [Mengelola Penyewa Perbolehkan/Memblokir Daftar](https://docs.microsoft.com/microsoft-365/security/office-365-security/tenant-allow-block-list)

- [Header pesan anti spam di Microsoft 365](https://docs.microsoft.com/microsoft-365/security/office-365-security/anti-spam-message-headers)

- [Proteksi spam keluar di EOP](https://docs.microsoft.com/microsoft-365/security/office-365-security/outbound-spam-controls)