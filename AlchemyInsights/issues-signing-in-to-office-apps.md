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
- "2560"
ms.openlocfilehash: 8065a49c42953013ccfae9c5c1714d10ee0b4d49
ms.sourcegitcommit: 8bc60ec34bc1e40685e3976576e04a2623f63a7c
ms.translationtype: MT
ms.contentlocale: id-ID
ms.lasthandoff: 04/15/2021
ms.locfileid: "51833078"
---
# <a name="fixing-the-microsoft-365-apps-sorry-another-account-from-your-organization-is-already-signed-in-message"></a>Memperbaiki pesan "Maaf, akun lain dari organisasi Anda telah masuk" aplikasi Microsoft 365

Untuk memperbaiki kesalahan ini, coba hal berikut ini:

- Hapus semua akun kerja, kecuali akun yang terpengaruh, menggunakan Pengaturan Windows > **Kerja atau sekolah Access.**
- [Hapus kredensial Office menggunakan](https://docs.microsoft.com/office/troubleshoot/error-messages/another-account-already-signed-in#step-3-clear-cached-credentials-on-the-computer) Pengelola Kredensial Windows.<br/>
    **Catatan:** Jalur registri untuk Office 2016 telah berubah menjadi 16.0. (misalnya: \Software\Microsoft\Office\16.0\Common\Identity\)
- Buka aplikasi Office, pilih **Keluar**  >  **Akun**  >  File. Kemudian masuk menggunakan akun pengguna dengan lisensi yang valid. Untuk informasi mendetail, lihat [ akun di Office ](https://support.office.com/article/accounts-in-office-628ea040-f265-49de-b986-be09c3ebf8a9).
- Untuk Mac, lihat [Tidak dapat masuk ke aplikasi Office 2016 untuk aplikasi Mac ](https://docs.microsoft.com/office365/troubleshoot/authentication/sign-in-to-office-2016-for-mac-fail).

Untuk informasi selengkapnya, [lihat "Maaf, akun lain dari organisasi Anda sudah masuk di komputer ini" di Office](https://docs.microsoft.com/office/troubleshoot/error-messages/another-account-already-signed-in).