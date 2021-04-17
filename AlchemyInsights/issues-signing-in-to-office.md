---
title: Masalah masuk ke aplikasi Microsoft 365
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
ms.openlocfilehash: e6cbab7401fd6168041e7fc31ac97e3be036536d
ms.sourcegitcommit: 8bc60ec34bc1e40685e3976576e04a2623f63a7c
ms.translationtype: MT
ms.contentlocale: id-ID
ms.lasthandoff: 04/15/2021
ms.locfileid: "51833042"
---
# <a name="blank-sign-in-screen-in-microsoft-365-apps"></a>Layar masuk kosong di aplikasi Microsoft 365

Untuk memperbaiki masalah ini, cobalah hal berikut:
- Instal pembaruan terkini untuk [Windows](https://support.microsoft.com/help/4027667/windows-10-update) dan [Office.](https://support.office.com/article/update-office-and-your-computer-with-microsoft-update-2ab296f3-7f03-43a2-8e50-46de917611c5)
- Mengatur ulang opsi Internet Explorer: Masuk ke Alat Opsi Internet Reset Pengaturan Internet Explorer Tingkat Lanjut (perhatikan bahwa Anda akan kehilangan pengaturan kustom), lalu coba masuk lagi  >    >    >   ke Office.
- Menonaktifkan Application Guard Pertahanan Windows (WKAL, Application Guard) atau program antivirus atau firewall yang serupa:
    1. Di Panel Kontrol, masuk **ke Program**, lalu pilih Aktifkan **atau nonaktifkan fitur Windows**.
    2. Jika Application Guard Pertahanan Windows diaktifkan, coba nonaktifkan.<br/>
    **Catatan:** Anda mungkin perlu memulai ulang komputer.
- Pastikan bahwa plug-in Microsoft.AAD.BrokerPlugin [AAD WAM tidak](https://docs.microsoft.com/office365/troubleshoot/administration/connection-issue-when-sign-in-office-2016#symptom-1) diblokir oleh program aplikasi atau firewall/antivirus apa pun.
- [Hapus kredensial Office menggunakan](https://docs.microsoft.com/office/troubleshoot/error-messages/another-account-already-signed-in#step-3-clear-cached-credentials-on-the-computer) Pengelola Kredensial Windows.<br/>
    **Catatan:** Jalur registri untuk Office 2016 telah berubah menjadi 16.0. (misalnya: \Software\Microsoft\Office\16.0\Common\Identity\)

Untuk informasi selengkapnya, lihat Masalah koneksi masuk setelah pembaruan ke [Office 2016 build 16.0.7967 di Windows 10](https://docs.microsoft.com/office365/troubleshoot/administration/connection-issue-when-sign-in-office-2016).