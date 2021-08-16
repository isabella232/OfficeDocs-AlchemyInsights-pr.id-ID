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
- "2560"
ms.openlocfilehash: 454000eafa6818f91e3c302cc69fbf252aae1107aa18904ac93a4756d4db642b
ms.sourcegitcommit: b5f7da89a650d2915dc652449623c78be6247175
ms.translationtype: MT
ms.contentlocale: id-ID
ms.lasthandoff: 08/05/2021
ms.locfileid: "54028043"
---
# <a name="fixing-the-microsoft-365-apps-sorry-another-account-from-your-organization-is-already-signed-in-message"></a>Memperbaiki aplikasi Microsoft 365 pesan "Maaf, akun lain dari organisasi Anda sudah masuk"

Untuk memperbaiki kesalahan ini, coba hal berikut ini:

- Hapus semua akun kerja, kecuali akun yang terpengaruh, menggunakan Windows Pengaturan > **Access kerja atau sekolah.**
- [Kosongkan Office kredensial](https://docs.microsoft.com/office/troubleshoot/error-messages/another-account-already-signed-in#step-3-clear-cached-credentials-on-the-computer) menggunakan Windows Manager Kredensial.<br/>
    **Catatan:** Jalur registri untuk Office 2016 telah berubah menjadi 16.0. (misalnya: \Software\Microsoft\Office\16.0\Common\Identity\)
- Buka buku aplikasi Office, pilih **Keluar**  >    >  **Akun** File. Kemudian masuk menggunakan akun pengguna dengan lisensi yang valid. Untuk informasi mendetail, lihat [ Akun di Office ](https://support.office.com/article/accounts-in-office-628ea040-f265-49de-b986-be09c3ebf8a9).
- Untuk Mac, lihat [Tidak dapat masuk ke aplikasi Office 2016 untuk aplikasi Mac ](https://docs.microsoft.com/office365/troubleshoot/authentication/sign-in-to-office-2016-for-mac-fail).

Untuk informasi selengkapnya, [lihat "Maaf, akun lain dari organisasi Anda sudah masuk di komputer ini" dalam Office](https://docs.microsoft.com/office/troubleshoot/error-messages/another-account-already-signed-in).