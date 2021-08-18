---
title: Mengirim pemberitahuan kustom dengan Intune
ms.author: brenduns
author: brenduns
manager: dougeby
ms.audience: Admin
ms.topic: article
ms.service: o365-administration
ROBOTS: NOINDEX, NOFOLLOW
localization_priority: Normal
ms.collection: Adm_O365
ms.custom:
- "9000679"
- "2565"
ms.openlocfilehash: 58acaa29f9d0b066cc7be6f6ee57b1806d0e8812b194e20166b133b7715226a8
ms.sourcegitcommit: b5f7da89a650d2915dc652449623c78be6247175
ms.translationtype: MT
ms.contentlocale: id-ID
ms.lasthandoff: 08/05/2021
ms.locfileid: "54086167"
---
# <a name="how-to-send-custom-notifications-to-the-users-of-managed-ios-and-android-devices"></a>Cara mengirim pemberitahuan kustom kepada pengguna di perangkat iOS dan Android yang dikelola

Pemberitahuan kustom untuk Intune diproses oleh Company Portal kustom pada perangkat pengguna. Aplikasi lalu membuat pemberitahuan push di perangkat itu.

Berikut ini adalah prasyarat perangkat untuk mendukung tanda terima pemberitahuan kustom, dan untuk aplikasi lalu membuat pemberitahuan push:

- Perangkat harus memiliki Company Portal terinstal.  

- Perangkat harus memperbolehkan aplikasi Company Portal mengirim pemberitahuan push. Saat aplikasi diinstal atau diperbarui, aplikasi akan meminta pengguna untuk mengizinkan pemberitahuan.

- Perangkat Android harus menginstal Layanan Google Play.

- Perangkat harus terdaftar dengan Intune.

Untuk informasi selengkapnya termasuk cara mengirim pesan, lihat [dokumentasi fitur](https://docs.microsoft.com/intune/custom-notifications).
