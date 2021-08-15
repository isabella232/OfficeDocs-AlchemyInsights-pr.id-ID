---
title: Kesalahan sinkronisasi Pendaftaran Perangkat Otomatis Apple
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
ms.openlocfilehash: 1664a26b313c4a38c9c6d78cdb89997749ba175fd3dd72f278e99bbd50b0ee84
ms.sourcegitcommit: b5f7da89a650d2915dc652449623c78be6247175
ms.translationtype: MT
ms.contentlocale: id-ID
ms.lasthandoff: 08/05/2021
ms.locfileid: "54013751"
---
# <a name="apple-automatic-device-enrollment-sync-errors"></a>Kesalahan sinkronisasi Pendaftaran Perangkat Otomatis Apple

"Kami mendeteksi bahwa Anda memiliki satu atau beberapa Token ADE/DEP yang berada dalam status kesalahan. Hingga status kesalahan diatasi untuk setiap token yang terpengaruh, fungsionalitas ADE tidak akan berfungsi seperti yang diharapkan.".

Kesalahan ini dapat di manifes dalam sejumlah cara, termasuk:

1. Perangkat mungkin tidak tersinkron dari ABM/ASM ke Intune
2. Penetapan profil pendaftaran mungkin gagal
3. Perangkat mungkin tidak berhasil menyelesaikan pendaftaran ADE

Periksa kesalahan sinkronisasi yang dilaporkan di konsol Intune di bawah Perangkat > Perangkat > pendaftaran **Apple > Token program pendaftaran**.

Salah satu penyebab paling umum kesalahan sinkronisasi adalah masa kedaluwarsa token saat ini. Dalam banyak kasus, perpanjangan token yang terpengaruh akan mengatasi masalah ini.

Jika satu atau beberapa token Anda telah kedaluwarsa, lihat dokumentasi berikut untuk membantu Anda memperpanjangnya dengan benar:

[Perbarui token Pendaftaran Perangkat Otomatis](https://docs.microsoft.com/mem/intune/enrollment/device-enrollment-program-enroll-ios#renew-an-automated-device-enrollment-token)

Selain itu, Anda dapat melihat dokumentasi berikut untuk melihat kemungkinan perbaikan atas kesalahan lain yang menyebabkan kegagalan sinkronisasi token:

[Kesalahan Sinkronisasi ABM/ASM untuk Token Pendaftaran Perangkat Otomatis iOS/iPadOS dan macOS](https://docs.microsoft.com/mem/intune/enrollment/troubleshoot-ios-enrollment-errors#sync-token-errors-between-intune-and-ade-dep)







[Kesalahan Sinkronisasi ABM/ASM untuk Token Pendaftaran Perangkat Otomatis iOS/iPadOS dan macOS](https://docs.microsoft.com/mem/intune/enrollment/troubleshoot-ios-enrollment-errors#resolutions-when-syncing-tokens-between-intune-and-abmasm-for-automated-device-enrollment)
