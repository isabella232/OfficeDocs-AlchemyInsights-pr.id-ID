---
title: Tidak dapat mengatur atau menampilkan kebijakan AllowSelfServicePurchase
ms.author: pebaum
author: pebaum
manager: scotv
ms.audience: Admin
ms.topic: article
ms.service: o365-administration
ROBOTS: NOINDEX, NOFOLLOW
localization_priority: Normal
ms.collection: Adm_O365
ms.custom:
- "9001212"
- "3526"
ms.openlocfilehash: 255dbe35b808b3fe6b5707779251bf3f4a7e1c269c8b6f0ac2cb43ca03c469e9
ms.sourcegitcommit: b5f7da89a650d2915dc652449623c78be6247175
ms.translationtype: MT
ms.contentlocale: id-ID
ms.lasthandoff: 08/05/2021
ms.locfileid: "54020195"
---
# <a name="unable-to-set-or-view-the-allowselfservicepurchase-policy"></a>Tidak dapat mengatur atau menampilkan kebijakan AllowSelfServicePurchase

Ketika mencoba mengatur atau menampilkan kebijakan AllowSelfServicePurchase, Anda menerima pesan kesalahan berikut:

*HandleError: Gagal mendapatkan kebijakan produk dengan PolicyId 'AllowSelfServicePurchase', ErrorMessage - Koneksi yang mendasari ditutup: Terjadi kesalahan yang tidak terduga pada pengiriman.*

Hal ini mungkin terjadi karena versi lama Transport Layer Security (TLS). Untuk menyambungkan layanan MSCommerce, Anda perlu menggunakan TLS 1.2 atau yang lebih besar.  

Coba langkah-langkah berikut untuk mengaktifkan/mengatur protokol TLS ke 1.2, verifikasi, dan coba lagi.
 1. Di prompt perintah PowerShell (PS C: \) masukkan perintah berikut ini untuk mengatur protokol TLS ke versi 1.2:

    `[Net.ServicePointManager]::SecurityProtocol = [Net.SecurityProtocolType]::Tls12`

2. Verifikasi protokol TLS yang digunakan, dengan perintah berikut ini:

    `[Net.ServicePointManager]::SecurityProtocol` 

3. Coba lagi perintah Dapatkan atau Perbarui sebagaimana diperlukan.

