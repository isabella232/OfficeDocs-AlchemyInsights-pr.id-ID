---
title: penerusan email 726 memblokir
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
- "726"
- "1200004"
ms.assetid: 8865c68e-7e8a-4135-a254-d7f69f1ded30
ms.openlocfilehash: c0d9ed14f83d3c7d47e1728d5ed9ca3a19412ad2
ms.sourcegitcommit: f74c9698a31634154ce58dda8b3145bb10685ace
ms.translationtype: MT
ms.contentlocale: id-ID
ms.lasthandoff: 09/23/2020
ms.locfileid: "48219858"
---
# <a name="blocking-or-unblocking-email-forwarding"></a>Memblokir atau membuka blokir penerusan email

Untuk mengaktifkan atau menonaktifkan penerusan email untuk kotak surat tertentu, lihat [mengonfigurasi penerusan email](https://docs.microsoft.com/microsoft-365/admin/email/configure-email-forwarding).

Pada tingkat penyewa, kontrol pengalihan eksternal dilakukan menggunakan kebijakan anti spam keluar. Jika diatur ke nonaktif atau otomatis, mungkin blokir penerusan email dengan kesalahan 550 "akses 5.7.520 ditolak, organisasi Anda tidak memperbolehkan penerusan eksternal". Selanjutnya, jika pengalihan diatur ke diblokir, itu adalah kesalahan yang akan dilihat pengguna Anda.

Jika pengalihan sedang diblokir, pastikan kebijakan dikonfigurasi untuk mengaktifkan penerusan otomatis eksternal. Anda dapat memeriksa kebijakan filter spam keluar dari pusat keamanan dan kepatuhan atau dengan menjalankan perintah Get-HostedOutboundSpamFilterPolicy | FL Name, AutoForwardingMode. Jika Anda ingin menyetel pemblokiran otomatis, perintah yang sama akan memberi tahu status kebijakan Anda sekarang.

Catatan: disarankan untuk menyimpan otomatis eksternal yang dinonaktifkan pada kebijakan filter spam keluar default Anda dan mengaktifkannya hanya untuk pengguna yang memerlukan penerusan eksternal dengan membuat kebijakan kustom untuk pengguna tersebut. Anda dapat membaca selengkapnya dalam [mengonfigurasi penerusan email eksternal di Office 365](https://docs.microsoft.com/microsoft-365/security/office-365-security/external-email-forwarding).