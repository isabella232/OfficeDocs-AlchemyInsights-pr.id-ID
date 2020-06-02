---
title: 'AIP: kebijakan tidak berperilaku seperti yang diharapkan'
ms.author: pebaum
author: pebaum
manager: mnirkhe
ms.audience: Admin
ms.topic: article
ROBOTS: NOINDEX, NOFOLLOW
localization_priority: Priority
ms.collection: Adm_O365
ms.custom:
- "9002266"
- "4780"
ms.openlocfilehash: 527556fcb02525eb88ea992c38a2ddfcba6f9453
ms.sourcegitcommit: bc7d6f4f3c9f7060d073f5130e1ec856e248d020
ms.translationtype: HT
ms.contentlocale: id-ID
ms.lasthandoff: 06/02/2020
ms.locfileid: "44506561"
---
# <a name="aip-policies-not-behaving-as-expected"></a>AIP: kebijakan tidak berperilaku seperti yang diharapkan

Perlindungan informasi Azure: kebijakan yang tidak berperilaku seperti yang diharapkan, lihat berikut ini untuk panduan yang disarankan untuk berbagai masalah kebijakan:

1. Jika Anda mengalami masalah dengan tanda visual, silakan Tinjau [saat tanda visual diterapkan](https://docs.microsoft.com/azure/information-protection/configure-policy-markings#when-visual-markings-are-applied).
2. Jika Anda mengalami masalah dengan pelabelan otomatis, Tinjau [cara mengonfigurasi ketentuan untuk klasifikasi otomatis dan direkomendasikan untuk perlindungan informasi Azure](https://docs.microsoft.com/azure/information-protection/configure-policy-classification) dan [apa yang dicari oleh jenis informasi sensitif](https://docs.microsoft.com/microsoft-365/compliance/sensitive-information-type-entity-definitions).
3. Jika Anda mengalami masalah dengan perlindungan Native/Pfile, silakan Tinjau [konfigurasi file api](https://docs.microsoft.com/azure/information-protection/develop/file-api-configuration).
4. Periksa apakah Anda menggunakan kebijakan scoped yang tidak dikonfigurasi dengan benar: [cara mengkonfigurasi kebijakan perlindungan informasi Azure untuk pengguna tertentu dengan menggunakan kebijakan scoped](https://docs.microsoft.com/azure/information-protection/configure-policy-scope).
5. Jika pelabelan otomatis tidak bekerja untuk Outlook saat melampirkan dokumen berlabel, verifikasi bahwa DRMEncryptProperty tidak ditetapkan seperti yang dijelaskan di sini: [IRM pengaturan registri untuk keamanan](https://docs.microsoft.com/deployoffice/security/protect-sensitive-messages-and-documents-by-using-irm-in-office#office-2016-irm-registry-key-options).

Jika Anda masih mengalami masalah, silakan mengumpulkan klien perlindungan informasi Azure log dan melampirkan log diekspor ke tiket ini.

1. Buka dokumen Office atau buat email baru di Outlook.
2. Klik **Lindungi/sensitivitas**  >  **bantuan dan umpan balik**.
3. Klik **ekspor log**.
4. Simpan log ke pilihan lokasi Anda, dan pasangkan ke permintaan layanan ini.

Sumber daya tambahan:

- [Cara mengkonfigurasi label untuk tanda visual untuk perlindungan informasi Azure](https://docs.microsoft.com/azure/information-protection/configure-policy-markings)
- [Tinjau dokumentasi perlindungan informasi Azure](https://docs.microsoft.com/azure/information-protection/what-is-information-protection)
- [Menggunakan label sensitivitas di aplikasi Office](https://docs.microsoft.com/microsoft-365/compliance/sensitivity-labels-office-apps)

