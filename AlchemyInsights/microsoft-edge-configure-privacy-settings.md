---
title: Mengonfigurasi pengaturan privasi Microsoft Edge
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
ms.openlocfilehash: dcd1d91dcde1f585caf0e1e3af30946513a0f26c
ms.sourcegitcommit: 94036315916fbc79dca2a692c2e9bc1139dd28f6
ms.translationtype: MT
ms.contentlocale: id-ID
ms.lasthandoff: 12/08/2020
ms.locfileid: "49677794"
---
# <a name="microsoft-edge-configure-privacy-settings"></a>Mengonfigurasi pengaturan privasi Microsoft Edge

Secara default, jika Microsoft Edge disebarkan di platform non-Windows, data diagnostik dan informasi situs tidak dikirim ke Microsoft. Namun, jika Microsoft Edge disebarkan di Windows 10, data diagnostik dan informasi situs dikirim sesuai dengan [pengaturan data diagnostik Windows](https://docs.microsoft.com/windows/privacy/configure-windows-diagnostic-data-in-your-organization)pengguna.

Untuk mengonfigurasi cara Microsoft Edge menangani kumpulan data untuk organisasi Anda, gunakan kebijakan grup berikut ini:
- [Metricsreportingenabled](https://docs.microsoft.com/DeployEdge/microsoft-edge-policies#metricsreportingenabled): kebijakan ini memungkinkan pelaporan data terkait penggunaan dan crash.
- [Sendsiteinfotoimproveservices](https://docs.microsoft.com/DeployEdge/microsoft-edge-policies#sendsiteinfotoimproveservices): kebijakan ini mengirimkan informasi situs yang digunakan untuk menyempurnakan layanan Microsoft.

Untuk mempelajari selengkapnya, lihat [mengonfigurasi pengaturan kebijakan](https://docs.microsoft.com/deployedge/microsoft-edge-enterprise-privacy-settings#configure-policy-settings).