---
title: Microsoft Edge mengonfigurasi pengaturan privasi
ms.author: v-smandalika
author: v-smandalika
manager: dansimp
ms.date: 12/03/2020
ms.audience: Admin
ms.topic: article
ms.service: o365-administration
ROBOTS: NOINDEX, NOFOLLOW
localization_priority: Normal
ms.collection: Adm_O365
ms.custom:
- "9003843"
- "6892"
ms.openlocfilehash: 24721325aefd4a8c0dbeb7864ce6da637c4df932694d4b6fff80cab5bb5b4319
ms.sourcegitcommit: b5f7da89a650d2915dc652449623c78be6247175
ms.translationtype: MT
ms.contentlocale: id-ID
ms.lasthandoff: 08/05/2021
ms.locfileid: "54114175"
---
# <a name="microsoft-edge-configure-privacy-settings"></a>Microsoft Edge mengonfigurasi pengaturan privasi

Secara default, Microsoft Edge disebarkan di platform non-Windows, data diagnostik, dan informasi situs tidak dikirim ke Microsoft. Namun, Microsoft Edge informasi situs dikirim Windows 10, data diagnostik dan informasi situs dikirim sesuai dengan pengaturan [data Windows pengguna.](https://docs.microsoft.com/windows/privacy/configure-windows-diagnostic-data-in-your-organization)

Untuk mengonfigurasi Microsoft Edge mana yang menangani pengumpulan data untuk organisasi Anda, gunakan kebijakan grup berikut ini:
- [MetricsReportingEnabled](https://docs.microsoft.com/DeployEdge/microsoft-edge-policies#metricsreportingenabled): Kebijakan ini memungkinkan pelaporan penggunaan dan data terkait crash.
- [SendSiteInfoToImproveServices](https://docs.microsoft.com/DeployEdge/microsoft-edge-policies#sendsiteinfotoimproveservices): Kebijakan ini mengirim informasi situs yang digunakan untuk menyempurnakan layanan Microsoft.

Untuk mempelajari selengkapnya, lihat [Mengonfigurasi pengaturan kebijakan](https://docs.microsoft.com/deployedge/microsoft-edge-enterprise-privacy-settings#configure-policy-settings).