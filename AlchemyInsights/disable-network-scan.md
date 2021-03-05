---
title: Menonaktifkan pemindaian jaringan
ms.author: v-smandalika
author: v-smandalika
manager: dansimp
ms.date: 02/25/2021
audience: Admin
ms.topic: article
ms.service: o365-administration
ROBOTS: NOINDEX, NOFOLLOW
localization_priority: Normal
ms.collection: Adm_O365
ms.custom:
- "9001464"
- "3492"
ms.openlocfilehash: 7b0f5c21a7e6afda0ee3000e75ee725cbadcedb7
ms.sourcegitcommit: 6741a997fff871d263f92d3ff7fb61e7755956a9
ms.translationtype: MT
ms.contentlocale: id-ID
ms.lasthandoff: 03/04/2021
ms.locfileid: "50481968"
---
# <a name="disable-network-scan"></a>Menonaktifkan pemindaian jaringan

Pemindaian berbagi jaringan dapat berdampak pada kinerja.  Untuk memastikan klien tidak memindai berbagi jaringan/file secara default, konfigurasikan pengaturan berikut dalam aplikasi Windows Defender ke **True**:

- DisableScanningMappedNetworkDrivesForFullScan
- DisableScanningNetworkFiles