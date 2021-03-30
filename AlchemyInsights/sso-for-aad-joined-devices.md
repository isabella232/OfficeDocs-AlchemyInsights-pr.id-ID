---
title: Single-Sign aktif untuk perangkat yang tergabung di Azure Active Directory
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
ms.openlocfilehash: f6426a3fb4addc24c5041196fe837134bf0d296b
ms.sourcegitcommit: db908b3da2c7a6508a77bf4f2c80afb294fadbd1
ms.translationtype: MT
ms.contentlocale: id-ID
ms.lasthandoff: 03/29/2021
ms.locfileid: "51405048"
---
# <a name="single-sign-on-for-azure-active-directory-joined-devices"></a>Akses tunggal untuk Perangkat Bergabung Azure Active Directory

Jika memiliki lingkungan Direktori Aktif (AD) lokal dan ingin menggabungkan komputer gabungan domain AD ke Azure AD, Anda dapat melakukannya dengan melakukan gabungan hibrid Azure AD. [Cara Untuk: Merencanakan penerapan gabungan Azure Active Directory](https://docs.microsoft.com/azure/active-directory/devices/hybrid-azuread-join-plan) hibrid akan memberi Anda langkah-langkah terkait untuk menerapkan gabungan Azure AD hibrid di lingkungan Anda.

[Mengonfigurasi perangkat yang bergabung di Azure AD untuk Perangkat Single-Sign Aktif menggunakan Windows Hello untuk Bisnis](https://docs.microsoft.com/azure/active-directory/devices/hybrid-azuread-join-plan) 

**Masalah Token Refresh Utama (PRT, Primary Refresh Token)** Token Refresh Utama (PRT) adalah artifak kunci autentikasi Azure AD di Windows 10, Windows Server 2016 dan versi yang lebih baru, perangkat iOS, dan Android. Cara ini adalah JSON Web Token (JWT) yang diterbitkan secara khusus untuk oelar token pihak pertama Microsoft untuk mengaktifkan akses masuk tunggal (SSO) di seluruh aplikasi yang digunakan di perangkat tersebut. [Dalam Apa itu Token Refresh Utama?](https://docs.microsoft.com/azure/active-directory/devices/concept-primary-refresh-token), kami akan menyediakan detail tentang bagaimana PRT diterbitkan, digunakan, dan dilindungi di perangkat Windows 10.

**WamDefaultSet: YES dan AzureADPrt: YES** Bidang-bidang ini menunjukkan apakah pengguna telah berhasil diautentikasi ke Azure AD ketika masuk ke perangkat. Jika nilai bukan **,** hal ini mungkin disebabkan:

- Bad storage key in the TPM associated with the device upon registration (check the KeySignTest while running elevated).
- ID Masuk Alternatif
- Proksi HTTP tidak ditemukan

Memecahkan masalah perangkat yang menggunakan perintah dsregcmd - [status SSO](https://docs.microsoft.com/azure/active-directory/devices/troubleshoot-device-dsregcmd#sso-state)
