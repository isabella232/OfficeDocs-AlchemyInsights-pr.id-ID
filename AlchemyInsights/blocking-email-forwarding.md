---
title: Memblokir atau membuka blokir penerusan email otomatis eksternal
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
ms.openlocfilehash: fe9e52023b809b38c43332a10a1184d114798cfe
ms.sourcegitcommit: ab75f66355116e995b3cb5505465b31989339e28
ms.translationtype: MT
ms.contentlocale: id-ID
ms.lasthandoff: 08/13/2021
ms.locfileid: "58315877"
---
# <a name="block-or-unblock-eternal-automatic-email-forwarding"></a>Memblokir atau membuka blokir penerusan email otomatis memblokir

Untuk mengaktifkan atau menonaktifkan penerusan email untuk kotak surat tertentu, lihat [Mengonfigurasi penerusan email](https://docs.microsoft.com/microsoft-365/admin/email/configure-email-forwarding).

Admin dapat mengontrol penerusan eksternal untuk organisasi menggunakan [kebijakan spam keluar.](https://docs.microsoft.com/microsoft-365/security/office-365-security/configure-the-outbound-spam-policy) Anda mengelola kebijakan spam keluar di portal Pertahanan Microsoft 365 di atau dengan menggunakan <https://security.microsoft.com/antispam> cmdlet [Get-HostedOutboundSpamFilterPolicy](https://docs.microsoft.com/powershell/module/exchange/get-hostedoutboundspamfilterpolicy) Exchange Online PowerShell.

Jika Anda menerima kesalahan berikut: **"550 5.7.520 Access denied, Your organization** does not allow external forwarding", make sure the policy is configured to enable external auto-forwarded messages.

**Catatan**: Kami menyarankan nilai default Otomatis  **-** Sistem dikontrol untuk pengaturan Aturan penerusan otomatis dalam kebijakan filter spam keluar default Anda (penerusan eksternal otomatis diblokir; penerusan otomatis internal masih berfungsi). Anda harus membuat kebijakan filter spam keluar kustom dan menggunakan nilai **Aktif - Penerusan** diaktifkan hanya untuk pengguna yang memerlukan penerusan email otomatis eksternal. Untuk informasi selengkapnya, [lihat Mengonfigurasi penerusan email eksternal Office 365](https://docs.microsoft.com/microsoft-365/security/office-365-security/external-email-forwarding).
