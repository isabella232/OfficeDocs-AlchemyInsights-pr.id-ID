---
title: AntiSpam-5.7.23
ms.author: pebaum
author: pebaum
manager: mnirkhe
ms.audience: Admin
ms.topic: article
ROBOTS: NOINDEX, NOFOLLOW
localization_priority: Normal
ms.collection: Adm_O365
ms.custom:
- "3156"
- "9001196"
ms.openlocfilehash: 307b738c40c620d057e68eff7d218c8c9b5eb665
ms.sourcegitcommit: 55eff703a17e500681d8fa6a87eb067019ade3cc
ms.translationtype: MT
ms.contentlocale: id-ID
ms.lasthandoff: 04/22/2020
ms.locfileid: "43676500"
---
# <a name="fix-email-delivery-issues-for-error-code-5723"></a>Memperbaiki masalah pengiriman email untuk kode galat 5.7.23

Verifikasikan data DNS SPF untuk domain Anda di pemeriksa data SPF atau DNS yang tersedia untuk umum di web.

Verifikasi bahwa pesan keluar tidak diidentifikasi sebagai spam oleh Microsoft dan diarahkan melalui [Pool pengiriman berisiko tinggi](https://docs.microsoft.com/office365/SecurityCompliance/high-risk-delivery-pool-for-outbound-messages). Pesan di Pool pengiriman berisiko tinggi tidak akan lulus pemeriksaan SPF, sehingga tidak akan diterima oleh organisasi email tujuan.

Jika masalah masih terjadi, Anda mungkin perlu menghubungi admin host surat yang sedang Anda coba untuk mengirim email. Catat kesalahan eksternal terperinci yang tersedia dalam pesan pentalan. Dukungan Microsoft mungkin tidak dapat membantu lebih lanjut.
