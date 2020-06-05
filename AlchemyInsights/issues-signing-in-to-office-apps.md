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
- "2560"
ms.openlocfilehash: e4f2fea5c2f368ae240614ee1f7bc729338dd75d
ms.sourcegitcommit: f28dafa0f727870038f72bc904da926daf4ec07b
ms.translationtype: MT
ms.contentlocale: id-ID
ms.lasthandoff: 06/05/2020
ms.locfileid: "44579940"
---
# <a name="fixing-the-microsoft-365-apps-sorry-another-account-from-your-organization-is-already-signed-in-message"></a>Memperbaiki aplikasi Microsoft 365 "Maaf, akun lain dari organisasi Anda sudah masuk" pesan

Untuk memperbaiki kesalahan ini, coba hal berikut ini:

- Hapus semua akun kerja, kecuali akun yang terpengaruh, menggunakan pengaturan Windows > **akses kerja atau sekolah**.
- [Hapus kredensial Office](https://docs.microsoft.com/office/troubleshoot/error-messages/another-account-already-signed-in#step-3-clear-cached-credentials-on-the-computer) yang menggunakan Pengelola mandat Windows.<br/>
    **Catatan:** Lintasan registri untuk Office 2016 telah diubah ke 16,0. (Mis: \Software\Microsoft\Office\16.0\Common\Identity\)
- Buka aplikasi Office, pilih keluar **File**  >  **Account**  >  **dari**akun file. Kemudian masuk menggunakan akun pengguna dengan lisensi yang valid. Untuk informasi mendetail, lihat [ akun di Office ](https://support.office.com/article/accounts-in-office-628ea040-f265-49de-b986-be09c3ebf8a9).
- Untuk Mac, lihat [Tidak dapat masuk ke aplikasi Office 2016 untuk aplikasi Mac ](https://docs.microsoft.com/office365/troubleshoot/authentication/sign-in-to-office-2016-for-mac-fail).

Untuk informasi selengkapnya, lihat ["Maaf, akun lain dari organisasi Anda telah masuk di komputer ini" di Office](https://docs.microsoft.com/office/troubleshoot/error-messages/another-account-already-signed-in).