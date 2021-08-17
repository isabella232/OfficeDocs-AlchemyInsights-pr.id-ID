---
title: 726 Memblokir penerusan email
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
ms.openlocfilehash: 0bff7ede02809e133dc6616452ec840f552bd4fa6c45b7987d6455b2a9ba49bf
ms.sourcegitcommit: b5f7da89a650d2915dc652449623c78be6247175
ms.translationtype: MT
ms.contentlocale: id-ID
ms.lasthandoff: 08/05/2021
ms.locfileid: "54059635"
---
# <a name="blocking-or-unblocking-email-forwarding"></a>Memblokir atau membuka blokir penerusan email

Untuk mengaktifkan atau menonaktifkan penerusan email untuk kotak surat tertentu, lihat [Mengonfigurasi penerusan email](https://docs.microsoft.com/microsoft-365/admin/email/configure-email-forwarding).

Pada tingkat penyewa, kontrol penerusan eksternal dilakukan menggunakan kebijakan spam keluar. Anda bisa memeriksa kebijakan filter spam keluar dari Pusat Keamanan dan [Kepatuhan](https://protection.office.com/antispam) di sini atau dengan menggunakan perintah [Get-HostedOutboundSpamFilterPolicy](https://docs.microsoft.com/powershell/module/exchange/get-hostedoutboundspamfilterpolicy).

Jika Anda mendapatkan kesalahan berikut: **"550 5.7.520 Access denied, Your organization** does not allow external forwarding", please make sure the policy is configured to enable External Auto-forward.

**Catatan:** Kami menyarankan agar Autoforward Eksternal tetap dinonaktifkan pada kebijakan filter spam keluar default Anda dan mengaktifkannya hanya untuk pengguna yang memerlukan penerusan eksternal dengan membuat kebijakan kustom untuk pengguna tersebut. Anda bisa membaca selengkapnya [di Mengonfigurasi penerusan email eksternal Office 365](https://docs.microsoft.com/microsoft-365/security/office-365-security/external-email-forwarding).