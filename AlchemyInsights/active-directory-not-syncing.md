---
title: Direktori Aktif tidak tersinkron
ms.author: pebaum
author: pebaum
manager: scotv
ms.audience: Admin
ms.topic: article
ms.service: o365-administration
ROBOTS: NOINDEX, NOFOLLOW
localization_priority: Normal
ms.collection: Adm_O365
ms.custom:
- "9001688"
- "1300023"
- "3754"
- "4531"
ms.openlocfilehash: 0da512379e5a2f6ccb773e18c465e545c0660560
ms.sourcegitcommit: e42bb24c9bae1d0df8c49c424d2aa5e7466703ac
ms.translationtype: MT
ms.contentlocale: id-ID
ms.lasthandoff: 06/14/2021
ms.locfileid: "52930978"
---
# <a name="active-directory-not-syncing"></a>Direktori Aktif tidak tersinkron

Jika Menerima kesalahan sinkronisasi, seperti "tidak ada sinkronisasi terbaru", atau pemberitahuan status sinkronisasi direktori di portal admin Office mengatakan, "Terakhir disinkronkan lebih dari 3 hari yang lalu," mungkin AADConnect memiliki pengaturan yang salah atau izin tidak cukup untuk melakukan sinkronisasi.  

Menginstal ulang AADConnect menggunakan pengaturan ekspres dapat mengatasi masalah dengan cepat:

1. [Unduh versi terbaru AADConnect.](https://go.microsoft.com/fwlink/?LinkId=615771)

2. [Ikuti instruksi untuk penginstalan ekspres.](/azure/active-directory/hybrid/how-to-connect-install-express)

Azure AD Connect harus diinstal di Windows Server 2012 atau yang lebih baru. Server ini harus berupa domain bersama dan juga pengontrol domain atau server member. Untuk daftar lengkap persyaratan Koneksi Azure AD dan prasyarat, tinjau Prasyarat [untuk Azure AD Koneksi](/azure/active-directory/hybrid/how-to-connect-install-prerequisites).

Untuk informasi selengkapnya tentang akun layanan AADConnect, lihat [Azure AD Koneksi: Akun dan izin](/azure/active-directory/hybrid/reference-connect-accounts-permissions).
