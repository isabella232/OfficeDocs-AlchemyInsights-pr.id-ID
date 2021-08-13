---
title: Perangkat Pengelola Konfigurasi hilang di portal
ms.author: pebaum
author: pebaum
manager: scotv
ms.audience: Admin
ms.topic: article
ms.service: o365-administration
ROBOTS: NOINDEX, NOFOLLOW
localization_priority: Priority
ms.collection: Adm_O365
ms.custom:
- "9001495"
- "4384"
ms.openlocfilehash: 358bb6aa0420a845e51e0b75049c2ae790daf3690e5cfb115b234d82a29e93a7
ms.sourcegitcommit: b5f7da89a650d2915dc652449623c78be6247175
ms.translationtype: MT
ms.contentlocale: id-ID
ms.lasthandoff: 08/05/2021
ms.locfileid: "53966112"
---
# <a name="configuration-manager-devices-missing-in-the-portal"></a>Perangkat Pengelola Konfigurasi hilang di portal

Agar sinkronisasi perangkat bekerja, [titik akhir internet yang diperlukan](https://docs.microsoft.com/configmgr/tenant-attach/device-sync-actions#internet-endpoints) harus dapat dijangkau dari server lokal yang menghosting peran Titik Koneksi Layanan. Untuk memecahkan masalah sinkronisasi perangkat, tinjau **CMGatewaySyncUploadWorker.log** yang terletak di titik koneksi layanan.

Pelajari selengkapnya tentang [Penambahan penyewa pada Microsoft Endpoint Manager](https://docs.microsoft.com/configmgr/tenant-attach/).
