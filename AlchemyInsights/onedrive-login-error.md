---
title: OneDrive masuk dengan AADSTS50011
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
ms.openlocfilehash: 80aafa2aee7213e1b77d274509a7eb9741c20b525ed97f473093ac8c6514f3c7
ms.sourcegitcommit: b5f7da89a650d2915dc652449623c78be6247175
ms.translationtype: MT
ms.contentlocale: id-ID
ms.lasthandoff: 08/05/2021
ms.locfileid: "54112915"
---
# <a name="onedrive-login-error-aadsts50011"></a>OneDrive masuk dengan AADSTS50011

Jika Anda menerima kesalahan "AADSTS50011: URL balasan yang ditentukan dalam permintaan tidak sesuai dengan balasan" ketika masuk ke aplikasi OneDrive, periksa hal berikut:

Versi OneDrive harus sama dengan atau lebih besar dari versi 20.052.XXXX.XXXX. Untuk memeriksa versi Anda, klik ikon OneDrive berwarna biru di area pemberitahuan, pilih **Bantuan & Pengaturan > Pengaturan > Tentang.**

Jaringan Anda mungkin memblokir lalu lintas **ke g.live.com** **dan oneclient.sfx.ms**. Jika lalu lintas diblokir, lalu lintas OneDrive tidak bisa memperbarui dirinya sendiri. Bekerja dengan administrator jaringan untuk memastikan Anda memiliki akses ke URL tersebut. [Titik akhir ini](https://docs.microsoft.com/microsoft-365/enterprise/urls-and-ip-address-ranges?view=o365-worldwide) harus dapat dijangkau oleh pelanggan Microsoft 365 baru.

Jika Anda perlu mendapatkan versi uji coba secara manual OneDrive, kunjungi [https://aka.ms/getonedrive](https://aka.ms/getonedrive) .
