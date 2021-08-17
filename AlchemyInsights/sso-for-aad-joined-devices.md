---
title: Single-Sign yang tersedia untuk Azure Active Directory yang sudah bergabung
ms.author: v-aiyengar
author: AshaIyengar21
manager: dansimp
ms.date: 03/24/2021
ms.audience: Admin
ms.topic: article
ms.service: o365-administration
ROBOTS: NOINDEX, NOFOLLOW
localization_priority: Normal
ms.collection: Adm_O365
ms.custom:
- "9003257"
- "9891"
ms.openlocfilehash: 365225926296677feb7853481651a634792fd8bfa9abd9dc9359ffaae50b60eb
ms.sourcegitcommit: b5f7da89a650d2915dc652449623c78be6247175
ms.translationtype: MT
ms.contentlocale: id-ID
ms.lasthandoff: 08/05/2021
ms.locfileid: "54050013"
---
# <a name="single-sign-on-for-azure-active-directory-joined-devices"></a>Masuk tunggal untuk Azure Active Directory Bersama

Jika memiliki lingkungan Direktori Aktif (AD) lokal dan ingin menggabungkan komputer gabungan domain AD ke Azure AD, Anda dapat melakukannya dengan melakukan gabungan hibrid Azure AD. [Cara Untuk: Merencanakan penerapan penerapan Azure Active Directory hibrid](https://docs.microsoft.com/azure/active-directory/devices/hybrid-azuread-join-plan) akan memberi Anda langkah-langkah terkait untuk menerapkan gabungan Azure AD hibrid di lingkungan Anda.

[Mengonfigurasi perangkat yang tergabung di Azure AD untuk Single-Sign Aktif menggunakan Windows Hello for Business](https://docs.microsoft.com/azure/active-directory/devices/hybrid-azuread-join-plan) 

**Masalah Token Refresh Utama (PRT, Primary Refresh Token)** Token Refresh Utama (PRT) adalah artifak kunci autentikasi Azure AD di perangkat Windows 10, Windows Server 2016 dan versi yang lebih baru, iOS, dan Android. Cara ini adalah JSON Web Token (JWT) yang diterbitkan secara khusus untuk oelar token pihak pertama Microsoft untuk mengaktifkan akses masuk tunggal (SSO) di seluruh aplikasi yang digunakan di perangkat tersebut. [Dalam Apa itu Token Refresh Utama?](https://docs.microsoft.com/azure/active-directory/devices/concept-primary-refresh-token), kami akan menyediakan detail tentang bagaimana PRT diterbitkan, digunakan, dan dilindungi di Windows 10 saya.

**WamDefaultSet: YES dan AzureADPrt: YES** Bidang-bidang ini menunjukkan apakah pengguna telah berhasil diautentikasi ke Azure AD ketika masuk ke perangkat. Jika nilai bukan **,** hal ini mungkin disebabkan:

- Bad storage key in the TPM associated with the device upon registration (check the KeySignTest while running elevated).
- ID Masuk Alternatif
- Proksi HTTP tidak ditemukan

Memecahkan masalah perangkat yang menggunakan perintah dsregcmd - [status SSO](https://docs.microsoft.com/azure/active-directory/devices/troubleshoot-device-dsregcmd#sso-state)
