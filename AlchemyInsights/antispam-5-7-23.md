---
title: Antispam - 5.7.23
ms.author: pebaum
author: pebaum
manager: scotv
ms.audience: Admin
ms.topic: article
ms.service: o365-administration
ROBOTS: NOINDEX, NOFOLLOW
localization_priority: Normal
ms.collection: Adm_O365
ms.custom:
- "3156"
- "9001196"
ms.openlocfilehash: cb9073306c65b09813290d6c8470d14395d2836fa3048f8ce0ecb8b06e71a010
ms.sourcegitcommit: b5f7da89a650d2915dc652449623c78be6247175
ms.translationtype: MT
ms.contentlocale: id-ID
ms.lasthandoff: 08/05/2021
ms.locfileid: "53932172"
---
# <a name="fix-email-delivery-issues-for-error-code-5723"></a>Memperbaiki masalah pengiriman email untuk kode kesalahan 5.7.23

Memverifikasi catatan DNS SPF untuk domain Anda di pemeriksa catatan DNS atau SPF yang tersedia untuk publik di web.

Verifikasi bahwa pesan keluar tidak diidentifikasi sebagai spam oleh Microsoft dan dirutekan melalui [Kolam Pengiriman Risiko Tinggi.](https://docs.microsoft.com/microsoft-365/security/office-365-security/high-risk-delivery-pool-for-outbound-messages) Pesan dalam Kolam Pengiriman Risiko Tinggi tidak akan lolos pemeriksaan SPF, dan oleh karena itu tidak akan diterima oleh organisasi email tujuan.

Jika masalah tetap ada, Anda mungkin perlu menghubungi admin host email tempat Anda mencoba mengirim email. Catat kesalahan eksternal mendetail yang tersedia dalam pesan terpental. Dukungan Microsoft mungkin tidak dapat membantu lebih lanjut.
