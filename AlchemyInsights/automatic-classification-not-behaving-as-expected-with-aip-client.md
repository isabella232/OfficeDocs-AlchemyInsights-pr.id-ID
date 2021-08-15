---
title: Klasifikasi otomatis tidak berperilaku seperti yang diharapkan dengan klien AIP
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
- "4373"
ms.openlocfilehash: 93d15b8b65fd52a567ecbb6e1f84363bf2b38946c105896b0b5ef41e49d16ea9
ms.sourcegitcommit: b5f7da89a650d2915dc652449623c78be6247175
ms.translationtype: MT
ms.contentlocale: id-ID
ms.lasthandoff: 08/05/2021
ms.locfileid: "53979712"
---
# <a name="automatic-classification-not-behaving-as-expected-with-the-aip-client"></a>Klasifikasi otomatis tidak berperilaku seperti yang diharapkan dengan klien AIP

Klasifikasi otomatis tidak berperilaku seperti yang diharapkan, gunakan panduan yang disarankan berikut ini:

1. Jika Anda mengalami masalah dengan pelabelan otomatis, lihat [Cara mengonfigurasi kondisi untuk klasifikasi otomatis dan rekomendasi untuk Perlindungan Informasi Azure](https://docs.microsoft.com/azure/information-protection/configure-policy-classification) dan [Apa yang dilihat tipe informasi sensitif](https://docs.microsoft.com/microsoft-365/compliance/sensitive-information-type-entity-definitions).
2. Periksa apakah Anda menggunakan kebijakan dibatasi yang tidak dikonfigurasi dengan benar: [Cara mengonfigurasi kebijakan Perlindungan Informasi Azure untuk pengguna tertentu menggunakan kebijakan dibatasi](https://docs.microsoft.com/azure/information-protection/configure-policy-scope).
3. Jika pelabelan otomatis tidak berfungsi untuk Outlook saat melampirkan dokumen berlabel, verifikasi bahwa `DRMEncryptProperty` tidak ditentukan seperti yang diuraikan di sini: [Pengaturan registri IRM untuk keamanan](https://docs.microsoft.com/deployoffice/security/protect-sensitive-messages-and-documents-by-using-irm-in-office#office-2016-irm-registry-key-options).
4. Jika menggunakan [tipe informasi bawaan](https://support.office.com/article/What-the-sensitive-information-types-look-for-fd505979-76be-4d9f-b459-abef3fc9e86b) untuk kebijakan Perlindungan Informasi Azure, verifikasi bahwa konten Anda cocok dengan format yang diharapkan.
5. Verifikasi bahwa label dikonfigurasi dengan benar untuk **Otomatis** atau **Rekomendasi**. (Pelabelan **Otomatis** tersedia untuk semua aplikasi Microsoft 365, sementara **Rekomendasi** tersedia untuk semua aplikasi Microsoft 365 kecuali Outlook.)
6. Anda tidak dapat menggunakan klasifikasi otomatis untuk dokumen dan email yang sebelumnya diberi label secara manual atau sebelumnya diberi label secara otomatis dengan klasifikasi yang lebih tinggi.  Untuk informasi selengkapnya, lihat: [Cara label otomatis atau rekomendasi diterapkan](https://docs.microsoft.com/azure/information-protection/configure-policy-classification#how-automatic-or-recommended-labels-are-applied).
7. Jika masih mengalami masalah, silakan kumpulkan log klien Perlindungan Informasi Azure lalu lampirkan log yang diekspor ke tiket dukungan Anda. Untuk mengekspor log Perlindungan Informasi Azure:
    - Buka dokumen Office atau buat email baru di Outlook.
    - Klik **Proteksi/Sensitivitas** > **Bantuan dan umpan balik**.
    - Klik **Ekspor Log**.
    - Simpan log ke lokasi pilihan, lalu lampirkan ke permintaan layanan Anda.

Untuk informasi tambahan, lihat:

- [Cara mengonfigurasi kondisi untuk klasifikasi otomatis dan rekomendasi untuk Perlindungan Informasi Azure](https://docs.microsoft.com/azure/information-protection/configure-policy-classification)
- [Panduan untuk skenario umum yang menggunakan Perlindungan Informasi Azure](https://docs.microsoft.com/azure/information-protection/how-to-guides)
- [Tinjau dokumentasi Perlindungan Informasi Azure](https://docs.microsoft.com/azure/information-protection/what-is-information-protection)
- [Tinjau langganan dan fitur Perlindungan Informasi Azure](https://azure.microsoft.com/pricing/details/information-protection)
- [Persyaratan untuk Perlindungan Informasi Azure](https://docs.microsoft.com/azure/information-protection/get-started/requirements)
- [Tutorial mulai cepat untuk Perlindungan Informasi Azure](https://docs.microsoft.com/azure/information-protection/get-started/infoprotect-quick-start-tutorial)
- [Unduh klien Perlindungan Informasi Azure](https://www.microsoft.com/download/details.aspx?id=53018)
