---
title: Penyetelan DKIM
ms.author: chrisda
author: chrisda
manager: dansimp
ms.audience: ITPro
ms.topic: article
ms.service: o365-administration
ROBOTS: NOINDEX, NOFOLLOW
localization_priority: Normal
ms.custom: 1388
ms.assetid: ''
ms.openlocfilehash: b34bfdafcab6229a4dd2e9d9f23103fa13556482
ms.sourcegitcommit: c6692ce0fa1358ec3529e59ca0ecdfdea4cdc759
ms.translationtype: MT
ms.contentlocale: id-ID
ms.lasthandoff: 09/15/2020
ms.locfileid: "47808710"
---
# <a name="setup-dkim"></a>Penyetelan DKIM

Instruksi lengkap untuk mengonfigurasi DKIM untuk domain kustom di Microsoft 365 ada [di sini](https://docs.microsoft.com/microsoft-365/security/office-365-security/use-dkim-to-validate-outbound-email#steps-you-need-to-do-to-manually-set-up-dkim).

1. Untuk **setiap** domain kustom, Anda perlu membuat **dua** catatan CNAME DKIM di layanan hosting DNS domain Anda (biasanya, pencatat domain). Misalnya, contoso.com dan fourthcoffee.com memerlukan empat catatan CNAME DKIM: dua untuk contoso.com dan dua untuk fourthcoffee.com.

   Catatan CNAME DKIM untuk **setiap** domain kustom menggunakan format berikut:

   - **Nama host**: `selector1._domainkey.<CustomDomain>`

     **Mengarahkan ke alamat atau nilai**: `selector1-<DomainGUID>._domainkey.<InitialDomain>`

     **TTL**: 3600

   - **Nama host**: `selector2._domainkey.<CustomDomain>`

     **Mengarahkan ke alamat atau nilai**: `selector2-<DomainGUID>._domainkey.<InitialDomain>`

     **TTL**: 3600

   \<DomainGUID\> adalah teks di sebelah kiri `.mail.protection.outlook.com` catatan MX yang dikustomisasi untuk domain kustom (misalnya, `contoso-com` untuk domain contoso.com). \<InitialDomain\> adalah domain yang Anda gunakan saat mendaftar untuk Microsoft 365 (misalnya, contoso.onmicrosoft.com).

2. Setelah Anda membuat catatan CNAME untuk domain kustom Anda, selesaikan instruksi berikut:

   untuk. [masuk ke Microsoft 365](https://support.office.microsoft.com/article/e9eb7d51-5430-4929-91ab-6157c5a050b4) dengan akun kantor atau sekolah Anda.

   b. Pilih ikon peluncur aplikasi di kiri atas dan pilih **admin**.

   's. Di navigasi kiri bawah, Perluas **admin** dan pilih **Exchange**.

   dih. Buka **proteksi**  >  **DKIM**.

   e. Pilih domain, lalu pilih **Aktifkan** untuk **tanda tangani pesan untuk domain ini dengan tanda tangan DKIM**. Ulangi langkah ini untuk setiap domain kustom.
