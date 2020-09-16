---
title: Memperbaiki aplikasi Microsoft 365 akun Anda dalam pesan status buruk
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
- "2558"
- "9000571"
ms.openlocfilehash: ec529291ec9406eba9dc2b0f2cc7a93c77fa3456
ms.sourcegitcommit: c6692ce0fa1358ec3529e59ca0ecdfdea4cdc759
ms.translationtype: MT
ms.contentlocale: id-ID
ms.lasthandoff: 09/14/2020
ms.locfileid: "47744548"
---
# <a name="fixing-the-microsoft-365-apps-your-account-is-in-a-bad-state-error"></a>Memperbaiki kesalahan aplikasi Microsoft 365 "akun Anda dalam keadaan yang tidak baik"

Untuk memperbaiki kesalahan ini, coba opsi berikut ini di komputer yang terpengaruh:

- Buka aplikasi Office, pilih akun **file**  >  **Account**  >  **keluar dari semua akun**. Masuk lagi menggunakan akun pengguna dengan lisensi yang valid. Untuk informasi mendetail, lihat [ akun di Office ](https://support.office.com/article/accounts-in-office-628ea040-f265-49de-b986-be09c3ebf8a9).
- [Kosongkan kredensial Office](https://docs.microsoft.com/office/troubleshoot/error-messages/another-account-already-signed-in#step-3-clear-cached-credentials-on-the-computer) menggunakan Pengelola kredensial Windows.<br>
  **Catatan:** Jalur registri untuk Office 2016 telah diubah ke 16,0. Misalnya, \Software\Microsoft\Office\16.0\Common\Identity\
- Jika kesalahan terjadi saat menyambungkan ke Office 365 menggunakan Office 2013, [Aktifkan autentikasi modern](https://docs.microsoft.com/microsoft-365/admin/security-and-compliance/enable-modern-authentication) untuk klien Office.

Untuk informasi selengkapnya, lihat [cara memecahkan masalah aplikasi non-browser yang tidak dapat masuk ke Microsoft 365, Azure, atau Intune](https://support.office.com/article/how-to-troubleshoot-non-browser-apps-that-can-t-sign-in-to-office-365-azure-or-intune-3ba1b268-66f6-462c-b0e5-070f5c2603c1).

