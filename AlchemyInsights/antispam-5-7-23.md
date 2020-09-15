---
title: AntiSpam-5.7.23
ms.author: pebaum
author: pebaum
manager: mnirkhe
ms.audience: Admin
ms.topic: article
ms.service: o365-administration
ROBOTS: NOINDEX, NOFOLLOW
localization_priority: Normal
ms.collection: Adm_O365
ms.custom:
- "3156"
- "9001196"
ms.openlocfilehash: ecbce4f0077dc9acab63575c19d40c0675a406ac
ms.sourcegitcommit: c6692ce0fa1358ec3529e59ca0ecdfdea4cdc759
ms.translationtype: MT
ms.contentlocale: id-ID
ms.lasthandoff: 09/14/2020
ms.locfileid: "47717328"
---
# <a name="fix-email-delivery-issues-for-error-code-5723"></a>Memperbaiki masalah pengiriman email untuk kode kesalahan 5.7.23

Verifikasi catatan DNS SPF untuk domain Anda pada publik yang tersedia untuk SPF atau pemeriksa catatan DNS di web.

Verifikasi bahwa pesan keluar tidak diidentifikasi sebagai spam oleh Microsoft dan dirutekan melalui [kumpulan pengiriman berisiko tinggi](https://docs.microsoft.com/microsoft-365/security/office-365-security/high-risk-delivery-pool-for-outbound-messages). Pesan dalam kumpulan pengiriman berisiko tinggi tidak akan melewati pemeriksaan SPF, sehingga tidak akan diterima oleh organisasi email tujuan.

Jika masalah masih terjadi, Anda mungkin perlu menghubungi admin email host tempat Anda mencoba mengirim email. Buat catatan tentang kesalahan eksternal mendetail yang tersedia di pesan pantulan. Dukungan Microsoft mungkin tidak dapat membantu lebih lanjut.
