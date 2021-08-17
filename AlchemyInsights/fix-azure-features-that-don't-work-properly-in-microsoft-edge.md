---
title: Apa yang harus dilakukan jika fitur Azure tidak berfungsi dengan baik Microsoft Edge
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
ms.openlocfilehash: e188ecb375f3d84b45a1a7718b3c0b797c756f822ba64b3824976fe79c1e8298
ms.sourcegitcommit: b5f7da89a650d2915dc652449623c78be6247175
ms.translationtype: MT
ms.contentlocale: id-ID
ms.lasthandoff: 08/05/2021
ms.locfileid: "54117091"
---
# <a name="what-to-do-if-azure-features-dont-work-properly-in-microsoft-edge"></a>Apa yang harus dilakukan jika fitur Azure tidak berfungsi dengan baik Microsoft Edge

Microsoft Edge memiliki [masalah umum](https://go.microsoft.com/fwlink/?linkid=2140608) yang terkait dengan zona keamanan dan mungkin memengaruhi cara pengguna Azure masuk ke Windows Admin Azure. Jika mengalami masalah dalam menggunakan fitur Azure dengan dukungan Microsoft Edge, cobalah langkah-langkah berikut:

1. Di menu **Mulai,** cari Opsi **Internet,** lalu pilih.
2. Dalam kotak dialog Properti **Internet,** masuk ke **tab** Keamanan.
3. Pilih zona **Situs** tepercaya, lalu pilih **tombol** Situs.
4. Dalam **kotak** dialog Situs tepercaya, tambahkan URL gateway serta [https://login.microsoftonline.com](https://login.microsoftonline.com) , lalu pilih [https://login.live.com](https://login.live.com) **Tutup**.
5. Dalam kotak dialog Properti **Internet,** masuk ke **tab** Privasi.
6. Di bagian **Pemblokir Pop-up,** pilih **Pengaturan**. Dalam kotak dialog yang terbuka, tambahkan URL gateway serta [https://login.microsoftonline.com](https://login.microsoftonline.com) , lalu pilih [https://login.live.com](https://login.live.com) **Tutup**.
