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
ms.openlocfilehash: 8dac2bdc20905cf37fc30317d9b371bfd755f452
ms.sourcegitcommit: 8bc60ec34bc1e40685e3976576e04a2623f63a7c
ms.translationtype: MT
ms.contentlocale: id-ID
ms.lasthandoff: 04/15/2021
ms.locfileid: "51826094"
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

