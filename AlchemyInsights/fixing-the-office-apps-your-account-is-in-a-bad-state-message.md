---
title: Memperbaiki aplikasi Microsoft 365 Akun Anda berada dalam pesan status buruk
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
- "2558"
- "9000571"
ms.openlocfilehash: 4654b49289a455c1e6641f47fae573d2fcebc717
ms.sourcegitcommit: 8bc60ec34bc1e40685e3976576e04a2623f63a7c
ms.translationtype: MT
ms.contentlocale: id-ID
ms.lasthandoff: 04/15/2021
ms.locfileid: "51812539"
---
# <a name="fixing-the-microsoft-365-apps-your-account-is-in-a-bad-state-error"></a>Memperbaiki kesalahan "Akun Anda berada dalam keadaan buruk" aplikasi Microsoft 365

Untuk memperbaiki kesalahan ini, cobalah opsi berikut pada komputer yang terpengaruh:

- Buka aplikasi Office, pilih **Akun File** Keluar dari  >    >  **semua akun**. Masuk lagi menggunakan akun pengguna dengan lisensi yang valid. Untuk informasi mendetail, lihat [ akun di Office ](https://support.office.com/article/accounts-in-office-628ea040-f265-49de-b986-be09c3ebf8a9).
- [Hapus kredensial Office menggunakan](https://docs.microsoft.com/office/troubleshoot/error-messages/another-account-already-signed-in#step-3-clear-cached-credentials-on-the-computer) Pengelola Kredensial Windows.<br>
  **Catatan:** Jalur registri untuk Office 2016 telah berubah menjadi 16.0. Misalnya, \Software\Microsoft\Office\16.0\Common\Identity\
- Jika kesalahan terjadi saat menyambungkan ke Office 365 menggunakan Office 2013, aktifkan [autentikasi modern](https://docs.microsoft.com/microsoft-365/admin/security-and-compliance/enable-modern-authentication) untuk klien Office.

Untuk informasi selengkapnya, lihat Cara memecahkan masalah aplikasi non-browser yang tidak dapat masuk ke [Microsoft 365, Azure, atau Intune.](https://support.office.com/article/how-to-troubleshoot-non-browser-apps-that-can-t-sign-in-to-office-365-azure-or-intune-3ba1b268-66f6-462c-b0e5-070f5c2603c1)

