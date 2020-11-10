---
title: Kesalahan masuk OneDrive AADSTS50011
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
- "9003820"
- "6840"
ms.openlocfilehash: 1f906f82e99c322ed953800d54fba5a073eacd10
ms.sourcegitcommit: 534e9217d99336eb471166ff83231c7e408fb1d9
ms.translationtype: MT
ms.contentlocale: id-ID
ms.lasthandoff: 11/09/2020
ms.locfileid: "48982481"
---
# <a name="onedrive-login-error-aadsts50011"></a>Kesalahan masuk OneDrive AADSTS50011

Jika Anda menerima kesalahan "AADSTS50011: URL balasan yang ditentukan dalam permintaan tidak cocok dengan Balasan" saat masuk ke aplikasi OneDrive, periksa hal berikut:

Versi OneDrive Anda harus sama dengan atau lebih besar dari versi 20.052. XXXX. XXXX. Untuk memeriksa versi Anda, klik ikon OneDrive biru di area pemberitahuan, pilih **bantuan & pengaturan > pengaturan > tentang**.

Jaringan Anda mungkin memblokir Traffic ke **g.Live.com** dan **oneclient.SFX.ms**. Jika lalu lintas diblokir, OneDrive tidak dapat memperbarui dirinya. Bekerja dengan administrator jaringan Anda untuk memastikan Anda memiliki akses ke URL tersebut. [Titik akhir ini](https://docs.microsoft.com/microsoft-365/enterprise/urls-and-ip-address-ranges?view=o365-worldwide) harus dapat dijangkau untuk pelanggan yang menggunakan paket Microsoft 365.

Jika Anda perlu mendapatkan versi terbaru OneDrive, kunjungi [https://aka.ms/getonedrive](https://aka.ms/getonedrive) .
