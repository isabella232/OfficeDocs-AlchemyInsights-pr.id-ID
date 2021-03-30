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
ms.openlocfilehash: 2367a7a55d1837fa7c7095fd0ac10ff1cf7ae72d
ms.sourcegitcommit: db908b3da2c7a6508a77bf4f2c80afb294fadbd1
ms.translationtype: MT
ms.contentlocale: id-ID
ms.lasthandoff: 03/29/2021
ms.locfileid: "51405105"
---
# <a name="configure-privacy-settings-in-microsoft-edge"></a>Mengonfigurasi pengaturan privasi di Microsoft Edge

Secara default, jika Microsoft Edge digunakan di platform non-Windows, data diagnostik dan informasi situs tidak akan dikirim ke Microsoft. Namun, jika Microsoft Edge disebarkan di Windows 10, data diagnostik dan informasi situs akan dikirim sesuai dengan pengaturan [data Diagnostik Windows pengguna.](https://go.microsoft.com/fwlink/?linkid=2132472)

Untuk mengonfigurasi cara Microsoft Edge menangani pengumpulan data untuk organisasi Anda, gunakan kebijakan grup berikut:
- [MetricsReportingEnabled](https://go.microsoft.com/fwlink/?linkid=2132470) aktif pada pelaporan penggunaan dan data terkait crash.
- [SendSiteInfoToImproveServices](https://go.microsoft.com/fwlink/?linkid=2132470) mengirimkan informasi situs yang digunakan untuk meningkatkan layanan Microsoft.

Untuk mempelajari selengkapnya, lihat [Mengonfigurasi pengaturan kebijakan](https://go.microsoft.com/fwlink/?linkid=2132577).
