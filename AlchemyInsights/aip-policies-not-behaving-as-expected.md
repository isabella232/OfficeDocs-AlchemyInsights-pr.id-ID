---
title: 'AIP: Kebijakan tidak seperti yang diharapkan'
ms.author: pebaum
author: pebaum
manager: scotv
ms.audience: Admin
ms.topic: article
ms.service: o365-administration
ROBOTS: NOINDEX, NOFOLLOW
localization_priority: Priority
ms.collection: Adm_O365
ms.custom:
- "9002266"
- "4780"
ms.openlocfilehash: 90448bf57297ce59ba222efd1927b5de588bfbfdb1206b6403764d7f43fed690
ms.sourcegitcommit: b5f7da89a650d2915dc652449623c78be6247175
ms.translationtype: MT
ms.contentlocale: id-ID
ms.lasthandoff: 08/05/2021
ms.locfileid: "53934296"
---
# <a name="aip-policies-not-behaving-as-expected"></a>AIP: Kebijakan tidak seperti yang diharapkan

Perlindungan Informasi Azure: Kebijakan yang tidak seperti yang diharapkan, lihat panduan yang disarankan untuk berbagai masalah kebijakan:

1. Jika Anda mengalami masalah dengan penandaan visual, [tinjau Ketika penandaan visual diterapkan.](https://docs.microsoft.com/azure/information-protection/configure-policy-markings#when-visual-markings-are-applied)
2. Jika Anda mengalami masalah dengan label otomatis, silakan tinjau Cara mengonfigurasi persyaratan klasifikasi otomatis dan direkomendasikan untuk Perlindungan Informasi [Azure](https://docs.microsoft.com/azure/information-protection/configure-policy-classification) dan Apa tipe informasi [sensitif mencari](https://docs.microsoft.com/microsoft-365/compliance/sensitive-information-type-entity-definitions).
3. Jika mengalami masalah dengan perlindungan Native/Pfile, silakan [tinjau konfigurasi File API](https://docs.microsoft.com/azure/information-protection/develop/file-api-configuration).
4. Periksa apakah Anda menggunakan kebijakan dibatasi yang tidak dikonfigurasi dengan benar: [Cara mengonfigurasi kebijakan Perlindungan Informasi Azure untuk pengguna tertentu menggunakan kebijakan dibatasi](https://docs.microsoft.com/azure/information-protection/configure-policy-scope).
5. Jika label otomatis tidak berfungsi untuk Outlook saat melampirkan dokumen berlabel, verifikasi bahwa DRMEncryptProperty tidak didefinisikan seperti yang diuraikan di sini: [Pengaturan registri IRM untuk keamanan.](https://docs.microsoft.com/deployoffice/security/protect-sensitive-messages-and-documents-by-using-irm-in-office#office-2016-irm-registry-key-options)

Jika Anda masih mengalami masalah, silakan kumpulkan log klien Perlindungan Informasi Azure dan lampirkan log yang diekspor ke tiket ini.

1. Buka dokumen Office atau buat email baru di Outlook.
2. Klik **Proteksi/Sensitivitas** > **Bantuan dan umpan balik**.
3. Klik **Ekspor Log**.
4. Simpan log ke lokasi pilihan Anda, dan lampirkan log ke permintaan layanan ini.

Sumber daya tambahan:

- [Cara mengonfigurasi label untuk penandaan visual untuk Perlindungan Informasi Azure](https://docs.microsoft.com/azure/information-protection/configure-policy-markings)
- [Tinjau dokumentasi Perlindungan Informasi Azure](https://docs.microsoft.com/azure/information-protection/what-is-information-protection)
- [Menggunakan label sensitivitas di Microsoft 365 ini](https://docs.microsoft.com/microsoft-365/compliance/sensitivity-labels-office-apps)

