---
title: Masalah masuk ke Microsoft 365 baru
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
- "2559"
ms.openlocfilehash: b0789a54f48b2850c1dad8651a8209449c805784bea96799f05e67c4bc43fdb0
ms.sourcegitcommit: b5f7da89a650d2915dc652449623c78be6247175
ms.translationtype: MT
ms.contentlocale: id-ID
ms.lasthandoff: 08/05/2021
ms.locfileid: "53986894"
---
# <a name="fixing-the-microsoft-365-apps-your-computers-trusted-platform-module-is-not-functioning-properly-message"></a>Memperbaiki aplikasi Microsoft 365 pesan "Modul Platform Tepercaya komputer Anda tidak berfungsi dengan baik"

Untuk memperbaiki kesalahan ini, coba hal berikut ini:

- Instal pembaruan terkini untuk semua [Windows](https://support.microsoft.com/help/4027667/windows-10-update) lalu [Office](https://support.office.com/article/update-office-and-your-computer-with-microsoft-update-2ab296f3-7f03-43a2-8e50-46de917611c5).
- [Kosongkan Office kredensial](https://docs.microsoft.com/office/troubleshoot/office-suite-issues/another-account-already-signed-in#step-4-clear-cached-credentials-on-the-computer) menggunakan Windows Manager Kredensial.<br/>
    **Catatan:** Jalur registri untuk Office 2016 telah berubah menjadi 16.0. (misalnya: \Software\Microsoft\Office\16.0\Common\Identity\)
- Coba proses [pemulihan pengguna untuk](https://docs.microsoft.com/office365/troubleshoot/administration/connection-issue-when-sign-in-office-2016#symptom-2) memperbaiki kegagalan Trusted Platform Module (TPM).
- Atur EnableADAL = 0 menggunakan langkah-langkah berikut:  
    1. Klik kanan tombol Windows Mulai, pilih **Jalankan**, ketik **regedit**, lalu pilih **OK.**
    2. Pilih **Ya** untuk mengizinkan Editor Registri membuat perubahan ke perangkat Anda.
    3. Di Editor Registri, tambahkan nilai DWORD dari **EnableADAL** dengan pengaturan **0 di bawah** HKEY_CURRENT_USER\Software\Microsoft\Office\16.0\Common\Identity.

Untuk informasi selengkapnya, lihat Masalah koneksi masuk setelah pembaruan [ke Office 2016 build 16.0.7967 pada Windows 10](https://docs.microsoft.com/office365/troubleshoot/administration/connection-issue-when-sign-in-office-2016).