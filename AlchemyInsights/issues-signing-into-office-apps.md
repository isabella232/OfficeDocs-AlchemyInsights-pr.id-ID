---
title: Masalah saat masuk ke aplikasi Microsoft 365
ms.author: pebaum
author: pebaum
manager: mnirkhe
ms.audience: Admin
ms.topic: article
ROBOTS: NOINDEX, NOFOLLOW
localization_priority: Normal
ms.collection: Adm_O365
ms.custom:
- "9000571"
- "2559"
ms.openlocfilehash: 4e7612562d036f1c717817d3c883d6df80f86e2f
ms.sourcegitcommit: f28dafa0f727870038f72bc904da926daf4ec07b
ms.translationtype: MT
ms.contentlocale: id-ID
ms.lasthandoff: 06/05/2020
ms.locfileid: "44579868"
---
# <a name="fixing-the-microsoft-365-apps-your-computers-trusted-platform-module-is-not-functioning-properly-message"></a>Memperbaiki aplikasi Microsoft 365 "komputer Anda terpercaya platform modul tidak berfungsi dengan benar" pesan

Untuk memperbaiki kesalahan ini, coba hal berikut ini:

- Instal pemutakhiran terbaru untuk [Windows](https://support.microsoft.com/help/4027667/windows-10-update) dan [Office](https://support.office.com/article/update-office-and-your-computer-with-microsoft-update-2ab296f3-7f03-43a2-8e50-46de917611c5).
- [Hapus kredensial Office](https://docs.microsoft.com/eoffice/troubleshoot/error-messages/another-account-already-signed-in#step-3-clear-cached-credentials-on-the-computer) yang menggunakan Pengelola mandat Windows.<br/>
    **Catatan:** Lintasan registri untuk Office 2016 telah diubah ke 16,0. (Mis: \Software\Microsoft\Office\16.0\Common\Identity\)
- Cobalah [proses pemulihan pengguna](https://docs.microsoft.com/office365/troubleshoot/administration/connection-issue-when-sign-in-office-2016#symptom-2) untuk memperbaiki kegagalan Trusted platform Module (TPM).
- Tetapkan EnableADAL = 0 dengan menggunakan langkah berikut:  
    1. Klik kanan tombol mulai Windows, pilih **Jalankan**, ketik **regedit**, dan kemudian pilih **OK**.
    2. Pilih **ya** untuk membolehkan Penyunting registri untuk membuat perubahan pada perangkat Anda.
    3. Di Penyunting registri, tambahkan nilai DWORD **Enableadal** dengan pengaturan **0** di bawah HKEY_CURRENT_USER \Software\Microsoft\Office\16.0\Common\Identity.

Untuk informasi selengkapnya, lihat [masalah sambungan di masuk setelah pembaruan ke Office 2016 membangun 16.0.7967 di Windows 10](https://docs.microsoft.com/office365/troubleshoot/administration/connection-issue-when-sign-in-office-2016).