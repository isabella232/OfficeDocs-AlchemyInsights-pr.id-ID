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
- "2560"
ms.openlocfilehash: de0a1b78724db9a8e93d8d599ce3b503abcb86e2
ms.sourcegitcommit: 699ac3b0d66e0640f8e933eba3c2a4ba1cfcf3c7
ms.translationtype: MT
ms.contentlocale: id-ID
ms.lasthandoff: 07/30/2019
ms.locfileid: "35938245"
---
# <a name="fixing-the-office-apps-sorry-another-account-from-your-organization-is-already-signed-in-message"></a>Memperbaiki pesan "Maaf, account yang lain dari organisasi Anda sudah masuk" aplikasi kantor

Untuk memperbaiki kesalahan ini, coba langkah berikut:

- Menghapus semua pekerjaan account, kecuali account yang terkena, menggunakan > Windows pengaturan **akses kerja atau sekolah**.
- [Jelas kantor kredensial](https://docs.microsoft.com/office/troubleshoot/error-messages/another-account-already-signed-in#step-3-clear-cached-credentials-on-the-computer) menggunakan Windows Credential Manager.<br/>
    **Catatan:** Jalur registri untuk kantor 2016 telah berubah untuk 16.0. (Ex: \Software\Microsoft\Office\16.0\Common\Identity\)
- Buka aplikasi kantor, pilih **File** > **Account** > **Sign Out**. Kemudian masuk menggunakan account pengguna dengan lisensi berlaku. Untuk informasi rinci, lihat [account di kantor](https://support.office.com/article/accounts-in-office-628ea040-f265-49de-b986-be09c3ebf8a9).
- Untuk Mac, lihat [tidak dapat masuk ke kantor 2016 untuk Mac app](https://docs.microsoft.com/office365/troubleshoot/authentication/sign-in-to-office-2016-for-mac-fail).

Untuk informasi lebih lanjut, lihat ["Maaf, account yang lain dari organisasi Anda telah masuk di komputer ini" di kantor](https://docs.microsoft.com/office/troubleshoot/error-messages/another-account-already-signed-in).