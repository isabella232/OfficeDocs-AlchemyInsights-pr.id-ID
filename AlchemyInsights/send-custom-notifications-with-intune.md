---
title: Kirim pemberitahuan kustom dengan Intune
ms.author: brenduns
author: brenduns
manager: dougeby
ms.audience: Admin
ms.topic: article
ROBOTS: NOINDEX, NOFOLLOW
localization_priority: Normal
ms.collection: Adm_O365
ms.custom:
- "9000679"
- "2565"
ms.openlocfilehash: 969649084a2ac536ee1b41f225c3be5415a27c4b
ms.sourcegitcommit: 2572c4e5a981d5f3f556835061c568cfd08b78da
ms.translationtype: MT
ms.contentlocale: id-ID
ms.lasthandoff: 12/27/2019
ms.locfileid: "40886860"
---
# <a name="how-to-send-custom-notifications-to-the-users-of-managed-ios-and-android-devices"></a>Cara mengirim pemberitahuan kustom ke pengguna perangkat iOS dan Android yang dikelola

Pemberitahuan kustom untuk Intune diproses oleh aplikasi portal perusahaan di perangkat pengguna. Aplikasi ini kemudian membuat pemberitahuan push pada perangkat tersebut.

Berikut adalah prasyarat perangkat untuk mendukung penerimaan pemberitahuan kustom, dan untuk aplikasi kemudian membuat pemberitahuan push:

- Perangkat harus memiliki aplikasi portal perusahaan yang diinstal.  

- Perangkat harus mengizinkan aplikasi portal perusahaan untuk mengirim pemberitahuan push. Ketika aplikasi diinstal atau diperbarui, itu akan meminta pengguna untuk mengizinkan pemberitahuan.

- Perangkat Android harus memiliki layanan Google Play terinstal.

- Perangkat harus terdaftar dengan Intune.

Untuk informasi selengkapnya, termasuk cara mengirim pesan, lihat [dokumentasi fitur](https://docs.microsoft.com/intune/custom-notifications).
