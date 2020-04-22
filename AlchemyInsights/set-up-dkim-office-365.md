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
ms.openlocfilehash: d23a816d4eef065f800eaee60829d57dc1e7177f
ms.sourcegitcommit: 6bf1d945b4fd6a1fe37d00c5ea99adea7eef9910
ms.translationtype: MT
ms.contentlocale: id-ID
ms.lasthandoff: 04/21/2020
ms.locfileid: "43645675"
---
# <a name="setup-dkim"></a>Pengaturan DKIM

Petunjuk lengkap untuk mengonfigurasi DKIM untuk domain kustom di Microsoft 365 ada [di sini](https://docs.microsoft.com/office365/SecurityCompliance/use-dkim-to-validate-outbound-email#what-you-need-to-do-to-manually-set-up-dkim-in-office-365).

1. Untuk **setiap** domain kustom, Anda perlu membuat **dua** data CNAME DKIM di layanan hosting DNS domain (biasanya, registrar domain). Misalnya, contoso.com dan fourthcoffee.com memerlukan empat data CNAME DKIM: dua untuk contoso.com dan dua untuk fourthcoffee.com.

   Data CNAME DKIM untuk **setiap** domain kustom menggunakan format berikut:

   - **Nama host**:`selector1._domainkey.<CustomDomain>`

     **Poin ke alamat atau nilai**:`selector1-<DomainGUID>._domainkey.<InitialDomain>`

     **TTL**: 3600

   - **Nama host**:`selector2._domainkey.<CustomDomain>`

     **Poin ke alamat atau nilai**:`selector2-<DomainGUID>._domainkey.<InitialDomain>`

     **TTL**: 3600

   \<DomainGUID\> adalah teks `.mail.protection.outlook.com` di sebelah kiri dalam data MX yang disesuaikan untuk domain kustom (misalnya, `contoso-com` untuk domain contoso.com). \<InitialDomain\> adalah domain yang Anda gunakan ketika Anda mendaftar untuk Microsoft 365 (misalnya, contoso.onmicrosoft.com).

2. Setelah membuat data CNAME untuk domain kustom, selesaikan petunjuk berikut:

   J. [masuk ke Microsoft 365](https://support.office.microsoft.com/article/e9eb7d51-5430-4929-91ab-6157c5a050b4) dengan akun kantor atau sekolah.

   B. Pilih ikon peluncur aplikasi di kiri atas dan pilih **admin**.

   C. Di navigasi kiri bawah, Perluas **admin** dan pilih **Exchange**.

   D. Pergi ke **perlindungan** > **DKIM**.

   E. Pilih domain, lalu pilih **Aktifkan** untuk **menandatangani pesan untuk domain ini dengan tanda tangan DKIM**. Ulangi langkah ini untuk setiap domain kustom.
