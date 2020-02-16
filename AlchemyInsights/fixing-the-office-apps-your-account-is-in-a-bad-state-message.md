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
ms.openlocfilehash: e591c56dd207a5bcb3979be3f66052121100b162
ms.sourcegitcommit: 2572c4e5a981d5f3f556835061c568cfd08b78da
ms.translationtype: MT
ms.contentlocale: id-ID
ms.lasthandoff: 12/27/2019
ms.locfileid: "41969539"
---
# <a name="fixing-the-office-apps-your-account-is-in-a-bad-state-error"></a>Memperbaiki aplikasi Office "akun Anda dalam keadaan buruk" galat

Untuk memperbaiki galat ini, cobalah opsi berikut ini di komputer yang terpengaruh:

- Buka aplikasi Office, pilih**akun** >  **file** > **keluar dari semua akun**. Masuk lagi menggunakan akun pengguna dengan lisensi yang valid. Untuk informasi selengkapnya, lihat [akun di Office](https://support.office.com/article/accounts-in-office-628ea040-f265-49de-b986-be09c3ebf8a9).
- [Hapus kredensial Office](https://docs.microsoft.com/office/troubleshoot/error-messages/another-account-already-signed-in#step-3-clear-cached-credentials-on-the-computer) yang menggunakan Pengelola mandat Windows.<br>
  **Catatan:** Lintasan registri untuk Office 2016 telah diubah ke 16,0. Sebagai contoh, \Software\Microsoft\Office\16.0\Common\Identity\
- Pada komputer yang terpengaruh, tetapkan EnableADAL = 0 dengan menggunakan langkah berikut:  
     1. Klik kanan tombol Windows dan pilih **Jalankan**. Di kotak **buka** , ketik **regedit**, dan kemudian pilih **OK**.
     2. Pilih **ya** saat diminta untuk mengizinkan Penyunting registri untuk membuat perubahan pada perangkat Anda.
    3. Di Penyunting registri, tambahkan nilai DWORD EnableADAL dengan pengaturan 0 di bawah HKEY_CURRENT_USER \Software\Microsoft\Office\16.0\Common\Identity.
- Jika galat terjadi saat menyambung ke Office 365 menggunakan Office 2013, [aktifkan otentikasi modern](https://docs.microsoft.com/office365/admin/security-and-compliance/enable-modern-authentication) untuk klien Office.

Untuk informasi selengkapnya, lihat [bagaimana cara memecahkan masalah aplikasi non-browser yang tidak dapat masuk ke Office 365, Azure, atau Intune](https://support.office.com/article/how-to-troubleshoot-non-browser-apps-that-can-t-sign-in-to-office-365-azure-or-intune-3ba1b268-66f6-462c-b0e5-070f5c2603c1).

