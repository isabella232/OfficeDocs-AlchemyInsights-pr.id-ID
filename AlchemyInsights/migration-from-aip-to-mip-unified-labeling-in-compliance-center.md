---
title: Melakukan migrasi dari AIP ke MIP/Unified Labeling di Pusat Kepatuhan
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
- "9002278"
- "5114"
ms.openlocfilehash: 12f5f5c46edd7918618c55a8a1905f3b28643092
ms.sourcegitcommit: 8bc60ec34bc1e40685e3976576e04a2623f63a7c
ms.translationtype: MT
ms.contentlocale: id-ID
ms.lasthandoff: 04/15/2021
ms.locfileid: "51825374"
---
# <a name="migration-from-aip-to-mipunified-labeling-in-the-compliance-center"></a>Melakukan migrasi dari AIP ke MIP/Unified Labeling di Pusat Kepatuhan

Untuk melakukan migrasi dari label AIP ke Label Terpadu di pusat Keamanan dan Kepatuhan, lakukan hal berikut:

**Mengaktifkan proteksi dari portal Azure**

1. Jika Anda belum melakukannya, buka jendela browser baru dan [masuk ke portal Azure](https://docs.microsoft.com/azure/information-protection/deploy-use/configure-policy#signing-in-to-the-azure-portal). Navigasikan ke **blade Perlindungan Informasi Azure.** Misalnya, pada menu hub, klik Semua **layanan dan** mulai mengetik **Informasi** dalam kotak Filter. Pilih **Azure Information Protection**. Jika Anda belum mengakses blade Perlindungan Informasi Azure sebelumnya, [](https://docs.microsoft.com/azure/information-protection/deploy-use/configure-policy#to-access-the-azure-information-protection-blade-for-the-first-time) lihat langkah tambahan satu kali untuk menambahkan blade ini ke portal. Untuk membuka blade Perlindungan Informasi Azure, Anda harus memiliki paket [Azure Information Protection Premium](https://www.microsoft.com/cloud-platform/azure-information-protection-pricing) atau paket Office 365 yang menyertakan Manajemen Hak. Jika Anda memiliki salah satu langganan ini namun melihat pesan bahwa langganan yang valid tidak dapat ditemukan, hubungi [Dukungan Microsoft](https://docs.microsoft.com/azure/information-protection/get-started/information-support#to-contact-microsoft-support) atau gunakan saluran dukungan standar Anda.

2. Temukan **opsi** menu Kelola, dan pilih Aktivasi **proteksi**. Klik **Aktifkan**, lalu konfirmasi tindakan Anda. Ketika aktivasi selesai, bilah informasi **menampilkan Aktivasi selesai dengan sukses**.

**Melakukan migrasi label Perlindungan Informasi Azure ke Pusat Keamanan Office 365 & Kepatuhan**

1. Pastikan Anda masuk sebagai pengguna dengan izin Administrator Global.

2. Navigasikan ke **blade Perlindungan Informasi Azure.**

3. Dari **opsi** menu Kelola, pilih **Label terpadu**.

4. Di **blade Perlindungan Informasi Azure - Labeling** terpadu, klik **Aktifkan,** lalu ikuti instruksi online.

**Catatan**: Verifikasi bahwa Anda memiliki izin yang tepat sebelum mengaktifkan Migrasi Pusat & Kepatuhan. Lihat artikel berikut ini untuk informasi selengkapnya:

1. [Apakah Anda perlu menjadi admin global untuk mengonfigurasi Perlindungan Informasi Azure, atau dapatkah saya mendelegasikan kepada administrator lain?](https://docs.microsoft.com/azure/information-protection/faqs#do-you-need-to-be-a-global-admin-to-configure-azure-information-protection-or-can-i-delegate-to-other-administrators)

2. [Informasi penting tentang peran administratif setelah melakukan migrasi ke Pusat & Kepatuhan.](https://docs.microsoft.com/azure/information-protection/configure-policy-migrate-labels#important-information-about-administrative-roles)

Untuk informasi selengkapnya tentang migrasi AIP ke Label Terpadu ke Pusat Keamanan dan Kepatuhan, lihat [Memigrasikan label](https://docs.microsoft.com/azure/information-protection/configure-policy-migrate-labels).
