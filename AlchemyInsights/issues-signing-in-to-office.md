---
title: Masalah masuk ke aplikasi Microsoft 365
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
- "9000571"
- "2556"
ms.openlocfilehash: 3c016b198ad43f35c8149dde71c28a2f7fc3bd38
ms.sourcegitcommit: c6692ce0fa1358ec3529e59ca0ecdfdea4cdc759
ms.translationtype: MT
ms.contentlocale: id-ID
ms.lasthandoff: 09/14/2020
ms.locfileid: "47695290"
---
# <a name="blank-sign-in-screen-in-microsoft-365-apps"></a>Layar masuk kosong di aplikasi Microsoft 365

Untuk memperbaiki masalah ini, cobalah yang berikut ini:
- Instal pembaruan terbaru untuk [Windows](https://support.microsoft.com/help/4027667/windows-10-update) dan [Office](https://support.office.com/article/update-office-and-your-computer-with-microsoft-update-2ab296f3-7f03-43a2-8e50-46de917611c5).
- Reset Opsi Internet Explorer: masuk ke **Tools**  >  **Opsi Internet**Tools  >  **Advanced**  >  **reset pengaturan Internet Explorer** (Perhatikan bahwa Anda akan kehilangan pengaturan kustom), lalu coba masuk ke Office lagi.
- Nonaktifkan Windows Defender Application Guard (WDAG) atau program firewall atau antivirus yang sama:
    1. Di panel kontrol, masuk ke **program**, lalu pilih **Aktifkan atau nonaktifkan fitur Windows**.
    2. Jika Windows Defender Application Guard diaktifkan, coba Nonaktifkan.<br/>
    **Catatan:** Anda mungkin perlu memulai ulang komputer.
- Pastikan bahwa plugin Microsoft. AAD. broker [AAD WAM plug-in](https://docs.microsoft.com/office365/troubleshoot/administration/connection-issue-when-sign-in-office-2016#symptom-1) tidak diblokir oleh aplikasi atau firewall/program antivirus.
- [Kosongkan kredensial Office](https://docs.microsoft.com/office/troubleshoot/error-messages/another-account-already-signed-in#step-3-clear-cached-credentials-on-the-computer) menggunakan Pengelola kredensial Windows.<br/>
    **Catatan:** Jalur registri untuk Office 2016 telah diubah ke 16,0. (Mis: \Software\Microsoft\Office\16.0\Common\Identity\)

Untuk informasi selengkapnya, lihat [masalah koneksi di masuk setelah pembaruan ke Office 2016 Build 16.0.7967 di Windows 10](https://docs.microsoft.com/office365/troubleshoot/administration/connection-issue-when-sign-in-office-2016).