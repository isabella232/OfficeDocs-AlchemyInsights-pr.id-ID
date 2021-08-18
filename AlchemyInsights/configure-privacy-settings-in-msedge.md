---
title: Mengonfigurasi pengaturan privasi di Microsoft Edge
ms.author: v-aiyengar
author: AshaIyengar21
manager: dansimp
ms.date: 03/24/2021
ms.audience: Admin
ms.topic: article
ms.service: o365-administration
ROBOTS: NOINDEX, NOFOLLOW
localization_priority: Normal
ms.collection: Adm_O365
ms.custom:
- "9004632"
- "8367"
ms.openlocfilehash: 991f323249e15abd137c3e69b400e40503ed30dec6507cc5071a0b1af7f72bb3
ms.sourcegitcommit: b5f7da89a650d2915dc652449623c78be6247175
ms.translationtype: MT
ms.contentlocale: id-ID
ms.lasthandoff: 08/05/2021
ms.locfileid: "54090307"
---
# <a name="configure-privacy-settings-in-microsoft-edge"></a>Mengonfigurasi pengaturan privasi di Microsoft Edge

Secara default, Microsoft Edge disebarkan di platform non-Windows, data diagnostik, dan informasi situs tidak dikirim ke Microsoft. Namun, Microsoft Edge informasi situs dikirim Windows 10, data diagnostik dan informasi situs dikirim sesuai dengan pengaturan [data Windows pengguna.](https://go.microsoft.com/fwlink/?linkid=2132472)

Untuk mengonfigurasi Microsoft Edge mana yang menangani pengumpulan data untuk organisasi Anda, gunakan kebijakan grup berikut ini:
- [MetricsReportingEnabled](https://go.microsoft.com/fwlink/?linkid=2132470) aktif pada pelaporan penggunaan dan data terkait crash.
- [SendSiteInfoToImproveServices](https://go.microsoft.com/fwlink/?linkid=2132470) mengirimkan informasi situs yang digunakan untuk menyempurnakan layanan Microsoft.

Untuk mempelajari selengkapnya, lihat [Mengonfigurasi pengaturan kebijakan](https://go.microsoft.com/fwlink/?linkid=2132577).
