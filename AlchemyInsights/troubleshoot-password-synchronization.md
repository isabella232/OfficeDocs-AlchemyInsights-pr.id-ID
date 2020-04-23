---
title: Memecahkan masalah sinkronisasi sandi
ms.author: pebaum
author: pebaum
manager: mnirkhe
ms.date: 04/21/2020
ms.audience: Admin
ms.topic: article
ROBOTS: NOINDEX, NOFOLLOW
localization_priority: Normal
ms.collection: Adm_O365
ms.custom:
- "579"
- "1300006"
ms.assetid: 1cba32c4-37ce-4ec1-9e58-8d3440b53d57
ms.openlocfilehash: edd4f68466296f72c2dc0bafda45e6749d62d942
ms.sourcegitcommit: 631cbb5f03e5371f0995e976536d24e9d13746c3
ms.translationtype: MT
ms.contentlocale: id-ID
ms.lasthandoff: 04/22/2020
ms.locfileid: "43732513"
---
# <a name="troubleshoot-password-synchronization"></a>Memecahkan masalah sinkronisasi sandi

Untuk memecahkan masalah di mana sandi tidak disinkronkan dengan Azure AD menyambung versi 1.1.614.0 atau yang lebih baru:
  
1. Buka sesi Windows PowerShell baru di server Azure AD menyambung dengan opsi **Jalankan sebagai administrator** .

2. Jalankan **set-executionpolicy Remotesanye** atau **set-executionpolicy terbatas**.

3. Mulai Wisaya Azure AD menyambung.

4. Navigasikan ke halaman **tugas tambahan** , pilih **pemecahan masalah**, dan klik **berikutnya**.

5. Pada halaman pemecahan masalah, klik **Luncurkan untuk memulai menu pemecahan masalah** di PowerShell.

6. Di menu utama, pilih **memecahkan masalah sinkronisasi sandi**.

7. Di sub menu, pilih **Sinkronisasi sandi tidak berfungsi sama sekali**.

**Memahami hasil tugas pemecahan masalah**
  
Tugas pemecahan masalah melakukan pemeriksaan berikut ini:
  
- Memvalidasi bahwa fitur sinkronisasi sandi diaktifkan untuk penghuni Azure AD Anda.

- Memvalidasi bahwa server Azure AD menyambung bukan dalam mode pementasan.

- Untuk setiap konektor Active Directory lokal yang ada (yang sesuai dengan hutan direktori aktif yang ada):

- 
  - Memvalidasi fitur sinkronisasi sandi diaktifkan.

  - Mencari peristiwa heartbeat Sinkronisasi sandi di log peristiwa aplikasi Windows.

  - Untuk setiap domain direktori aktif di bawah konektor Active Directory lokal:

  - Memvalidasi domain dapat dicapai dari server Azure AD menyambung.

  - Memvalidasi account layanan domain direktori aktif (AD DS) yang digunakan oleh konektor Active Directory lokal memiliki nama pengguna yang benar, sandi, dan izin yang diperlukan untuk sinkronisasi sandi.

Untuk bantuan lebih lanjut pemecahan masalah sinkronisasi sandi, lihat [memecahkan masalah sinkronisasi sandi dengan AZURE AD menyambung sinkronisasi](https://docs.microsoft.com/azure/active-directory/connect/active-directory-aadconnectsync-troubleshoot-password-synchronization).
  