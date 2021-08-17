---
title: DKIM Penyiapan
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
ms.openlocfilehash: 5dc90965516cc4d360b9be56c7737c6d134123ea8ac263b092559dd1416faff4
ms.sourcegitcommit: b5f7da89a650d2915dc652449623c78be6247175
ms.translationtype: MT
ms.contentlocale: id-ID
ms.lasthandoff: 08/05/2021
ms.locfileid: "54108559"
---
# <a name="setup-dkim"></a>DKIM Penyiapan

Instruksi lengkap untuk mengonfigurasi DKIM untuk domain kustom dalam Microsoft 365 ada [di sini.](https://docs.microsoft.com/microsoft-365/security/office-365-security/use-dkim-to-validate-outbound-email#steps-you-need-to-do-to-manually-set-up-dkim)

1. Untuk **setiap** domain kustom, Anda perlu membuat **dua** catatan DKIM CNAME di layanan hosting DNS domain (biasanya, pendaftar domain). Misalnya, untuk contoso.com dan fourthcoffee.com memerlukan empat data CNAME DKIM: dua untuk contoso.com dan dua untuk fourthcoffee.com.

   Catatan DKIM CNAME untuk **setiap** domain kustom menggunakan format berikut:

   - **Nama host**: `selector1._domainkey.<CustomDomain>`

     **Alamat atau nilai yang ditujukan:**`selector1-<DomainGUID>._domainkey.<InitialDomain>`

     **TTL**: 3600

   - **Nama host**: `selector2._domainkey.<CustomDomain>`

     **Alamat atau nilai yang ditujukan:**`selector2-<DomainGUID>._domainkey.<InitialDomain>`

     **TTL**: 3600

   \<DomainGUID\> adalah teks di sebelah kiri dalam catatan MX yang dikustomisasi untuk domain kustom `.mail.protection.outlook.com` (misalnya, `contoso-com` untuk bidang contoso.com). \<InitialDomain\>adalah domain yang Anda gunakan saat Anda mendaftar untuk Microsoft 365 (misalnya, contoso.onmicrosoft.com).

2. Setelah membuat catatan CNAME untuk domain kustom Anda, selesaikan instruksi berikut ini:

   a. [masuk ke Microsoft 365](https://support.office.microsoft.com/article/e9eb7d51-5430-4929-91ab-6157c5a050b4) dengan akun kerja atau sekolah Anda.

   b. Pilih ikon peluncur aplikasi di kiri atas dan pilih **Admin**.

   c. Di navigasi kiri bawah, perluas **Admin dan** **pilih Exchange**.

   d. Buka **Proteksi**  >  **DKIM**.

   e. Pilih domain, lalu pilih **Aktifkan untuk** Menandatangani pesan untuk domain ini dengan tanda **tangan DKIM**. Ulangi langkah ini untuk setiap domain kustom.
