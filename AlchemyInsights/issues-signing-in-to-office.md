---
title: Masalah masuk ke Microsoft 365 baru
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
- "9000571"
- "2556"
ms.openlocfilehash: 7a8a0b68fc211e99b22e857d51d1de54e53a69357f75a0c60b1e83078cd5b27f
ms.sourcegitcommit: b5f7da89a650d2915dc652449623c78be6247175
ms.translationtype: MT
ms.contentlocale: id-ID
ms.lasthandoff: 08/05/2021
ms.locfileid: "54088039"
---
# <a name="blank-sign-in-screen-in-microsoft-365-apps"></a>Layar masuk kosong di Microsoft 365 gratis

Untuk memperbaiki masalah ini, cobalah hal berikut:
- Instal pembaruan terkini untuk semua [Windows](https://support.microsoft.com/help/4027667/windows-10-update) lalu [Office](https://support.office.com/article/update-office-and-your-computer-with-microsoft-update-2ab296f3-7f03-43a2-8e50-46de917611c5).
- Mengatur ulang opsi Internet Explorer: Masuk ke Alat Opsi Internet Tingkat Lanjut Reset  >    >    >  **Internet Explorer Pengaturan** (perhatikan bahwa Anda akan kehilangan pengaturan kustom), lalu coba masuk lagi Office lagi.
- Menonaktifkan Application Guard Pertahanan Windows (WKAL) atau firewall atau program antivirus yang serupa:
    1. Di Panel Kontrol, masuk **ke Program**, lalu pilih Windows mengaktifkan atau menonaktifkan **fitur ini.**
    2. Jika Application Guard Pertahanan Windows diaktifkan, cobalah menonaktifkannya.<br/>
    **Catatan:** Anda mungkin perlu memulai ulang komputer.
- Pastikan bahwa plug-in Microsoft.AAD.BrokerPlugin [AAD WAM tidak](https://docs.microsoft.com/office365/troubleshoot/administration/connection-issue-when-sign-in-office-2016#symptom-1) diblokir oleh program aplikasi atau firewall/antivirus apa pun.
- [Kosongkan Office kredensial](https://docs.microsoft.com/office/troubleshoot/error-messages/another-account-already-signed-in#step-3-clear-cached-credentials-on-the-computer) menggunakan Windows Manager Kredensial.<br/>
    **Catatan:** Jalur registri untuk Office 2016 telah berubah menjadi 16.0. (misalnya: \Software\Microsoft\Office\16.0\Common\Identity\)

Untuk informasi selengkapnya, lihat Masalah koneksi masuk setelah pembaruan [ke Office 2016 build 16.0.7967 pada Windows 10](https://docs.microsoft.com/office365/troubleshoot/administration/connection-issue-when-sign-in-office-2016).