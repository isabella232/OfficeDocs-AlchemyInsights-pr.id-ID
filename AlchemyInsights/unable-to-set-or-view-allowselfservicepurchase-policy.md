---
title: Tidak dapat menetapkan atau melihat kebijakan AllowSelfServicePurchase
ms.author: pebaum
author: pebaum
manager: mnirkhe
ms.audience: Admin
ms.topic: article
ROBOTS: NOINDEX, NOFOLLOW
localization_priority: Normal
ms.collection: Adm_O365
ms.custom:
- "9001212"
- "3526"
ms.openlocfilehash: 587a05cccbc71a970d4bd7723bff0df0c3b64ccc
ms.sourcegitcommit: 2a9d059262c07c33f9a740b3da4e6e3366b2f925
ms.translationtype: MT
ms.contentlocale: id-ID
ms.lasthandoff: 02/20/2020
ms.locfileid: "42158564"
---
# <a name="unable-to-set-or-view-the-allowselfservicepurchase-policy"></a>Tidak dapat menetapkan atau melihat kebijakan AllowSelfServicePurchase

Ketika mencoba untuk menetapkan atau melihat kebijakan AllowSelfServicePurchase, Anda menerima pesan galat berikut:

*HandleError: gagal untuk mengambil kebijakan produk dengan PolicyId ' AllowSelfServicePurchase ', ErrorMessage-yang mendasari sambungan ditutup: galat tak terduga terjadi pada kirim.*

Hal ini mungkin karena versi lama Transport Layer Security (TLS). Untuk menyambungkan Layanan MSCommerce, Anda harus menggunakan TLS 1,2 atau yang lebih baru.  

Cobalah langkah berikut untuk mengaktifkan/menetapkan protokol TLS ke 1,2, verifikasi, dan coba lagi.
 1. Pada PowerShell prompt perintah (PS C:\) masukkan perintah berikut ini untuk menetapkan protokol TLS ke versi 1,2:

    `[Net.ServicePointManager]::SecurityProtocol = [Net.SecurityProtocolType]::Tls12`

2. Verifikasi protokol TLS yang digunakan, dengan perintah berikut:

    `[Net.ServicePointManager]::SecurityProtocol` 

3. Coba lagi perintah Get atau update sesuai kebutuhan.

