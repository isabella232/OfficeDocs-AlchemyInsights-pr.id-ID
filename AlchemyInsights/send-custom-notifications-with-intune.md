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
ms.openlocfilehash: 2e5e2e2f24c46d3db4f08862dcc80934937f6f51
ms.sourcegitcommit: c6692ce0fa1358ec3529e59ca0ecdfdea4cdc759
ms.translationtype: MT
ms.contentlocale: id-ID
ms.lasthandoff: 09/14/2020
ms.locfileid: "47720649"
---
# <a name="how-to-send-custom-notifications-to-the-users-of-managed-ios-and-android-devices"></a>Cara mengirim pemberitahuan kustom kepada pengguna perangkat iOS dan Android yang dikelola

Pemberitahuan kustom untuk Intune diproses oleh aplikasi portal perusahaan di perangkat pengguna. Aplikasi tersebut membuat pemberitahuan push pada perangkat tersebut.

Berikut ini adalah prasyarat perangkat untuk mendukung penerimaan pemberitahuan kustom, dan untuk aplikasi untuk membuat pemberitahuan push:

- Perangkat harus menginstal aplikasi portal perusahaan.  

- Perangkat harus memperbolehkan aplikasi portal perusahaan mengirimkan pemberitahuan push. Saat aplikasi terinstal atau diperbarui, aplikasi akan meminta pengguna untuk memperbolehkan pemberitahuan.

- Perangkat Android harus menginstal Google Play Services.

- Perangkat harus didaftarkan dengan Intune.

Untuk informasi selengkapnya, termasuk cara mengirim pesan, lihat [dokumentasi fitur](https://docs.microsoft.com/intune/custom-notifications).
