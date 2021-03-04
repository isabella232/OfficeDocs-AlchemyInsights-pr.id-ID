---
title: Kesalahan sinkronisasi pendaftaran perangkat otomatis Apple
ms.author: v-jmathew
author: v-jmathew
manager: scotv
audience: Admin
ms.topic: article
ms.service: o365-administration
ROBOTS: NOINDEX, NOFOLLOW
localization_priority: Normal
ms.collection: Adm_O365
ms.custom:
- "9000654"
- "7256"
ms.openlocfilehash: 912c9e56b4c468fb333769f15bd7c212594dc11a
ms.sourcegitcommit: 6741a997fff871d263f92d3ff7fb61e7755956a9
ms.translationtype: MT
ms.contentlocale: id-ID
ms.lasthandoff: 03/04/2021
ms.locfileid: "50448925"
---
# <a name="apple-automatic-device-enrollment-sync-errors"></a>Kesalahan sinkronisasi pendaftaran perangkat otomatis Apple

"Kami telah mendeteksi bahwa Anda memiliki satu atau beberapa token ADE/DEP yang dalam kondisi kesalahan. Hingga status kesalahan teratasi untuk setiap Token yang terpengaruh, fungsi ADE tidak akan berfungsi seperti yang diharapkan. ".

Kesalahan ini mungkin terwujud dalam beberapa cara termasuk:

1. Perangkat mungkin tidak sinkron dari ABM/ASM ke Intune
2. Penetapan profil pendaftaran mungkin gagal
3. Perangkat mungkin tidak menyelesaikan pendaftaran ADE berhasil

Periksa kesalahan sinkronisasi yang dilaporkan dalam konsol Intune di bawah **perangkat > mendaftar perangkat > pendaftaran > token program pendaftaran**.

Salah satu penyebab kesalahan sinkronisasi paling umum adalah berakhirnya token saat ini. Dalam banyak kasus, pembaruan Token yang terpengaruh akan mengatasi masalah tersebut.

Jika satu atau beberapa token Anda telah kedaluwarsa, lihat dokumentasi berikut ini untuk membantu Anda memperbaruinya sesuai keperluan:

[Memperpanjang token pendaftaran perangkat otomatis](https://docs.microsoft.com/mem/intune/enrollment/device-enrollment-program-enroll-ios#renew-an-automated-device-enrollment-token)

Selain itu, Anda bisa melihat dokumentasi berikut ini untuk melihat potensi remediasi untuk kesalahan lain yang menyebabkan kegagalan sinkronisasi token:

[Kesalahan sinkronisasi ABM/ASM untuk iOS/iPadOS dan token pendaftaran perangkat otomatis macOS](https://docs.microsoft.com/mem/intune/enrollment/troubleshoot-ios-enrollment-errors#sync-token-errors-between-intune-and-ade-dep)







[Kesalahan sinkronisasi ABM/ASM untuk iOS/iPadOS dan token pendaftaran perangkat otomatis macOS](https://docs.microsoft.com/mem/intune/enrollment/troubleshoot-ios-enrollment-errors#resolutions-when-syncing-tokens-between-intune-and-abmasm-for-automated-device-enrollment)
