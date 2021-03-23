---
title: Memecahkan masalah masuk tunggal untuk perangkat yang bergabung dengan Azure AD
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
ms.openlocfilehash: d11c24719eb2db9e9fd87c158c80cec5cb75b946
ms.sourcegitcommit: c08bed4071baa3bb5879496df3ed44fb828c8367
ms.translationtype: MT
ms.contentlocale: id-ID
ms.lasthandoff: 03/19/2021
ms.locfileid: "51036172"
---
# <a name="troubleshoot-single-sign-on-for-azure-ad-joined-devices"></a>Memecahkan masalah masuk tunggal untuk perangkat yang bergabung dengan Azure AD

Jika Anda memiliki lingkungan direktori aktif (AD) di tempat dan Anda ingin bergabung dengan komputer yang tergabung dalam domain-domain ke Azure AD, Anda bisa mencapainya dengan melakukan gabungan Azure AD Exchange. [Cara: merencanakan penerapan hibrid Azure Active Directory gabungan](https://docs.microsoft.com/azure/active-directory/devices/hybrid-azuread-join-plan) memberi Anda langkah terkait untuk menerapkan gabungan Azure AD di lingkungan Anda.

Untuk informasi selengkapnya, lihat [mengonfigurasi perangkat yang bergabung dengan AZURE AD untuk Single-Sign di tempat untuk menggunakan Windows Hello for Business](https://docs.microsoft.com/windows/security/identity-protection/hello-for-business/hello-hybrid-aadj-sso-base).

**Masalah token refresh utama (PRT)**

Token refresh utama (PRT) adalah artefak kunci Azure AD Authentication pada Windows 10, Windows Server 2016 dan versi yang lebih baru, iOS, dan perangkat Android. Ini adalah JSON web Token (JWT) yang diterbitkan secara khusus untuk pialang Microsoft pihak pertama untuk mengaktifkan masuk tunggal (SSO) di seluruh aplikasi yang digunakan pada perangkat tersebut. Untuk detail tentang cara PRT dikeluarkan, digunakan, dan diproteksi pada perangkat Windows 10, lihat [apa itu token refresh utama?](https://docs.microsoft.com/azure/active-directory/devices/concept-primary-refresh-token).

**WamDefaultSet: Ya dan AzureADPrt: Ya**

Bidang ini menunjukkan apakah pengguna telah berhasil diautentikasi ke Azure AD saat masuk ke perangkat. Jika nilai **tidak**, itu mungkin karena:

- Kunci penyimpanan yang buruk dalam TPM yang terkait dengan perangkat saat pendaftaran (periksa tombol uji saat menjalankan peningkatan)
- ID masuk alternatif
- Proksi HTTP tidak ditemukan

Untuk memecahkan masalah perangkat menggunakan perintah dsregcmd, lihat [status SSO](https://docs.microsoft.com/azure/active-directory/devices/troubleshoot-device-dsregcmd#sso-state).
