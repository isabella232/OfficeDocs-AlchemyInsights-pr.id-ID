---
title: Masalah menggunakan konsol admin Intune
ms.author: pebaum
author: pebaum
manager: scotv
ms.date: 07/29/2020
ms.audience: Admin
ms.topic: article
ROBOTS: NOINDEX, NOFOLLOW
localization_priority: Priority
ms.collection: Adm_O365
ms.custom:
- "1790"
- "9000214"
ms.openlocfilehash: 7a36d502a92d360b06336ccfa6183f666f0260ab
ms.sourcegitcommit: ffbed67c0a16ec423fa1d79b71e48ea4e2d320e1
ms.translationtype: MT
ms.contentlocale: id-ID
ms.lasthandoff: 07/29/2020
ms.locfileid: "46555384"
---
# <a name="problems-using-the-intune-admin-console"></a>Masalah menggunakan konsol admin Intune

**"Akses ditolak" saat menavigasi portal admin Intune.**

- Jika Anda adalah anggota dari peran kustom Intune, pastikan bahwa Intune atau Enterprise Mobility Suite (EMS) lisensi ditetapkan ke akun Anda.
- Jika Anda menggunakan Manajer konfigurasi untuk mengelola perangkat, verifikasi Anda bukan bagian dari koleksi pengguna Intune untuk manajer konfigurasi MDM.
- Verifikasi bahwa Anda telah ditetapkan sesuai peran berbasis administrasi kontrol (RBAC) izin dalam bilah peran Intune.
- Verifikasi grup yang digunakan bukanlah daftar distribusi. Intune di portal Azure hanya mendukung akun pengguna yang menjadi bagian dari grup keamanan Azure Active Directory. Tinjau grup Anda di Azure portal > **Intune**  >  **grup**, atau Azure portal > **Azure Active Directory**.

**Pengguna memiliki terlalu banyak izin untuk ditetapkan Intune peran**

Menyarankan pengguna untuk pergi ke **Intune**  >  **Intune peran**  >  **izin saya**  >  **ekspor** untuk meninjau diberikan izin.

**Saya menambahkan grup lingkup ke peran, namun pengguna dalam peran tersebut masih melihat pengguna atau perangkat lain.**

Grup lingkup tidak menyaring pengguna atau perangkat. Kelompok lingkup:

- Batasi pengguna yang dapat menetapkan kebijakan atau aplikasi.
- Izinkan hanya pengguna tertentu untuk menjalankan tugas jarak jauh di perangkat.

Untuk informasi selengkapnya tentang grup lingkup, lihat [kontrol akses berbasis peran (RBAC) dengan Microsoft Intune](https://docs.microsoft.com/intune/role-based-access-control).

**Saya menambahkan pengguna ke peran Intune tetapi mereka masih memiliki akses penuh ke konsol admin Intune.**

Arahkan ke Intune > **pengguna** di Azure portal dan verifikasi bahwa pengguna tidak ditetapkan ke salah satu peran berikut ini di Azure Portal:

- Administrator global
- Intune Layanan administrator
- Administrator SharePoint

Untuk informasi lebih lanjut, lihat [kontrol akses berbasis peran (RBAC) dengan Microsoft Intune](https://docs.microsoft.com/intune/role-based-access-control).

**Masalah akses**

Untuk informasi lebih lanjut, lihat [Anda tidak dapat masuk ke Office 365, Azure, atau Intune](https://support.microsoft.com/help/2412085/you-can-t-sign-in-to-office-365-azure-or-intune).