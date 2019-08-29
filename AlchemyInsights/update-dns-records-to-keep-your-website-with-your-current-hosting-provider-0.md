---
title: Pembaruan data DNS untuk menjaga website Anda dengan penyedia hosting Anda saat ini
ms.author: pebaum
author: pebaum
manager: mnirkhe
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
ms.openlocfilehash: 7bd36c3954d12d3ee4ac624a2f827d8e5cd88082
ms.sourcegitcommit: b3e55405af384e868fcd32ea794eb15d1356c3fc
ms.translationtype: MT
ms.contentlocale: id-ID
ms.lasthandoff: 08/29/2019
ms.locfileid: "36665763"
---
# <a name="update-dns-records-to-keep-your-website-with-your-current-hosting-provider"></a>Pembaruan data DNS untuk menjaga website Anda dengan penyedia hosting Anda saat ini

1. Di pusat admin Microsoft 365, pergi ke **pengaturan** > [domain](https://portal.office.com/adminportal/home#/Domains) halaman, dan dalam daftar domain, pilih domain yang Anda gunakan untuk website Anda.

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
