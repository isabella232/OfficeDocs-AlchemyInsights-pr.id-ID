---
title: Memecahkan masalah Masuk tunggal untuk Perangkat Yang Tergabung di Azure AD
ms.author: v-jmathew
author: v-jmathew
manager: scotv
audience: Admin
ms.topic: article
ms.service: o365-administration
ROBOTS: NOINDEX, NOFOLLOW
localization_priority: Normal
ms.collection: Adm_O365
ms.custom:
- "9003246"
- "9327"
ms.openlocfilehash: 872333e13bb51b3a22431154627ad561f6db88c681c9eeee523fdd09e58c0371
ms.sourcegitcommit: b5f7da89a650d2915dc652449623c78be6247175
ms.translationtype: MT
ms.contentlocale: id-ID
ms.lasthandoff: 08/05/2021
ms.locfileid: "54039249"
---
# <a name="troubleshoot-single-sign-on-for-azure-ad-joined-devices"></a>Memecahkan masalah Masuk tunggal untuk Perangkat Yang Tergabung di Azure AD

Jika memiliki lingkungan Direktori Aktif (AD) lokal dan ingin menggabungkan komputer gabungan domain AD ke Azure AD, Anda dapat melakukannya dengan melakukan gabungan hibrid Azure AD. [Cara Untuk: Merencanakan penerapan penerapan Azure Active Directory hibrid](https://docs.microsoft.com/azure/active-directory/devices/hybrid-azuread-join-plan) akan memberi Anda langkah-langkah terkait untuk menerapkan gabungan Azure AD hibrid di lingkungan Anda.

Untuk informasi selengkapnya, lihat Mengonfigurasi perangkat yang tergabung di Azure AD untuk [Layanan Single-Sign Lokal menggunakan Windows Hello for Business.](https://docs.microsoft.com/windows/security/identity-protection/hello-for-business/hello-hybrid-aadj-sso-base)

**Masalah Token Refresh Utama (PRT, Primary Refresh Token)**

Token Refresh Utama (PRT) adalah artifak kunci autentikasi Azure AD di perangkat Windows 10, Windows Server 2016 dan versi yang lebih baru, iOS, dan Android. Cara ini adalah JSON Web Token (JWT) yang diterbitkan secara khusus untuk oelar token pihak pertama Microsoft untuk mengaktifkan akses masuk tunggal (SSO) di seluruh aplikasi yang digunakan di perangkat tersebut. Untuk detail tentang bagaimana PRT diterbitkan, digunakan, dan dilindungi di Windows 10 saya, lihat [Apa itu Token Refresh Utama?](https://docs.microsoft.com/azure/active-directory/devices/concept-primary-refresh-token).

**WamDefaultSet: YES dan AzureADPrt: YES**

Bidang-bidang ini menunjukkan apakah pengguna telah berhasil diautentikasi ke Azure AD ketika masuk ke perangkat. Jika nilai bukan **,** hal ini mungkin disebabkan oleh:

- Bad storage key in the TPM associated with the device upon registration (check the KeySignTest while running elevated)
- ID Masuk Alternatif
- Proksi HTTP tidak ditemukan

Untuk memecahkan masalah perangkat menggunakan perintah dsregcmd, lihat [Status SSO](https://docs.microsoft.com/azure/active-directory/devices/troubleshoot-device-dsregcmd#sso-state).
