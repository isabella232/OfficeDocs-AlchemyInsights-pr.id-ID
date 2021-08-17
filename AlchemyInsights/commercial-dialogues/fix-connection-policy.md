---
title: Perbaiki kebijakan koneksi
ms.author: v-jmathew
author: v-jmathew
manager: dansimp
audience: Admin
ms.topic: article
ms.service: o365-administration
ROBOTS: NOINDEX, NOFOLLOW
localization_priority: Normal
ms.collection: Adm_O365
ms.custom:
- "9000760"
- "7391"
ms.openlocfilehash: 9094dcdc4507f52da1dd7c95f83aa98bab1446639d2d9f52eb3a7bc849dc183c
ms.sourcegitcommit: 920051182781bd97ce4d4d6fbd268cb37b84d239
ms.translationtype: MT
ms.contentlocale: id-ID
ms.lasthandoff: 08/11/2021
ms.locfileid: "57888409"
---
# <a name="fix-connection-policy"></a>Perbaiki kebijakan koneksi

Email ditandai aman dan dikirimkan ke Kotak Masuk pengguna karena alamat IP sumber ditandai sebagai aman dalam kebijakan filter koneksi default. Untuk meninjau kebijakan, lakukan langkah-langkah berikut ini:

1. Dalam portal Pertahanan Microsoft 365 di , masuk ke Email & Kebijakan Kolaborasi <https://security.microsoft.com/>  \> **& aturan** kebijakan \>  \> **Ancaman Anti spam** di **bagian** Kebijakan.

   Untuk langsung masuk ke **halaman Kebijakan anti spam,** gunakan <https://security.microsoft.com/antispam> .

2. Di **halaman Kebijakan anti spam,** pilih kebijakan bernama **Kebijakan filter koneksi (Default)** dengan mengklik nama kebijakan.

3. Di flyout detail yang muncul, klik **Edit kebijakan filter koneksi** di bagian **Pemfilteran** koneksi.

4. Tinjau entri di **bagian Selalu perbolehkan pesan** dari alamat IP atau rentang alamat berikut ini, dan lihat apakah Aktifkan daftar **aman** dipilih.

   > [!NOTE]
   > Microsoft berlangganan ke sumber pihak ketiga dari pengirim tepercaya. Jika daftar aman diaktifkan, pengirim tepercaya ini tidak ditandai sebagai spam secara tidak sengaja. Kami merekomendasikan untuk memilih opsi ini, karena akan mengurangi jumlah positif palsu (email baik yang diklasifikasikan sebagai spam) yang Anda terima.

Untuk informasi selengkapnya, lihat [Mengonfigurasi pemfilteran koneksi](https://docs.microsoft.com/microsoft-365/security/office-365-security/configure-the-connection-filter-policy).
