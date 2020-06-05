---
title: Memperbaiki aplikasi Microsoft 365 akun Anda berada dalam pesan status buruk
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
ms.openlocfilehash: 264307f23a349ef4ebf40f48ddbcddd3216a4927
ms.sourcegitcommit: f28dafa0f727870038f72bc904da926daf4ec07b
ms.translationtype: MT
ms.contentlocale: id-ID
ms.lasthandoff: 06/05/2020
ms.locfileid: "44580120"
---
# <a name="fixing-the-microsoft-365-apps-your-account-is-in-a-bad-state-error"></a>Memperbaiki Microsoft 365 aplikasi "akun Anda dalam keadaan buruk" galat

Untuk memperbaiki galat ini, cobalah opsi berikut ini di komputer yang terpengaruh:

- Buka aplikasi Office, pilih akun **file**  >  **Account**  >  **keluar dari semua akun**. Masuk lagi menggunakan akun pengguna dengan lisensi yang valid. Untuk informasi mendetail, lihat [ akun di Office ](https://support.office.com/article/accounts-in-office-628ea040-f265-49de-b986-be09c3ebf8a9).
- [Hapus kredensial Office](https://docs.microsoft.com/office/troubleshoot/error-messages/another-account-already-signed-in#step-3-clear-cached-credentials-on-the-computer) yang menggunakan Pengelola mandat Windows.<br>
  **Catatan:** Lintasan registri untuk Office 2016 telah diubah ke 16,0. Sebagai contoh, \Software\Microsoft\Office\16.0\Common\Identity\
- Jika galat terjadi saat menyambung ke Office 365 menggunakan Office 2013, [aktifkan otentikasi modern](https://docs.microsoft.com/microsoft-365/admin/security-and-compliance/enable-modern-authentication) untuk klien Office.

Untuk informasi selengkapnya, lihat [bagaimana cara memecahkan masalah aplikasi non-browser yang tidak dapat masuk ke Microsoft 365, Azure, atau Intune](https://support.office.com/article/how-to-troubleshoot-non-browser-apps-that-can-t-sign-in-to-office-365-azure-or-intune-3ba1b268-66f6-462c-b0e5-070f5c2603c1).

