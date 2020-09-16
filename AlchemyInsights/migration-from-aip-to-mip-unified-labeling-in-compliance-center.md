---
title: Migrasi dari AIP ke MIP/pelabelan terpadu di pusat kepatuhan
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
- "9002278"
- "5114"
ms.openlocfilehash: 7157eada10db2443f64fb7925f408359275d75eb
ms.sourcegitcommit: c6692ce0fa1358ec3529e59ca0ecdfdea4cdc759
ms.translationtype: MT
ms.contentlocale: id-ID
ms.lasthandoff: 09/14/2020
ms.locfileid: "47674329"
---
# <a name="migration-from-aip-to-mipunified-labeling-in-the-compliance-center"></a>Migrasi dari AIP ke MIP/pelabelan terpadu di pusat kepatuhan

Untuk melakukan migrasi dari label AIP ke pelabelan terpadu di pusat keamanan dan kepatuhan, lakukan hal berikut:

**Mengaktifkan proteksi dari portal Azure**

1. Jika Anda belum melakukannya, buka jendela browser baru dan [masuk ke Azure portal](https://docs.microsoft.com/azure/information-protection/deploy-use/configure-policy#signing-in-to-the-azure-portal). Navigasikan ke bilah **proteksi informasi Azure** . Misalnya, pada menu hub, klik **semua layanan** dan mulai mengetik **informasi** dalam kotak filter. Pilih **proteksi informasi Azure**. Jika Anda belum mengakses bilah proteksi informasi Azure sebelumnya, lihat [langkah-langkah tambahan](https://docs.microsoft.com/azure/information-protection/deploy-use/configure-policy#to-access-the-azure-information-protection-blade-for-the-first-time) satu kali untuk menambahkan bilah ini ke portal. Untuk membuka bilah proteksi informasi Azure, Anda harus memiliki [Paket Premium proteksi informasi Azure](https://www.microsoft.com/cloud-platform/azure-information-protection-pricing) atau paket Office 365 yang menyertakan manajemen hak. Jika Anda memiliki salah satu langganan ini tetapi melihat pesan bahwa langganan yang valid tidak dapat ditemukan, [Hubungi dukungan Microsoft](https://docs.microsoft.com/azure/information-protection/get-started/information-support#to-contact-microsoft-support) atau gunakan saluran dukungan standar Anda.

2. Temukan opsi **Kelola** menu, dan pilih **aktivasi proteksi**. Klik **Aktifkan**, lalu konfirmasikan tindakan Anda. Ketika aktivasi selesai, bilah informasi menampilkan **aktivasi selesai dengan sukses**.

**Migrasi label proteksi informasi Azure ke pusat kepatuhan & keamanan Office 365**

1. Pastikan Anda masuk sebagai pengguna dengan izin administrator global.

2. Navigasikan ke bilah **proteksi informasi Azure** .

3. Dari opsi menu **Kelola** , pilih **label terpadu**.

4. Pada **pelindung informasi Azure-pisau pelabelan terpadu** , klik **Aktifkan** dan ikuti instruksi online.

**Catatan**: verifikasi bahwa Anda memiliki izin yang sesuai sebelum mengaktifkan migrasi keamanan & Compliance Center. Lihat artikel berikut ini untuk informasi selengkapnya:

1. [Apakah Anda perlu menjadi admin global untuk mengonfigurasi proteksi informasi Azure, atau Bisakah saya mendelegasikan ke administrator lain?](https://docs.microsoft.com/azure/information-protection/faqs#do-you-need-to-be-a-global-admin-to-configure-azure-information-protection-or-can-i-delegate-to-other-administrators)

2. [Informasi penting tentang peran administratif setelah bermigrasi ke pusat kepatuhan & keamanan.](https://docs.microsoft.com/azure/information-protection/configure-policy-migrate-labels#important-information-about-administrative-roles)

Untuk informasi selengkapnya tentang RAKUTEN Insight untuk Unified pelabelan migrasi ke pusat keamanan dan kepatuhan, lihat [memindahkan label](https://docs.microsoft.com/azure/information-protection/configure-policy-migrate-labels).
