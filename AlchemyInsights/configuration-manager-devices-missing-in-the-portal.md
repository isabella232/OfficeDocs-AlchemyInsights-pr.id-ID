---
title: Perangkat Pengelola Konfigurasi hilang di portal
ms.author: pebaum
author: pebaum
manager: mnirkhe
ms.audience: Admin
ms.topic: article
ROBOTS: NOINDEX, NOFOLLOW
localization_priority: Priority
ms.collection: Adm_O365
ms.custom:
- "9001495"
- "4384"
ms.openlocfilehash: 7a11ad3c6970be2c52a7cf0696bd3810b9bd665a
ms.sourcegitcommit: 89ae9e8b36d1980f89f07b016fff0ec48f96b620
ms.translationtype: HT
ms.contentlocale: id-ID
ms.lasthandoff: 04/23/2020
ms.locfileid: "43789905"
---
# <a name="configuration-manager-devices-missing-in-the-portal"></a>Perangkat Pengelola Konfigurasi hilang di portal

Agar sinkronisasi perangkat bekerja, [titik akhir internet yang diperlukan](https://docs.microsoft.com/configmgr/tenant-attach/device-sync-actions#internet-endpoints) harus dapat dijangkau dari server lokal yang menghosting peran Titik Koneksi Layanan. Untuk memecahkan masalah sinkronisasi perangkat, tinjau **CMGatewaySyncUploadWorker.log** yang terletak di titik koneksi layanan.

Pelajari selengkapnya tentang [Penambahan penyewa pada Microsoft Endpoint Manager](https://docs.microsoft.com/configmgr/tenant-attach/).
