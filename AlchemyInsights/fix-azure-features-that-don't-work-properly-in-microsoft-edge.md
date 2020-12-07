---
title: Apa yang harus dilakukan jika fitur Azure tidak berfungsi dengan baik di Microsoft Edge
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
- "9004128"
- "7206"
ms.openlocfilehash: 463236bcd9ff480471604c992aa1ed1ed4ac2987
ms.sourcegitcommit: 2e4a5153e530bf15744a52e982eeb0d99757e9d2
ms.translationtype: MT
ms.contentlocale: id-ID
ms.lasthandoff: 12/04/2020
ms.locfileid: "49583459"
---
# <a name="what-to-do-if-azure-features-dont-work-properly-in-microsoft-edge"></a>Apa yang harus dilakukan jika fitur Azure tidak berfungsi dengan baik di Microsoft Edge

Microsoft Edge telah [mengetahui masalah](https://go.microsoft.com/fwlink/?linkid=2140608) yang terkait dengan zona keamanan dan mungkin mempengaruhi cara pengguna Azure masuk ke Pusat admin Windows. Jika Anda mengalami masalah dalam menggunakan fitur Azure dengan Microsoft Edge, cobalah langkah-langkah berikut:

1. Di menu **mulai** , Cari **Opsi Internet** dan pilih.
2. Dalam kotak dialog **properti Internet** , masuk ke tab **keamanan** .
3. Pilih zona **situs tepercaya** lalu pilih tombol **situs** .
4. Dalam kotak dialog **situs tepercaya** , Tambahkan URL Gateway Anda serta [https://login.microsoftonline.com](https://login.microsoftonline.com) , lalu [https://login.live.com](https://login.live.com) pilih **tutup**.
5. Dalam kotak dialog **properti Internet** , masuk ke tab **privasi** .
6. Di bagian **Pemblokir pop-up** , pilih **pengaturan**. Dalam kotak dialog yang terbuka, Tambahkan URL Gateway Anda serta [https://login.microsoftonline.com](https://login.microsoftonline.com) [https://login.live.com](https://login.live.com) , lalu pilih **tutup**.
