---
title: Mengaktifkan autentikasi SMTP dan pemecahan masalah
ms.author: pebaum
author: pebaum
manager: scotv
ms.audience: Admin
ms.topic: article
ms.service: o365-administration
ROBOTS: NOINDEX, NOFOLLOW
localization_priority: Priority
ms.collection: Adm_O365
ms.custom:
- "3000003"
- "5652"
ms.openlocfilehash: f6f0228f6cdf7e07c9f439c54a7a2bd5364381c0e47dc80117bd964c5eafea61
ms.sourcegitcommit: b5f7da89a650d2915dc652449623c78be6247175
ms.translationtype: MT
ms.contentlocale: id-ID
ms.lasthandoff: 08/05/2021
ms.locfileid: "53957211"
---
# <a name="enable-smtp-authentication-and-troubleshooting"></a>Mengaktifkan autentikasi SMTP dan pemecahan masalah

Jika ingin mengaktifkan autentikasi SMTP untuk kotak surat atau mendapatkan kesalahan "Client not authenticated", "Authentication unsuccessful", atau "SmtpClientAuthentication" dengan kode 5.7.57 atau 5.7.3 atau 5.7.139 ketika mencoba melakukan relai email dengan mengautentikasi perangkat atau aplikasi dengan Microsoft 365, lakukan tiga tindakan ini untuk mengatasi masalah tersebut:

1. Nonaktifkan [default keamanan Azure](/azure/active-directory/fundamentals/concept-fundamentals-security-defaults) dengan mengaktifkan keamanan default **ke** **Tidak.**

    a. Masuk ke portal Azure sebagai administrator Keamanan, administrator Akses Kondisional, atau administrator global.<BR/>
    b. Telusuri ke Azure Active Directory > **Properti.**<BR/>
    c. Pilih **Kelola default keamanan.**<BR/>
    d. Atur **Aktifkan default keamanan ke** **Tidak.**<BR/>
    e. Pilih **Simpan**.

2. [Mengaktifkan pengiriman SMTP Klien](/exchange/clients-and-mobile-in-exchange-online/authenticated-client-smtp-submission#enable-smtp-auth-for-specific-mailboxes) pada kotak surat berlisensi.

    a. Dari pusat admin Microsoft 365, masuk ke **Pengguna Aktif**, lalu pilih pengguna.<BR/>
    b. Masuk ke tab Email, dan di **bawah Aplikasi email**, pilih Kelola aplikasi **email**.<BR/>
    d. Pastikan SMTP **Terautentikasi** dicentang (diaktifkan).<BR/>
    e. Pilih **Simpan perubahan.**<BR/>

3. [Menonaktifkan Multi-Factor Authentication (MFA) pada](/microsoft-365/admin/security-and-compliance/set-up-multi-factor-authentication#turn-off-legacy-per-user-mfa) kotak surat berlisensi.

    a. Masuk ke pusat admin Microsoft 365, dan di menu navigasi kiri, pilih **Pengguna**  >  **Aktif pengguna**.<BR/>
    b. Pilih **Multi-factor authentication**.<BR/>
    c. Pilih pengguna dan nonaktifkan **Multi-Factor auth**.<BR/>
