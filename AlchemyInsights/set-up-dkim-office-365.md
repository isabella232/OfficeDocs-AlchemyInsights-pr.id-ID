---
title: Setup DKIM di Office 365
ms.author: chrisda
author: chrisda
manager: dansimp
ms.audience: ITPro
ms.topic: article
ROBOTS: NOINDEX, NOFOLLOW
localization_priority: Normal
ms.custom: 1388
ms.assetid: ''
ms.openlocfilehash: dd908db6a4bc1739b3c1cff059387034d67e093d
ms.sourcegitcommit: b3e55405af384e868fcd32ea794eb15d1356c3fc
ms.translationtype: MT
ms.contentlocale: id-ID
ms.lasthandoff: 08/29/2019
ms.locfileid: "36666267"
---
# <a name="setup-dkim-in-office-365"></a>Setup DKIM di Office 365

Petunjuk lengkap untuk mengkonfigurasi DKIM untuk custom domain di Office 365 [di sini](https://docs.microsoft.com/office365/SecurityCompliance/use-dkim-to-validate-outbound-email#what-you-need-to-do-to-manually-set-up-dkim-in-office-365).

1. Untuk **setiap** domain kustom, Anda perlu membuat **dua** DKIM CNAME records di layanan hosting DNS domain Anda (biasanya, registrar domain). Misalnya, contoso.com dan fourthcoffee.com memerlukan empat DKIM CNAME records: dua untuk contoso.com dan dua untuk fourthcoffee.com.

   DKIM CNAME records untuk **setiap** domain kustom menggunakan format berikut:

   - **Nama host**:`selector1._domainkey.<CustomDomain>`

     **Poin ke alamat atau nilai**:`selector1-<DomainGUID>._domainkey.<InitialDomain>`

     **TTL**: 3600

   - **Nama host**:`selector2._domainkey.<CustomDomain>`

     **Poin ke alamat atau nilai**:`selector2-<DomainGUID>._domainkey.<InitialDomain>`

     **TTL**: 3600

   \<DomainGUID\> adalah teks di sebelah kiri `.mail.protection.outlook.com` dalam data MX disesuaikan untuk custom domain (misalnya, `contoso-com` untuk domain contoso.com). \<InitialDomain\> adalah domain yang digunakan saat mendaftar ke Office 365 (misalnya, contoso.onmicrosoft.com).

2. Setelah membuat data CNAME untuk domain kustom, lengkap petunjuk berikut:

   a. [Masuk ke kantor 365](https://support.office.microsoft.com/article/e9eb7d51-5430-4929-91ab-6157c5a050b4) dengan akun kantor atau sekolah.

   b. Pilih ikon peluncur app di kiri dan pilih **Admin**.

   c. Pada navigasi kiri, memperluas **Admin** dan memilih **asing**.

   d. Pergi ke **perlindungan** > **DKIM**.

   e. Pilih domain, dan kemudian memilih **mengaktifkan** **tanda**pesan untuk domain ini dengan DKIM tanda tangan. Ulangi langkah ini untuk setiap domain kustom.
