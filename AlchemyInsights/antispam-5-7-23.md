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
ms.openlocfilehash: 8122b409a731a5fcc46c718aff1eeda07e26890b
ms.sourcegitcommit: bc7d6f4f3c9f7060d073f5130e1ec856e248d020
ms.translationtype: MT
ms.contentlocale: id-ID
ms.lasthandoff: 06/02/2020
ms.locfileid: "44506446"
---
# <a name="fix-email-delivery-issues-for-error-code-5723"></a>Memperbaiki masalah pengiriman email untuk kode galat 5.7.23

Verifikasikan data DNS SPF untuk domain Anda di pemeriksa data SPF atau DNS yang tersedia untuk umum di web.

Verifikasi bahwa pesan keluar tidak diidentifikasi sebagai spam oleh Microsoft dan diarahkan melalui [Pool pengiriman berisiko tinggi](https://docs.microsoft.com/microsoft-365/security/office-365-security/high-risk-delivery-pool-for-outbound-messages). Pesan di Pool pengiriman berisiko tinggi tidak akan lulus pemeriksaan SPF, sehingga tidak akan diterima oleh organisasi email tujuan.

Jika masalah masih terjadi, Anda mungkin perlu menghubungi admin host surat yang sedang Anda coba untuk mengirim email. Catat kesalahan eksternal terperinci yang tersedia dalam pesan pentalan. Dukungan Microsoft mungkin tidak dapat membantu lebih lanjut.
