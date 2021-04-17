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
ms.openlocfilehash: b7ab09fe8430a54dacf2cd1ba076414a5f562541
ms.sourcegitcommit: 8bc60ec34bc1e40685e3976576e04a2623f63a7c
ms.translationtype: HT
ms.contentlocale: id-ID
ms.lasthandoff: 04/15/2021
ms.locfileid: "51820901"
---
# <a name="automatic-classification-not-behaving-as-expected-with-the-aip-client"></a>Klasifikasi otomatis tidak berperilaku seperti yang diharapkan dengan klien AIP

Klasifikasi otomatis tidak berperilaku seperti yang diharapkan, gunakan panduan yang disarankan berikut ini:

1. Jika Anda mengalami masalah dengan label otomatis, lihat [Cara mengonfigurasi kondisi untuk klasifikasi otomatis dan direkomendasikan untuk Perlindungan Informasi Azure](https://docs.microsoft.com/azure/information-protection/configure-policy-classification) dan [Apa yang dilihat tipe informasi sensitif](https://docs.microsoft.com/microsoft-365/compliance/sensitive-information-type-entity-definitions).
2. Periksa apakah Anda menggunakan kebijakan terinvestigasi yang tidak dikonfigurasi dengan benar: [Cara mengonfigurasi kebijakan Perlindungan Informasi Azure untuk pengguna tertentu dengan menggunakan kebijakan terinvestigasi](https://docs.microsoft.com/azure/information-protection/configure-policy-scope).
3. Jika label otomatis tidak berfungsi untuk Outlook saat melampirkan dokumen berlabel, verifikasi bahwa `DRMEncryptProperty` tidak ditentukan seperti yang diuraikan di sini: [pengaturan registri IRM untuk keamanan](https://docs.microsoft.com/deployoffice/security/protect-sensitive-messages-and-documents-by-using-irm-in-office#office-2016-irm-registry-key-options).
4. Jika menggunakan [tipe informasi bawaan](https://support.office.com/article/What-the-sensitive-information-types-look-for-fd505979-76be-4d9f-b459-abef3fc9e86b) untuk kebijakan Perlindungan Informasi Azure, verifikasi bahwa konten Anda cocok dengan format yang diharapkan.
5. Verifikasi bahwa label dikonfigurasi dengan tepat untuk **Otomatis** atau **Disarankan**. (Label **otomatis** tersedia untuk semua aplikasi Microsoft 365, sedangkan **Yang Disarankan** tersedia untuk semua aplikasi Microsoft 365 kecuali Outlook.)
6. Anda tidak dapat menggunakan klasifikasi otomatis untuk dokumen dan email yang sebelumnya diberi label secara manual atau sebelumnya diberi label secara otomatis dengan klasifikasi yang lebih tinggi.  Untuk informasi selengkapnya, lihat: [Bagaimana label otomatis atau label yang direkomendasikan diterapkan](https://docs.microsoft.com/azure/information-protection/configure-policy-classification#how-automatic-or-recommended-labels-are-applied).
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
