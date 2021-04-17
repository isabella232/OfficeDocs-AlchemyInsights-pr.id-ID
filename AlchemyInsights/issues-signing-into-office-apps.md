---
title: Masalah masuk ke aplikasi Microsoft 365
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
ms.openlocfilehash: c64cf2c9dbf63caad22e54ae801adc3ed8ff0f62
ms.sourcegitcommit: 8bc60ec34bc1e40685e3976576e04a2623f63a7c
ms.translationtype: MT
ms.contentlocale: id-ID
ms.lasthandoff: 04/15/2021
ms.locfileid: "51833006"
---
# <a name="fixing-the-microsoft-365-apps-your-computers-trusted-platform-module-is-not-functioning-properly-message"></a>Memperbaiki pesan "Modul Platform Tepercaya komputer Anda tidak berfungsi dengan baik" aplikasi Microsoft 365

Untuk memperbaiki kesalahan ini, coba hal berikut ini:

- Instal pembaruan terkini untuk [Windows](https://support.microsoft.com/help/4027667/windows-10-update) dan [Office.](https://support.office.com/article/update-office-and-your-computer-with-microsoft-update-2ab296f3-7f03-43a2-8e50-46de917611c5)
- [Hapus kredensial Office menggunakan](https://docs.microsoft.com/office/troubleshoot/office-suite-issues/another-account-already-signed-in#step-4-clear-cached-credentials-on-the-computer) Pengelola Kredensial Windows.<br/>
    **Catatan:** Jalur registri untuk Office 2016 telah berubah menjadi 16.0. (misalnya: \Software\Microsoft\Office\16.0\Common\Identity\)
- Coba proses [pemulihan pengguna untuk](https://docs.microsoft.com/office365/troubleshoot/administration/connection-issue-when-sign-in-office-2016#symptom-2) memperbaiki kegagalan Trusted Platform Module (TPM).
- Atur EnableADAL = 0 menggunakan langkah-langkah berikut:  
    1. Klik kanan tombol Mulai Windows, pilih **Jalankan**, ketik **regedit**, lalu pilih **OK.**
    2. Pilih **Ya** untuk mengizinkan Editor Registri membuat perubahan ke perangkat Anda.
    3. Di Editor Registri, tambahkan nilai DWORD dari **EnableADAL** dengan pengaturan **0 di bawah** HKEY_CURRENT_USER\Software\Microsoft\Office\16.0\Common\Identity.

Untuk informasi selengkapnya, lihat Masalah koneksi masuk setelah pembaruan ke [Office 2016 build 16.0.7967 di Windows 10](https://docs.microsoft.com/office365/troubleshoot/administration/connection-issue-when-sign-in-office-2016).