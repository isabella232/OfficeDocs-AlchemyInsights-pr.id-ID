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
- "2559"
ms.openlocfilehash: 5f500ecf1f779fb1be4d257fd050a3ad054087dc
ms.sourcegitcommit: 699ac3b0d66e0640f8e933eba3c2a4ba1cfcf3c7
ms.translationtype: MT
ms.contentlocale: id-ID
ms.lasthandoff: 07/30/2019
ms.locfileid: "35938248"
---
# <a name="fixing-the-office-apps-your-computers-trusted-platform-module-is-not-functioning-properly-message"></a>Memperbaiki pesan kantor apps "modul terpercaya Platform komputer Anda tidak berfungsi dengan benar"

Untuk memperbaiki kesalahan ini, coba langkah berikut:

- Menginstal update terbaru untuk [Windows](https://support.microsoft.com/help/4027667/windows-10-update) dan [Office](https://support.office.com/article/update-office-and-your-computer-with-microsoft-update-2ab296f3-7f03-43a2-8e50-46de917611c5).
- [Jelas kantor kredensial](https://docs.microsoft.com/eoffice/troubleshoot/error-messages/another-account-already-signed-in#step-3-clear-cached-credentials-on-the-computer) menggunakan Windows Credential Manager.<br/>
    **Catatan:** Jalur registri untuk kantor 2016 telah berubah untuk 16.0. (Ex: \Software\Microsoft\Office\16.0\Common\Identity\)
- Mencoba [proses pemulihan pengguna](https://docs.microsoft.com/office365/troubleshoot/administration/connection-issue-when-sign-in-office-2016#symptom-2) untuk memperbaiki kegagalan dipercaya Platform modul (TPM).
- Menetapkan EnableADAL = 0 menggunakan langkah-langkah berikut:  
    1. Klik kanan tombol mulai Windows, memilih **Jalankan**, ketik **regedit**dan kemudian pilih **OK**.
    2. Pilih **ya** untuk memungkinkan Registry Editor untuk membuat perubahan ke perangkat Anda.
    3. Di Penyunting registri, menambahkan nilai DWORD **EnableADAL** dengan suasana **0** di bawah HKEY_CURRENT_USER\Software\Microsoft\Office\16.0\Common\Identity.

Untuk selengkapnya, lihat [sambungan isu-isu dalam masuk setelah update ke kantor 2016 membangun 16.0.7967 pada Windows 10](https://docs.microsoft.com/office365/troubleshoot/administration/connection-issue-when-sign-in-office-2016).