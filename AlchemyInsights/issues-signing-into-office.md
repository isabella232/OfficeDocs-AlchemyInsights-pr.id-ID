---
title: Masalah masuk ke Microsoft 365 aplikasi
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
- "9000571"
- "2574"
ms.openlocfilehash: f8f2824cc4a575ab7d7c9adec5b75e5955ec9fb5
ms.sourcegitcommit: b6dd6ae628a02ea6b997a993c49de083465bc2ac
ms.translationtype: MT
ms.contentlocale: id-ID
ms.lasthandoff: 08/30/2021
ms.locfileid: "58744649"
---
# <a name="issues-signing-into-microsoft-365-apps"></a>Masalah masuk ke Aplikasi Microsoft 365

Catatan: Jika Anda menggunakan versi Windows yang lebih lama (misalnya Windows 7 SP1, Windows Server 2008 R2), gunakan perbaikan mudah untuk mengaktifkan TLS 1.2 sebagai default. [](https://download.microsoft.com/download/0/6/5/0658B1A7-6D2E-474F-BC2C-D69E5B9E9A68/MicrosoftEasyFix51044.msi) Untuk informasi selengkapnya, lihat Pembaruan untuk mengaktifkan [TLS 1.1 dan TLS 1.2](https://support.microsoft.com/topic/update-to-enable-tls-1-1-and-tls-1-2-as-default-secure-protocols-in-winhttp-in-windows-c4bd73d2-31d7-761e-0178-11268bb10392)sebagai protokol aman default di WinHTTP Windows .

Untuk mengatasi masalah masuk aplikasi Microsoft 365, cobalah opsi berikut di komputer yang terpengaruh:  

- Untuk Windows, lihat [Rekomendasi mengatasi masalah masuk umum](https://docs.microsoft.com/office365/troubleshoot/administration/disabling-adal-wam-not-recommended#recommendations-on-resolving-common-sign-in-issues)
- Untuk Mac, [lihat Tidak dapat masuk ke aplikasi Office 2016 untuk Mac Anda](https://docs.microsoft.com/office365/troubleshoot/authentication/sign-in-to-office-2016-for-mac-fail)

**Tips** Di komputer Windows, kami dapat mendiagnosis dan otomatis memperbaiki beberapa masalah masuk Office yang umum untuk Anda. Unduh dan jalankan  **[Asisten Dukungan dan Pemulihan Microsoft](https://aka.ms/SaRA-OfficeSignInScenario)** untuk menggunakan alat otomatis kami.

**Catatan:** Menonaktifkan Autentikasi Modern (ADAL) atau Manajemen Akun Web (WAM, Web Account Management) untuk memperbaiki masalah masuk atau **aktivasi tidak disarankan.** Jika kesalahan terjadi saat menyambungkan ke Microsoft 365 menggunakan Office 2013, pastikan bahwa Anda mengaktifkan autentikasi [modern](https://docs.microsoft.com/microsoft-365/admin/security-and-compliance/enable-modern-authentication) untuk Office klien.

Untuk tindakan pemecahan masalah spesifik, lihat:

[Masalah koneksi masuk setelah pembaruan ke Office 2016 build 16.0.7967 pada Windows 10](https://docs.microsoft.com/office365/troubleshoot/administration/connection-issue-when-sign-in-office-2016)  

[Anda tidak dapat masuk ke akun organisasi seperti akun Office 365 Azure, atau Intune](https://docs.microsoft.com/office365/troubleshoot/authentication/sign-in-to-office-365-azure-intune)

[Cara memecahkan masalah aplikasi non-browser yang tidak dapat masuk ke Office 365, Azure, atau Intune](https://support.office.com/article/how-to-troubleshoot-non-browser-apps-that-can-t-sign-in-to-office-365-azure-or-intune-3ba1b268-66f6-462c-b0e5-070f5c2603c1?ui=en-US&rs=en-US&ad=US)

[Berulang kali dimintai kredensial di Office](https://docs.microsoft.com/office365/troubleshoot/authentication/access-denied-when-connect-to-office-365)