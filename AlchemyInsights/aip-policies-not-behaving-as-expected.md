---
title: 'AIP: kebijakan tidak berperilaku seperti yang diharapkan'
ms.author: pebaum
author: pebaum
manager: mnirkhe
ms.audience: Admin
ms.topic: article
ms.service: o365-administration
ROBOTS: NOINDEX, NOFOLLOW
localization_priority: Priority
ms.collection: Adm_O365
ms.custom:
- "9002266"
- "4780"
ms.openlocfilehash: 0dfaae776ec551fe12919e8a8e69f2e7a58d67d0
ms.sourcegitcommit: c6692ce0fa1358ec3529e59ca0ecdfdea4cdc759
ms.translationtype: MT
ms.contentlocale: id-ID
ms.lasthandoff: 09/14/2020
ms.locfileid: "47663192"
---
# <a name="aip-policies-not-behaving-as-expected"></a>AIP: kebijakan tidak berperilaku seperti yang diharapkan

Perlindungan informasi Azure: kebijakan tidak berperilaku seperti yang diharapkan, lihat berikut ini untuk panduan yang direkomendasikan untuk berbagai masalah kebijakan:

1. Jika Anda mengalami masalah dengan tanda visual, silakan Tinjau [Kapan tanda visual diterapkan](https://docs.microsoft.com/azure/information-protection/configure-policy-markings#when-visual-markings-are-applied).
2. Jika Anda mengalami masalah dengan pelabelan otomatis, silakan Tinjau [cara mengonfigurasi ketentuan untuk klasifikasi otomatis dan yang direkomendasikan untuk proteksi informasi Azure](https://docs.microsoft.com/azure/information-protection/configure-policy-classification) dan [apa yang dicari tipe informasi sensitif](https://docs.microsoft.com/microsoft-365/compliance/sensitive-information-type-entity-definitions).
3. Jika Anda mengalami masalah dengan proteksi Native/Pfile, silakan Tinjau [konfigurasi file api](https://docs.microsoft.com/azure/information-protection/develop/file-api-configuration).
4. Periksa apakah Anda menggunakan kebijakan lingkup yang tidak dikonfigurasi dengan benar: [cara mengonfigurasi kebijakan perlindungan informasi Azure untuk pengguna tertentu dengan menggunakan kebijakan lingkup](https://docs.microsoft.com/azure/information-protection/configure-policy-scope).
5. Jika label otomatis tidak berfungsi untuk Outlook saat melampirkan dokumen berlabel, pastikan bahwa DRMEncryptProperty tidak ditentukan seperti yang diuraikan di sini: [pengaturan registri IRM untuk keamanan](https://docs.microsoft.com/deployoffice/security/protect-sensitive-messages-and-documents-by-using-irm-in-office#office-2016-irm-registry-key-options).

Jika Anda masih mengalami masalah, silakan kumpulkan log klien proteksi informasi Azure dan lampirkan log yang diekspor ke tiket ini.

1. Buka dokumen Office atau buat email baru di Outlook.
2. Klik **proteksi/kepekaan**  >  **bantuan dan umpan balik**.
3. Klik **ekspor log**.
4. Simpan log ke pilihan lokasi Anda, lalu Lampirkan ke permintaan layanan ini.

Sumber daya tambahan:

- [Cara mengonfigurasikan label untuk tanda visual untuk proteksi informasi Azure](https://docs.microsoft.com/azure/information-protection/configure-policy-markings)
- [Meninjau dokumentasi perlindungan informasi Azure](https://docs.microsoft.com/azure/information-protection/what-is-information-protection)
- [Menggunakan label sensitivitas dalam aplikasi Microsoft 365](https://docs.microsoft.com/microsoft-365/compliance/sensitivity-labels-office-apps)

