---
title: Teams add-in untuk Mac
ms.author: pebaum
author: pebaum
manager: scotv
ms.date: 08/10/2020
ms.audience: Admin
ms.topic: article
ms.service: o365-administration
ROBOTS: NOINDEX, NOFOLLOW
localization_priority: Priority
ms.collection: Adm_O365
ms.custom:
- "6173"
- "6166"
- "9003233"
- "9002573"
ms.openlocfilehash: c9c4eb811c93f6d11ebf606ba4bd20cddc2901d6616700ebfe6ef597dd8dc006
ms.sourcegitcommit: b5f7da89a650d2915dc652449623c78be6247175
ms.translationtype: MT
ms.contentlocale: id-ID
ms.lasthandoff: 08/05/2021
ms.locfileid: "53940678"
---
# <a name="teams-add-in-for-mac"></a>Teams add-in untuk Mac

Untuk memecahkan masalah add-in Teams yang hilang untuk pengguna sistem operasi Mac, ikuti langkah-langkah ini:

**Langkah 1:** Jika Anda memiliki Hybrid Exchange On-Premises (2016 CU3 atau yang lebih baru diperlukan), gunakan alat Test-HMA.ps1 untuk mengonfirmasi bahwa Autentikasi Modern Hibrid telah dikonfigurasi dengan benar. Untuk informasi selengkapnya, lihat [Memvalidasi penyiapan Autentikasi Modern Hibrid untuk Outlook untuk iOS dan Android.](https://aka.ms/TestHMAEAS)  

**Catatan** Gunakan format alamat UPN (misalnya, username@contoso.com ), [bukan](mailto:username@contoso.com)domain \namapengguna. Lakukan hal ini bahkan untuk pengguna dengan Exchange Online surat.

**Langkah 2:** Miliki pengguna untuk masuk ke **Akun**  >  **Alat**... di Outlook untuk Mac, dan temukan dan pilih akun tersebut. Konfirmasi nama pengguna yang tercantum berada dalam format UPN (misalnya, [username@contoso.com](mailto:username@contoso.com)).

**Langkah 3:** Konfirmasi bahwa pengguna berlisensi Microsoft Teams. Pengguna harus menggunakan langganan Office 365 untuk Mac, produk versi 16.24 atau lebih baru.