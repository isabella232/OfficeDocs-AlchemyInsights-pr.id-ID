---
title: Memperbaiki aplikasi Office akun Anda berada dalam pesan status buruk
ms.author: pebaum
author: pebaum
manager: mnirkhe
ms.audience: Admin
ms.topic: article
ROBOTS: NOINDEX, NOFOLLOW
localization_priority: Normal
ms.collection: Adm_O365
ms.custom:
- "2558"
- "9000571"
ms.openlocfilehash: ac760b417ad98b9d5bb6be4b92e60074ab93ceb3
ms.sourcegitcommit: 55eff703a17e500681d8fa6a87eb067019ade3cc
ms.translationtype: MT
ms.contentlocale: id-ID
ms.lasthandoff: 04/22/2020
ms.locfileid: "43708690"
---
# <a name="fixing-the-office-apps-your-account-is-in-a-bad-state-error"></a>Memperbaiki aplikasi Office "akun Anda dalam keadaan buruk" galat

Untuk memperbaiki galat ini, cobalah opsi berikut ini di komputer yang terpengaruh:

- Buka aplikasi Office, pilih**akun** >  **file** > **keluar dari semua akun**. Masuk lagi menggunakan akun pengguna dengan lisensi yang valid. Untuk informasi mendetail, lihat [ akun di Office ](https://support.office.com/article/accounts-in-office-628ea040-f265-49de-b986-be09c3ebf8a9).
- [Hapus kredensial Office](https://docs.microsoft.com/office/troubleshoot/error-messages/another-account-already-signed-in#step-3-clear-cached-credentials-on-the-computer) yang menggunakan Pengelola mandat Windows.<br>
  **Catatan:** Lintasan registri untuk Office 2016 telah diubah ke 16,0. Sebagai contoh, \Software\Microsoft\Office\16.0\Common\Identity\
- Jika galat terjadi saat menyambung ke Office 365 menggunakan Office 2013, [aktifkan otentikasi modern](https://docs.microsoft.com/office365/admin/security-and-compliance/enable-modern-authentication) untuk klien Office.

Untuk informasi selengkapnya, lihat [bagaimana cara memecahkan masalah aplikasi non-browser yang tidak dapat masuk ke Microsoft 365, Azure, atau Intune](https://support.office.com/article/how-to-troubleshoot-non-browser-apps-that-can-t-sign-in-to-office-365-azure-or-intune-3ba1b268-66f6-462c-b0e5-070f5c2603c1).

