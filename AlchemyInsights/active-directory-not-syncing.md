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
ms.openlocfilehash: d4615d335b9aeef69148cd93ff9f44bec6d7d876
ms.sourcegitcommit: ab75f66355116e995b3cb5505465b31989339e28
ms.translationtype: MT
ms.contentlocale: id-ID
ms.lasthandoff: 08/13/2021
ms.locfileid: "58314207"
---
# <a name="active-directory-not-syncing"></a>Direktori Aktif tidak tersinkron

Jika Anda menerima kesalahan sinkronisasi, seperti "tidak ada sinkronisasi terbaru," atau pemberitahuan status sinkronisasi direktori di portal admin Office mengatakan, "Terakhir disinkronkan lebih dari 3 hari yang lalu," mungkin AADConnect memiliki pengaturan yang salah atau izin tidak cukup untuk melakukan sinkronisasi.  

Menginstal ulang AADConnect menggunakan pengaturan ekspres dapat mengatasi masalah dengan cepat:

1. [Unduh versi terbaru AADConnect.](https://go.microsoft.com/fwlink/?LinkId=615771)

2. [Ikuti instruksi untuk penginstalan ekspres.](https://docs.microsoft.com/azure/active-directory/hybrid/how-to-connect-install-express)

Azure AD Connect harus diinstal di Windows Server 2012 atau yang lebih baru. Server ini harus berupa domain bersama dan juga pengontrol domain atau server member. Untuk daftar lengkap Persyaratan Koneksi Azure AD dan prasyarat, tinjau Prasyarat [untuk Azure AD Koneksi](https://docs.microsoft.com/azure/active-directory/hybrid/how-to-connect-install-prerequisites).

Untuk informasi selengkapnya tentang akun layanan AADConnect, lihat [Azure AD Koneksi: Akun dan izin](https://docs.microsoft.com/azure/active-directory/hybrid/reference-connect-accounts-permissions).
