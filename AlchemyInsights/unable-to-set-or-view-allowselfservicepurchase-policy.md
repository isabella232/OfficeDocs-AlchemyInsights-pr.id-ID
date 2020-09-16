---
title: Tidak dapat mengatur atau menampilkan kebijakan AllowSelfServicePurchase
ms.author: pebaum
author: pebaum
manager: mnirkhe
ms.audience: Admin
ms.topic: article
ms.service: o365-administration
ROBOTS: NOINDEX, NOFOLLOW
localization_priority: Normal
ms.collection: Adm_O365
ms.custom:
- "9001212"
- "3526"
ms.openlocfilehash: 5ec16b3071f95ef52af2771e95137116222a3c5b
ms.sourcegitcommit: c6692ce0fa1358ec3529e59ca0ecdfdea4cdc759
ms.translationtype: MT
ms.contentlocale: id-ID
ms.lasthandoff: 09/14/2020
ms.locfileid: "47735202"
---
# <a name="unable-to-set-or-view-the-allowselfservicepurchase-policy"></a>Tidak dapat mengatur atau menampilkan kebijakan AllowSelfServicePurchase

Saat mencoba mengatur atau menampilkan kebijakan AllowSelfServicePurchase, Anda menerima pesan kesalahan berikut:

*Saperkesalahan: gagal untuk mengambil kebijakan produk dengan PolicyId ' AllowSelfServicePurchase ', ErrorMessage-The underlying Connection ditutup: kesalahan yang tidak diharapkan terjadi pada kirim.*

Ini mungkin karena versi lama Transport Layer Security (TLS). Untuk menyambungkan Layanan MSCommerce, Anda harus menggunakan TLS 1,2 atau yang lebih baru.  

Cobalah langkah-langkah berikut untuk mengaktifkan/mengatur protokol TLS ke 1,2, memverifikasi, dan coba lagi.
 1. Pada prompt perintah PowerShell (PS C: \) Masukkan perintah berikut ini untuk mengatur protokol TLS ke versi 1,2:

    `[Net.ServicePointManager]::SecurityProtocol = [Net.SecurityProtocolType]::Tls12`

2. Verifikasi protokol TLS yang digunakan, dengan perintah berikut ini:

    `[Net.ServicePointManager]::SecurityProtocol` 

3. Coba lagi perintah Dapatkan atau Perbarui sesuai keperluan.

