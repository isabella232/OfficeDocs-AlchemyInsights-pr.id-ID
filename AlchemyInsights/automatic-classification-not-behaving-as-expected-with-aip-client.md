---
title: Klasifikasi otomatis tidak berperilaku seperti yang diharapkan dengan klien AIP
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
- "4373"
ms.openlocfilehash: 95a994d6a49ee8737a6ebcb196314f92776d8482
ms.sourcegitcommit: 2afad0b107d03cd8c4de0b85b5bee38a13a7960d
ms.translationtype: MT
ms.contentlocale: id-ID
ms.lasthandoff: 05/26/2020
ms.locfileid: "44493175"
---
# <a name="automatic-classification-not-behaving-as-expected-with-the-aip-client"></a>Klasifikasi otomatis tidak berperilaku seperti yang diharapkan dengan klien AIP

Klasifikasi otomatis tidak berperilaku seperti yang diharapkan, gunakan panduan direkomendasikan berikut ini:

1. Jika Anda mengalami masalah dengan pelabelan otomatis, lihat [cara mengkonfigurasi kondisi untuk klasifikasi otomatis dan direkomendasikan untuk perlindungan informasi Azure](https://docs.microsoft.com/azure/information-protection/configure-policy-classification) dan [apa yang dicari jenis informasi sensitif](https://docs.microsoft.com/office365/securitycompliance/what-the-sensitive-information-types-look-for).
2. Periksa apakah Anda menggunakan kebijakan scoped yang tidak dikonfigurasi dengan benar: [cara mengkonfigurasi kebijakan perlindungan informasi Azure untuk pengguna tertentu dengan menggunakan kebijakan scoped](https://docs.microsoft.com/azure/information-protection/configure-policy-scope).
3. Jika pelabelan otomatis tidak bekerja untuk Outlook saat melampirkan dokumen berlabel, verifikasi yang `DRMEncryptProperty` tidak ditetapkan seperti yang dijelaskan di sini: [pengaturan registri IRM untuk keamanan](https://docs.microsoft.com/deployoffice/security/protect-sensitive-messages-and-documents-by-using-irm-in-office#office-2016-irm-registry-key-options).
4. Jika Anda menggunakan [jenis informasi internal](https://support.office.com/article/What-the-sensitive-information-types-look-for-fd505979-76be-4d9f-b459-abef3fc9e86b) untuk kebijakan perlindungan informasi Azure, Verifikasikan bahwa konten Anda sesuai dengan format yang diharapkan.
5. Verifikasi bahwa label dikonfigurasi dengan benar untuk **otomatis** atau **direkomendasikan**. (Pelabelan**otomatis** tersedia untuk semua aplikasi Office, sedangkan **disarankan** tersedia untuk semua aplikasi Office kecuali untuk Outlook.)
6. Anda tidak dapat menggunakan klasifikasi otomatis untuk dokumen dan email yang sebelumnya diberi label secara manual atau sebelumnya secara otomatis diberi label dengan klasifikasi yang lebih tinggi.  Untuk informasi lebih lanjut, lihat: [bagaimana label otomatis atau rekomendasi diterapkan](https://docs.microsoft.com/azure/information-protection/configure-policy-classification#how-automatic-or-recommended-labels-are-applied).
7. Jika Anda masih mengalami masalah, silakan mengumpulkan log klien perlindungan informasi Azure dan melampirkan log yang diekspor ke tiket dukungan Anda. Untuk mengekspor log perlindungan informasi Azure:
    - Buka dokumen Office atau buat email baru di Outlook.
    - Klik **Lindungi/sensitivitas**  >  **bantuan dan umpan balik**.
    - Klik **ekspor log**.
    - Simpan log ke pilihan lokasi Anda, dan pasangkan ke permintaan layanan Anda.

Untuk informasi tambahan, lihat:

- [Cara mengkonfigurasi kondisi untuk klasifikasi otomatis dan direkomendasikan untuk perlindungan informasi Azure](https://docs.microsoft.com/azure/information-protection/configure-policy-classification)
- [Panduan cara untuk skenario umum yang menggunakan perlindungan informasi Azure](https://docs.microsoft.com/azure/information-protection/how-to-guides)
- [Tinjau dokumentasi perlindungan informasi Azure](https://docs.microsoft.com/azure/information-protection/what-is-information-protection)
- [Meninjau langganan dan fitur perlindungan informasi Azure](https://azure.microsoft.com/pricing/details/information-protection)
- [Persyaratan untuk perlindungan informasi Azure](https://docs.microsoft.com/azure/information-protection/get-started/requirements)
- [Tutorial memulai cepat untuk perlindungan informasi Azure](https://docs.microsoft.com/azure/information-protection/get-started/infoprotect-quick-start-tutorial)
- [Unduh klien perlindungan informasi Azure](https://www.microsoft.com/download/details.aspx?id=53018)
