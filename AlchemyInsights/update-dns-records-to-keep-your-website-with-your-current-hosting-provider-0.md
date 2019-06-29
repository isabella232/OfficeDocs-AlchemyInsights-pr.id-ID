---
title: Pembaruan data DNS untuk menjaga website Anda dengan penyedia hosting Anda saat ini
ms.author: pebaum
author: pebaum
manager: mnirkhe
ms.date: 5/2/2018
ms.audience: Admin
ms.topic: article
ROBOTS: NOINDEX, NOFOLLOW
localization_priority: Normal
ms.collection: Adm_O365
ms.custom:
- "42"
- "43"
- "100002"
ms.assetid: 48251355-7383-4fdc-a1e1-9dc2c85a8d29
ms.openlocfilehash: 62f49038cf541c2185ed6a60c6cb58fe2889342d
ms.sourcegitcommit: 5fb7a4b28859690020efdea630d03e70cc0e6334
ms.translationtype: MT
ms.contentlocale: id-ID
ms.lasthandoff: 06/28/2019
ms.locfileid: "35353180"
---
# <a name="update-dns-records-to-keep-your-website-with-your-current-hosting-provider"></a>Pembaruan data DNS untuk menjaga website Anda dengan penyedia hosting Anda saat ini

1. Pada halaman [domain](https://portal.office.com/adminportal/home#/Domains) , dalam daftar domain, pilih domain yang Anda gunakan untuk website Anda, dan kemudian pilih **pengaturan DNS** di panel manajemen.

2. Pilih **+ catatan kustom baru** dan masukkan yang berikut:

  - Untuk **jenis DNS** masukkan: **(alamat)**

  - Untuk **nama Host atau Alias**, ketik berikut ini:**@**

  - Untuk **Alamat IP**, ketik alamat IP statis untuk situs web tempat itu saat ini host (misalnya, 172.16.140.1).

    Ini harus menjadi alamat IP *statis* untuk website, bukan alamat IP *dinamis* . Periksa dengan situs mana situs web adalah host untuk memastikan Anda bisa mendapatkan alamat IP statis untuk situs umum.

3. Pilih **Simpan**.

Selain itu, Anda dapat membuat CNAME untuk membantu pelanggan menemukan situs web Anda.
  
1. Pilih **+ catatan kustom baru** dan masukkan yang berikut:

  - Untuk **jenis DNS** masukkan: **CNAME (Alias)**

  - Untuk **nama Host atau Alias**, ketik berikut: **www**

  - Untuk **poin ke alamat**, ketik nama domain sepenuhnya memenuhi syarat (FQDN) untuk situs web Anda (misalnya, contoso.com).

2. Pilih **Simpan**.
