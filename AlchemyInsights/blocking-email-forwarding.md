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
ms.openlocfilehash: 2f3528375d251542fd82761d00c776706de2e23c
ms.sourcegitcommit: f7b82f75a5400e992ecbd48a666783354e2e2871
ms.translationtype: MT
ms.contentlocale: id-ID
ms.lasthandoff: 10/15/2020
ms.locfileid: "48473104"
---
# <a name="blocking-or-unblocking-email-forwarding"></a>Memblokir atau membuka blokir penerusan email

Untuk mengaktifkan atau menonaktifkan penerusan email untuk kotak surat tertentu, lihat [mengonfigurasi penerusan email](https://docs.microsoft.com/microsoft-365/admin/email/configure-email-forwarding).

Pada tingkat penyewa, kontrol pengalihan eksternal dilakukan menggunakan kebijakan spam keluar. Anda dapat memeriksa kebijakan filter spam keluar dari pusat keamanan dan kepatuhan [di sini] ( https://protection.office.com/antispam) atau dengan menggunakan [perintah Get-HostedOutboundSpamFilterPolicy](https://docs.microsoft.com/powershell/module/exchange/get-hostedoutboundspamfilterpolicy).

Jika Anda mendapatkan kesalahan berikut: **"550 5.7.520 Access ditolak, organisasi Anda tidak memperbolehkan penerusan eksternal"**, pastikan kebijakan dikonfigurasi untuk mengaktifkan penerusan otomatis eksternal.

**Catatan:** Disarankan untuk menyimpan otomatis eksternal dinonaktifkan pada kebijakan filter spam keluar default Anda dan mengaktifkannya hanya untuk pengguna yang memerlukan penerusan eksternal dengan membuat kebijakan kustom untuk pengguna tersebut. Anda dapat membaca selengkapnya dalam [mengonfigurasi penerusan email eksternal di Office 365](https://docs.microsoft.com/microsoft-365/security/office-365-security/external-email-forwarding).