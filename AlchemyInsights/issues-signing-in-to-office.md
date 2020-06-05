---
title: Masalah saat masuk ke aplikasi Microsoft 365
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
- "2556"
ms.openlocfilehash: 4658b4df8a48072b4cc9d72bf503d7911bb5126b
ms.sourcegitcommit: f28dafa0f727870038f72bc904da926daf4ec07b
ms.translationtype: MT
ms.contentlocale: id-ID
ms.lasthandoff: 06/05/2020
ms.locfileid: "44579904"
---
# <a name="blank-sign-in-screen-in-microsoft-365-apps"></a>Layar masuk kosong di Microsoft 365 aplikasi

Untuk memperbaiki masalah ini, cobalah berikut ini:
- Instal pemutakhiran terbaru untuk [Windows](https://support.microsoft.com/help/4027667/windows-10-update) dan [Office](https://support.office.com/article/update-office-and-your-computer-with-microsoft-update-2ab296f3-7f03-43a2-8e50-46de917611c5).
- Reset Internet Explorer Options: pergi ke **alat**  >  **Internet Options**  >  **lanjutan**  >  **reset Internet Explorer pengaturan** (Perhatikan bahwa Anda akan kehilangan pengaturan kustom), dan kemudian coba masuk ke kantor lagi.
- Nonaktifkan Windows Defender Application Guard (WDAG) atau program firewall atau anti-virus yang serupa:
    1. Di panel kontrol, pergi ke **program**, dan kemudian pilih **fitur Windows mengaktifkan atau menonaktifkan**.
    2. Jika pelindung aplikasi Windows Defender diaktifkan, cobalah menonaktifkannya.<br/>
    **Catatan:** Anda mungkin perlu me-restart komputer.
- Pastikan bahwa Microsoft. AAD. broker plugin [AAD WAM plug-in](https://docs.microsoft.com/office365/troubleshoot/administration/connection-issue-when-sign-in-office-2016#symptom-1) tidak sedang diblokir oleh aplikasi atau firewall/anti-virus program.
- [Hapus kredensial Office](https://docs.microsoft.com/office/troubleshoot/error-messages/another-account-already-signed-in#step-3-clear-cached-credentials-on-the-computer) yang menggunakan Pengelola mandat Windows.<br/>
    **Catatan:** Lintasan registri untuk Office 2016 telah diubah ke 16,0. (Mis: \Software\Microsoft\Office\16.0\Common\Identity\)

Untuk informasi selengkapnya, lihat [masalah sambungan di masuk setelah pembaruan ke Office 2016 membangun 16.0.7967 di Windows 10](https://docs.microsoft.com/office365/troubleshoot/administration/connection-issue-when-sign-in-office-2016).