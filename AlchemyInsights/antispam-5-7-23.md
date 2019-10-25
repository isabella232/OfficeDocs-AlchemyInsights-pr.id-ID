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
ms.openlocfilehash: 9c9bc2d04fb8efaa5e75194b4ca09316d24e018e
ms.sourcegitcommit: 07b47d7f3ca191363e6bc84140e8e01524d6f08e
ms.translationtype: MT
ms.contentlocale: id-ID
ms.lasthandoff: 10/24/2019
ms.locfileid: "37682176"
---
# <a name="fix-email-delivery-issues-for-error-code-5723"></a>Memperbaiki masalah pengiriman email untuk kode galat 5.7.23

Verifikasikan data DNS SPF untuk domain Anda di pemeriksa data SPF atau DNS yang tersedia untuk umum di web.

Verifikasi bahwa pesan keluar tidak diidentifikasi sebagai spam oleh Office 365 dan diarahkan melalui [Pool pengiriman risiko tinggi](https://docs.microsoft.com/office365/SecurityCompliance/high-risk-delivery-pool-for-outbound-messages). Pesan di Pool pengiriman berisiko tinggi tidak akan lulus pemeriksaan SPF, sehingga tidak akan diterima oleh organisasi email tujuan.

Jika masalah masih terjadi, Anda mungkin perlu menghubungi admin host surat yang sedang Anda coba untuk mengirim email. Catat kesalahan eksternal terperinci yang tersedia dalam pesan pentalan.  Dukungan Office 365 mungkin tidak dapat membantu lebih lanjut.