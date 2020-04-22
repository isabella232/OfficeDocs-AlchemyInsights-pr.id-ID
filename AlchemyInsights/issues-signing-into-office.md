---
title: Masalah saat masuk ke aplikasi Office
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
- "2574"
ms.openlocfilehash: 695d449a876c22ff441da2367ef67aaea470eb66
ms.sourcegitcommit: 631cbb5f03e5371f0995e976536d24e9d13746c3
ms.translationtype: MT
ms.contentlocale: id-ID
ms.lasthandoff: 04/22/2020
ms.locfileid: "43763004"
---
# <a name="issues-signing-in-to-office-apps"></a>Masalah saat masuk ke aplikasi Office

Untuk memperbaiki masalah masuk dengan aplikasi Office, coba hal berikut:

- Hapus semua akun kerja, kecuali akun yang terpengaruh, menggunakan pengaturan Windows > **akses kerja atau sekolah**.
- [Hapus kredensial Office](https://docs.microsoft.com/office/troubleshoot/error-messages/another-account-already-signed-in#step-3-clear-cached-credentials-on-the-computer) yang menggunakan Pengelola mandat Windows.<br/>
    **Catatan:** Lintasan registri untuk Office 2016 telah diubah ke 16,0. (Mis: \Software\Microsoft\Office\16.0\Common\Identity\)
- Buka aplikasi Office, pilih keluar **File** > **Account** > **dari**akun file. Kemudian masuk menggunakan akun pengguna dengan lisensi yang valid. Untuk informasi mendetail, lihat [ akun di Office ](https://support.office.com/article/accounts-in-office-628ea040-f265-49de-b986-be09c3ebf8a9).
- Untuk Mac, lihat [Tidak dapat masuk ke aplikasi Office 2016 untuk aplikasi Mac ](https://docs.microsoft.com/office365/troubleshoot/authentication/sign-in-to-office-2016-for-mac-fail).
- Jika kesalahan terjadi saat menyambung ke Microsoft 365 menggunakan Office 2013, aktifkan otentikasi modern untuk klien Office.

Untuk informasi selengkapnya, lihat:
- [Anda tidak dapat masuk ke Microsoft 365, Azure, atau Intune](https://docs.microsoft.com/office365/troubleshoot/authentication/sign-in-to-office-365-azure-intune)
- [Masalah sambungan masuk setelah pembaruan untuk Office 2016 membangun 16.0.7967 di Windows 10](https://docs.microsoft.com/office365/troubleshoot/administration/connection-issue-when-sign-in-office-2016)
- ["Maaf, akun lain dari organisasi Anda sudah masuk di komputer ini" di Office](https://docs.microsoft.com/office/troubleshoot/error-messages/another-account-already-signed-in)
- [Memecahkan masalah masuk dengan otentikasi modern Office ketika Anda menggunakan ADFS](https://docs.microsoft.com/office365/troubleshoot/authentication/sign-in-issue-with-modern-auth)