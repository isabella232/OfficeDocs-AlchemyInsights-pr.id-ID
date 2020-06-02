---
title: Pengaturan DKIM
ms.author: chrisda
author: chrisda
manager: dansimp
ms.audience: ITPro
ms.topic: article
ROBOTS: NOINDEX, NOFOLLOW
localization_priority: Normal
ms.custom: 1388
ms.assetid: ''
ms.openlocfilehash: 0acaed476dbd06bc933bf466f9bf6116413a44bb
ms.sourcegitcommit: bc7d6f4f3c9f7060d073f5130e1ec856e248d020
ms.translationtype: MT
ms.contentlocale: id-ID
ms.lasthandoff: 06/02/2020
ms.locfileid: "44509387"
---
# <a name="setup-dkim"></a>Pengaturan DKIM

Petunjuk lengkap untuk mengonfigurasi DKIM untuk domain kustom di Microsoft 365 ada [di sini](https://docs.microsoft.com/microsoft-365/security/office-365-security/use-dkim-to-validate-outbound-email#steps-you-need-to-do-to-manually-set-up-dkim).

1. Untuk **setiap** domain kustom, Anda perlu membuat **dua** data CNAME DKIM di layanan hosting DNS domain (biasanya, registrar domain). Misalnya, contoso.com dan fourthcoffee.com memerlukan empat data CNAME DKIM: dua untuk contoso.com dan dua untuk fourthcoffee.com.

   Data CNAME DKIM untuk **setiap** domain kustom menggunakan format berikut:

   - **Nama host**:`selector1._domainkey.<CustomDomain>`

     **Poin ke alamat atau nilai**:`selector1-<DomainGUID>._domainkey.<InitialDomain>`

     **TTL**: 3600

   - **Nama host**:`selector2._domainkey.<CustomDomain>`

     **Poin ke alamat atau nilai**:`selector2-<DomainGUID>._domainkey.<InitialDomain>`

     **TTL**: 3600

   \<DomainGUID\>adalah teks di sebelah kiri `.mail.protection.outlook.com` dalam data MX yang disesuaikan untuk domain kustom (misalnya, `contoso-com` untuk domain contoso.com). \<InitialDomain\>adalah domain yang Anda gunakan saat mendaftar untuk Microsoft 365 (misalnya, contoso.onmicrosoft.com).

2. Setelah membuat data CNAME untuk domain kustom, selesaikan petunjuk berikut:

   J. [masuk ke Microsoft 365](https://support.office.microsoft.com/article/e9eb7d51-5430-4929-91ab-6157c5a050b4) dengan akun kantor atau sekolah.

   B. Pilih ikon peluncur aplikasi di kiri atas dan pilih **admin**.

   C. Di navigasi kiri bawah, Perluas **admin** dan pilih **Exchange**.

   D. Pergi ke **perlindungan**  >  **DKIM**.

   E. Pilih domain, lalu pilih **Aktifkan** untuk **menandatangani pesan untuk domain ini dengan tanda tangan DKIM**. Ulangi langkah ini untuk setiap domain kustom.
