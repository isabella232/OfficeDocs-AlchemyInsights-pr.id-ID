---
title: Perbarui data DNS untuk menjaga situs web Anda dengan penyedia hosting Anda saat ini
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
ms.sourcegitcommit: bc7d6f4f3c9f7060d073f5130e1ec856e248d020
ms.translationtype: MT
ms.contentlocale: id-ID
ms.lasthandoff: 06/02/2020
ms.locfileid: "36665763"
---
# <a name="update-dns-records-to-keep-your-website-with-your-current-hosting-provider"></a>Perbarui data DNS untuk menjaga situs web Anda dengan penyedia hosting Anda saat ini

1. Di pusat admin Microsoft 365, pergi ke halaman **setup**  >  [domain](https://portal.office.com/adminportal/home#/Domains) , dan dalam daftar domain, pilih domain yang Anda gunakan untuk situs web Anda.

2. Pilih **+ rekaman kustom baru** dan masukkan yang berikut:

  - Untuk **tipe DNS** , masukkan: **A (alamat)**

  - Untuk **nama host atau alias**, ketik berikut ini:**@**

  - Untuk **Alamat IP**, KETIK alamat IP statis untuk situs web tempat saat ini dihosting (misalnya, 172.16.140.1).

    Ini harus alamat IP *statis* untuk situs web, bukan alamat IP *dinamis* . Periksa dengan situs di mana situs web Anda di-host untuk memastikan Anda bisa mendapatkan alamat IP statis untuk situs web publik Anda.

3. Pilih **Simpan**.

Selain itu, Anda dapat membuat data CNAME untuk membantu pelanggan menemukan situs web Anda.
  
1. Pilih **+ rekaman kustom baru** dan masukkan yang berikut:

  - Untuk **tipe DNS** , masukkan: **CNAME (alias)**

  - Untuk **nama host atau alias**, ketik berikut ini: **www**

  - Untuk **titik alamat**, ketik nama domain yang sepenuhnya memenuhi syarat (FQDN) untuk situs web Anda (misalnya, contoso.com).

2. Pilih **Simpan**.
