---
title: Log kata sandi
ms.author: v-smandalika
author: v-smandalika
manager: dansimp
ms.date: 03/08/2021
audience: Admin
ms.topic: article
ms.service: o365-administration
ROBOTS: NOINDEX, NOFOLLOW
localization_priority: Priority
ms.collection: Adm_O365
ms.custom:
- "9361"
- "9003259"
ms.openlocfilehash: ed151b436fa2043c610931deeb74a202af88fcf4
ms.sourcegitcommit: 226fe97678b6be215eda0c278399f8be9be525c1
ms.translationtype: MT
ms.contentlocale: id-ID
ms.lasthandoff: 03/08/2021
ms.locfileid: "50527184"
---
# <a name="password-logs"></a>Log kata sandi

**Saya mengalami masalah saat mengakses log audit penyetelan ulang kata sandi**

Untuk memecahkan masalah terkait akses ke log penyetelan ulang kata sandi, lakukan langkah berikut:

Pastikan Anda memiliki wewenang untuk melihat log audit. 

Hanya peran berikut yang diizinkan:
 - Administrator global
 - Administrator keamanan
 - Pembaca keamanan

**Saya ingin melihat semua kejadian ulang kata sandi mengaudit dari waktu yang saya gunakan pada awalnya**

Acara pengaturan ulang kata sandi hingga 120.000 disimpan dalam laporan 30 hari terakhir. Batas maksimal ini berlaku untuk UI saat mengunduh CSV. 1.000.000 acara tersedia melalui PowerShell.
Untuk informasi selengkapnya, lihat link di bawah ini:

- [Acara reset kata sandi layanan mandiri dari laporan Azure AD dan API kejadian](https://docs.microsoft.com/azure/active-directory/authentication/howto-sspr-reporting)
- [Cara mengunduh ulang kata sandi acara pendaftaran dengan cepat menggunakan PowerShell](https://docs.microsoft.com/azure/active-directory/authentication/howto-sspr-reporting)

**Saya ingin memahami kapabilitas pelaporan penyetelan ulang kata sandi**

Periksa siapa yang mendaftar atau mereset kata sandi dengan log reset kata sandi Azure AD audit di portal Azure di bawah **pengguna dan grup**.
Untuk informasi selengkapnya, lihat link berikut ini:

- [Gambaran umum laporan penyetelan ulang kata sandi](https://docs.microsoft.com/azure/active-directory/authentication/howto-sspr-reporting)
- [Cara menampilkan laporan penyetelan ulang kata sandi di portal Azure](https://docs.microsoft.com/azure/active-directory/authentication/howto-sspr-reporting)
- [Acara reset kata sandi layanan mandiri dari laporan Azure AD dan API kejadian](https://docs.microsoft.com/azure/active-directory/authentication/howto-sspr-reporting)
- [Cara mengunduh ulang kata sandi acara pendaftaran dengan cepat menggunakan PowerShell](https://docs.microsoft.com/azure/active-directory/authentication/howto-sspr-reporting)


