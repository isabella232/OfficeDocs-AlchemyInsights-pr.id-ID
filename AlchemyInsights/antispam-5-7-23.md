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
ms.openlocfilehash: e494e8017f24d65a94d1a7490be4d67c46a2120b
ms.sourcegitcommit: 8bc60ec34bc1e40685e3976576e04a2623f63a7c
ms.translationtype: MT
ms.contentlocale: id-ID
ms.lasthandoff: 04/15/2021
ms.locfileid: "51821414"
---
# <a name="fix-email-delivery-issues-for-error-code-5723"></a>Memperbaiki masalah pengiriman email untuk kode kesalahan 5.7.23

Memverifikasi catatan DNS SPF untuk domain Anda di pemeriksa catatan DNS atau SPF yang tersedia untuk publik di web.

Verifikasi bahwa pesan keluar tidak diidentifikasi sebagai spam oleh Microsoft dan dirutekan melalui [Kolam Pengiriman Risiko Tinggi.](https://docs.microsoft.com/microsoft-365/security/office-365-security/high-risk-delivery-pool-for-outbound-messages) Pesan dalam Kolam Pengiriman Risiko Tinggi tidak akan lolos pemeriksaan SPF, dan oleh karena itu tidak akan diterima oleh organisasi email tujuan.

Jika masalah tetap ada, Anda mungkin perlu menghubungi admin host email tempat Anda mencoba mengirim email. Catat kesalahan eksternal mendetail yang tersedia dalam pesan terpental. Dukungan Microsoft mungkin tidak dapat membantu lebih lanjut.
