---
title: Memperbaiki aplikasi Microsoft 365 Akun Anda berada dalam pesan status yang buruk
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
ms.openlocfilehash: 68c4dfcc0500761f8ce5090fddb9f2ad58af77bc411c9e714b14c383fef177de
ms.sourcegitcommit: b5f7da89a650d2915dc652449623c78be6247175
ms.translationtype: MT
ms.contentlocale: id-ID
ms.lasthandoff: 08/05/2021
ms.locfileid: "54068239"
---
# <a name="fixing-the-microsoft-365-apps-your-account-is-in-a-bad-state-error"></a>Memperbaiki kesalahan Microsoft 365 "Akun Anda berada dalam keadaan buruk"

Untuk memperbaiki kesalahan ini, cobalah opsi berikut pada komputer yang terpengaruh:

- Buka buku aplikasi Office, pilih **Keluar** Akun File  >    >  **dari semua akun**. Masuk lagi menggunakan akun pengguna dengan lisensi yang valid. Untuk informasi mendetail, lihat [ Akun di Office ](https://support.office.com/article/accounts-in-office-628ea040-f265-49de-b986-be09c3ebf8a9).
- [Kosongkan Office kredensial](https://docs.microsoft.com/office/troubleshoot/error-messages/another-account-already-signed-in#step-3-clear-cached-credentials-on-the-computer) menggunakan Windows Manager Kredensial.<br>
  **Catatan:** Jalur registri untuk Office 2016 telah berubah menjadi 16.0. Misalnya, \Software\Microsoft\Office\16.0\Common\Identity\
- Jika kesalahan terjadi saat menyambungkan ke Office 365 menggunakan Office 2013, aktifkan autentikasi [modern](https://docs.microsoft.com/microsoft-365/admin/security-and-compliance/enable-modern-authentication) untuk Office klien.

Untuk informasi selengkapnya, lihat Cara memecahkan masalah aplikasi non-browser yang tidak dapat masuk ke [Microsoft 365, Azure, atau Intune.](https://support.office.com/article/how-to-troubleshoot-non-browser-apps-that-can-t-sign-in-to-office-365-azure-or-intune-3ba1b268-66f6-462c-b0e5-070f5c2603c1)

