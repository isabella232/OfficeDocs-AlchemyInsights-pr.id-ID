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
ms.openlocfilehash: 14f1454ad687b4d76cf419583b442685fa19b5a2
ms.sourcegitcommit: ab75f66355116e995b3cb5505465b31989339e28
ms.translationtype: MT
ms.contentlocale: id-ID
ms.lasthandoff: 08/13/2021
ms.locfileid: "58321756"
---
# <a name="enable-smtp-authentication-and-troubleshooting"></a>Mengaktifkan autentikasi SMTP dan pemecahan masalah

Jika ingin mengaktifkan autentikasi SMTP untuk kotak surat atau mendapatkan kesalahan "Client not authenticated", "Authentication unsuccessful", atau "SmtpClientAuthentication" dengan kode 5.7.57 atau 5.7.3 atau 5.7.139 ketika mencoba melakukan relai email dengan mengautentikasi perangkat atau aplikasi dengan Microsoft 365, lakukan tiga tindakan ini untuk mengatasi masalah tersebut:

1. Nonaktifkan [default keamanan Azure](https://docs.microsoft.com/azure/active-directory/fundamentals/concept-fundamentals-security-defaults) dengan mengaktifkan keamanan default **ke** **Tidak**.

    a. Masuk ke portal Azure sebagai administrator Keamanan, administrator Akses Kondisional, atau administrator global.<BR/>
    b. Telusuri ke Azure Active Directory > **Properti.**<BR/>
    c. Pilih **Kelola default keamanan.**<BR/>
    d. Atur **Aktifkan default keamanan ke** **Tidak.**<BR/>
    e. Pilih **Simpan**.

2. [Mengaktifkan pengiriman SMTP Klien](https://docs.microsoft.com/exchange/clients-and-mobile-in-exchange-online/authenticated-client-smtp-submission#enable-smtp-auth-for-specific-mailboxes) pada kotak surat berlisensi.

    a. Dari pusat admin Microsoft 365, masuk ke **Pengguna Aktif**, lalu pilih pengguna.<BR/>
    b. Masuk ke tab Email, dan di **bawah Aplikasi email**, pilih Kelola aplikasi **email**.<BR/>
    d. Pastikan SMTP **Terautentikasi** dicentang (diaktifkan).<BR/>
    e. Pilih **Simpan perubahan.**<BR/>

3. [Menonaktifkan Multi-Factor Authentication (MFA) pada](https://docs.microsoft.com/microsoft-365/admin/security-and-compliance/set-up-multi-factor-authentication#turn-off-legacy-per-user-mfa) kotak surat berlisensi.

    a. Masuk ke pusat admin Microsoft 365, dan di menu navigasi kiri, pilih **Pengguna**  >  **Aktif pengguna**.<BR/>
    b. Pilih **Multi-factor authentication**.<BR/>
    c. Pilih pengguna dan nonaktifkan **Multi-Factor auth**.<BR/>
