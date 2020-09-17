---
title: Memperbarui catatan DNS untuk mempertahankan situs web Anda dengan penyedia hosting Anda saat ini
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
- "42"
- "43"
- "100002"
ms.assetid: 48251355-7383-4fdc-a1e1-9dc2c85a8d29
ms.openlocfilehash: 1d8654bc2dfb9063d0203992d624285eb646027d
ms.sourcegitcommit: 78939b01579b626b147d356045a37aec1170c948
ms.translationtype: MT
ms.contentlocale: id-ID
ms.lasthandoff: 09/15/2020
ms.locfileid: "47815788"
---
# <a name="update-dns-records-to-keep-your-website-with-your-current-hosting-provider"></a>Memperbarui catatan DNS untuk mempertahankan situs web Anda dengan penyedia hosting Anda saat ini

1. Di pusat admin Microsoft 365, masuk ke halaman domain **penyetelan**  >  [Domains](https://admin.microsoft.com/Adminportal#/Domains) , dan di daftar domain, pilih domain yang Anda gunakan untuk situs web Anda.

2. Pilih **+ catatan kustom baru** , lalu masukkan yang berikut ini:

  - Untuk **tipe DNS** , masukkan: **A (address)**

  - Untuk **nama host atau alias**, ketikkan yang berikut ini: **@**

  - Untuk **Alamat IP**, KETIKKAN alamat IP statis untuk situs web Anda saat ini dihosting (misalnya, 172.16.140.1).

    Ini harus berupa alamat IP  *statis*  untuk situs web, bukan alamat IP  *dinamis*  . Periksa situs tempat situs web Anda dihosting untuk memastikan Anda bisa mendapatkan alamat IP statis untuk situs web publik Anda.

3. Pilih **Simpan**.

Selain itu, Anda bisa membuat catatan CNAME untuk membantu pelanggan menemukan situs web Anda.
  
1. Pilih **+ catatan kustom baru** , lalu masukkan yang berikut ini:

  - Untuk **tipe DNS** masukkan: **CNAME (alias)**

  - Untuk **nama host atau alias**, ketikkan yang berikut: **www**

  - Untuk **Alamat**target, ketikkan nama domain yang sepenuhnya memenuhi syarat (FQDN) untuk situs web Anda (misalnya, contoso.com).

2. Pilih **Simpan**.
