---
title: Kesalahan sinkronisasi pendaftaran perangkat otomatis Apple
ms.author: v-jmathew
author: v-jmathew
manager: scotv
ms.audience: Admin
ms.topic: article
ms.service: o365-administration
ROBOTS: NOINDEX, NOFOLLOW
localization_priority: Normal
ms.collection: Adm_O365
ms.custom:
- "9000654"
- "7256"
ms.openlocfilehash: d7a9398046a1073e30fdbe2950f750bb55d4fa2f
ms.sourcegitcommit: 87c8d0a1e6668211b9dd5427f98984ccdcadb02d
ms.translationtype: MT
ms.contentlocale: id-ID
ms.lasthandoff: 12/17/2020
ms.locfileid: "49714832"
---
# <a name="apple-automatic-device-enrollment-sync-errors"></a>Kesalahan sinkronisasi pendaftaran perangkat otomatis Apple

"Kami telah mendeteksi bahwa Anda memiliki satu atau beberapa token ADE/DEP yang dalam kondisi kesalahan. Hingga status kesalahan teratasi untuk setiap Token yang terpengaruh, fungsi ADE tidak akan berfungsi sama ".

Kesalahan ini mungkin terwujud dalam beberapa cara termasuk:

1. Perangkat mungkin tidak sinkron dari ABM/ASM ke Intune
2. Penetapan profil pendaftaran mungkin gagal
3. Perangkat mungkin tidak menyelesaikan pendaftaran ADE berhasil

Periksa kesalahan sinkronisasi yang dilaporkan dalam konsol Intune di bawah **perangkat > mendaftar perangkat > pendaftaran Apple > token program pendaftaran** dan Tinjau dokumentasi berikut ini untuk melihat potensi remediasi:

[Kesalahan sinkronisasi ABM/ASM untuk iOS/iPadOS dan token pendaftaran perangkat otomatis macOS](https://docs.microsoft.com/mem/intune/enrollment/troubleshoot-ios-enrollment-errors#resolutions-when-syncing-tokens-between-intune-and-abmasm-for-automated-device-enrollment)
