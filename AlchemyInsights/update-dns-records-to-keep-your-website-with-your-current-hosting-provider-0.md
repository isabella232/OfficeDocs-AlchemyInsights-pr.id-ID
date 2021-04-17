---
title: Memperbarui catatan DNS untuk mempertahankan situs web Anda dengan penyedia hosting Anda saat ini
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
- "42"
- "43"
- "100002"
ms.assetid: 48251355-7383-4fdc-a1e1-9dc2c85a8d29
ms.openlocfilehash: 89bce2aa5931c0c20706efabd42d2351be43938b
ms.sourcegitcommit: 8bc60ec34bc1e40685e3976576e04a2623f63a7c
ms.translationtype: MT
ms.contentlocale: id-ID
ms.lasthandoff: 04/15/2021
ms.locfileid: "51827524"
---
# <a name="update-dns-records-to-keep-your-website-with-your-current-hosting-provider"></a>Memperbarui catatan DNS untuk mempertahankan situs web Anda dengan penyedia hosting Anda saat ini

1. Di pusat admin Microsoft 365, masuk ke halaman **Penyiapan** Domain, lalu dalam daftar domain, pilih domain yang digunakan untuk  >  [](https://admin.microsoft.com/Adminportal#/Domains) situs web Anda.

2. Pilih **+ Catatan kustom baru,** lalu masukkan hal berikut:

  - Untuk **tipe DNS,** masukkan: **A (Alamat)**

  - Untuk **Nama host atau Alias,** ketikkan: **@**

  - Untuk **Alamat IP,** ketikkan alamat IP statis tempat situs web dihosting saat ini (misalnya, 172.16.140.1).

    Ini harus merupakan  *alamat*  IP statis untuk situs web, bukan  *alamat*  IP dinamis. Periksa situs tempat situs web Anda dihosting untuk memastikan Anda bisa mendapatkan alamat IP statis untuk situs web publik.

3. Pilih **Simpan.**

Selain itu, Anda bisa membuat catatan CNAME untuk membantu pelanggan menemukan situs web Anda.
  
1. Pilih **+ Catatan kustom baru,** lalu masukkan hal berikut:

  - Untuk **Tipe DNS,** masukkan: **CNAME (Alias)**

  - Untuk **Nama host atau Alias,** ketikkan: **www**

  - Untuk **Alamat tujuan,** ketikkan FQDN (nama domain yang sepenuhnya memenuhi syarat) untuk situs web Anda (misalnya, contoso.com).

2. Pilih **Simpan.**
