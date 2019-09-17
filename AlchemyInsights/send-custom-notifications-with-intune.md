---
title: Kirim pemberitahuan kustom dengan Intune
ms.author: brenduns
author: brenduns
manager: dougeby
ms.date: 07/31/2019
ms.audience: Admin
ms.topic: article
ROBOTS: NOINDEX, NOFOLLOW
localization_priority: Normal
ms.collection: Adm_O365
ms.custom: 9000679
ms.openlocfilehash: 1244f07fd56cf603280f1710520a04d579224e44
ms.sourcegitcommit: 16f08d051afca3c6d0de32826324f91cf63ab5ba
ms.translationtype: MT
ms.contentlocale: id-ID
ms.lasthandoff: 09/16/2019
ms.locfileid: "36992316"
---
# <a name="how-to-send-custom-notifications-to-the-users-of-managed-ios-and-android-devices"></a>Cara mengirim pemberitahuan kustom ke pengguna perangkat iOS dan Android yang dikelola

Pemberitahuan kustom untuk Intune diproses oleh aplikasi portal perusahaan di perangkat pengguna. Aplikasi ini kemudian membuat pemberitahuan push pada perangkat tersebut.

Berikut adalah prasyarat perangkat untuk mendukung penerimaan pemberitahuan kustom, dan untuk aplikasi kemudian membuat pemberitahuan push:

- Perangkat harus memiliki aplikasi portal perusahaan yang diinstal.  

- Perangkat harus mengizinkan aplikasi portal perusahaan untuk mengirim pemberitahuan push. Ketika aplikasi diinstal atau diperbarui, itu akan meminta pengguna untuk mengizinkan pemberitahuan.

- Perangkat Android harus memiliki layanan Google Play terinstal.

- Perangkat harus terdaftar dengan Intune.

Untuk informasi selengkapnya, termasuk cara mengirim pesan, lihat [dokumentasi fitur](https://docs.microsoft.com/intune/custom-notifications).
