---
title: Masalah masuk ke aplikasi Microsoft 365
ms.author: pebaum
author: pebaum
manager: mnirkhe
ms.audience: Admin
ms.topic: article
ms.service: o365-administration
ROBOTS: NOINDEX, NOFOLLOW
localization_priority: Normal
ms.collection: Adm_O365
ms.custom:
- "9000571"
- "2559"
ms.openlocfilehash: d736c6c687695824f0ab37b8ffdc8456065353b0
ms.sourcegitcommit: 0eb4f9bde53395b5fd4b5cd4ffc56ca96db91298
ms.translationtype: MT
ms.contentlocale: id-ID
ms.lasthandoff: 03/10/2021
ms.locfileid: "50709109"
---
# <a name="fixing-the-microsoft-365-apps-your-computers-trusted-platform-module-is-not-functioning-properly-message"></a>Memperbaiki aplikasi Microsoft 365 "modul platform tepercaya komputer Anda tidak berfungsi dengan benar"

Untuk memperbaiki kesalahan ini, coba hal berikut ini:

- Instal pembaruan terbaru untuk [Windows](https://support.microsoft.com/help/4027667/windows-10-update) dan [Office](https://support.office.com/article/update-office-and-your-computer-with-microsoft-update-2ab296f3-7f03-43a2-8e50-46de917611c5).
- [Kosongkan kredensial Office](https://docs.microsoft.com/office/troubleshoot/office-suite-issues/another-account-already-signed-in#step-4-clear-cached-credentials-on-the-computer) menggunakan Pengelola kredensial Windows.<br/>
    **Catatan:** Jalur registri untuk Office 2016 telah diubah ke 16,0. (Mis: \Software\Microsoft\Office\16.0\Common\Identity\)
- Cobalah [proses pemulihan pengguna](https://docs.microsoft.com/office365/troubleshoot/administration/connection-issue-when-sign-in-office-2016#symptom-2) untuk memperbaiki kegagalan Trusted platform Module (TPM).
- Atur EnableADAL = 0 menggunakan langkah-langkah berikut:  
    1. Klik kanan tombol mulai Windows, pilih **Jalankan**, ketik **regedit**, lalu pilih **OK**.
    2. Pilih **ya** untuk memperbolehkan editor registri membuat perubahan pada perangkat Anda.
    3. Dalam editor registri, tambahkan nilai DWORD **Enableadal** dengan pengaturan **0** di bawah HKEY_CURRENT_USER\Software\Microsoft\Office\16.0\Common\Identity.

Untuk informasi selengkapnya, lihat [masalah koneksi di masuk setelah pembaruan ke Office 2016 Build 16.0.7967 di Windows 10](https://docs.microsoft.com/office365/troubleshoot/administration/connection-issue-when-sign-in-office-2016).