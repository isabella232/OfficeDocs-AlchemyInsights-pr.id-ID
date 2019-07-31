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
- "2556"
ms.openlocfilehash: 08bb0a94066f071f2ba0e9c54378f0d479191496
ms.sourcegitcommit: 699ac3b0d66e0640f8e933eba3c2a4ba1cfcf3c7
ms.translationtype: MT
ms.contentlocale: id-ID
ms.lasthandoff: 07/30/2019
ms.locfileid: "35938247"
---
# <a name="blank-sign-in-screen-in-office-apps"></a>Masuk layar kosong di Office apps

Untuk mengatasi masalah ini, cobalah berikut ini:
- Menginstal update terbaru untuk [Windows](https://support.microsoft.com/help/4027667/windows-10-update) dan [Office](https://support.office.com/article/update-office-and-your-computer-with-microsoft-update-2ab296f3-7f03-43a2-8e50-46de917611c5).
- Mengatur ulang Internet Explorer pilihan: pergi ke **Tools** > **Internet Options** > **Advanced** > **Reset tataan Internet Explorer** (Perhatikan bahwa Anda akan kehilangan pengaturan), dan kemudian mencoba masuk ke kantor lagi.
- Menonaktifkan Windows Defender aplikasi penjaga (WDAG) atau program serupa firewall atau antivirus:
    1. Di Panel kontrol, pergi ke **program**, dan kemudian memilih **fitur Windows mengubah atau mati**.
    2. Jika Windows Defender aplikasi Guard diaktifkan, coba Nonaktifkan.<br/>
    **Catatan:** Anda mungkin perlu me-restart komputer.
- Memastikan bahwa Microsoft.AAD.BrokerPlugin [AAD WAM plug-in](https://docs.microsoft.com/office365/troubleshoot/administration/connection-issue-when-sign-in-office-2016#symptom-1) tidak sedang diblokir oleh firewall/anti-anti-virus program atau aplikasi apapun.
- [Jelas kantor kredensial](https://docs.microsoft.com/office/troubleshoot/error-messages/another-account-already-signed-in#step-3-clear-cached-credentials-on-the-computer) menggunakan Windows Credential Manager.<br/>
    **Catatan:** Jalur registri untuk kantor 2016 telah berubah untuk 16.0. (Ex: \Software\Microsoft\Office\16.0\Common\Identity\)

Untuk selengkapnya, lihat [sambungan isu-isu dalam masuk setelah update ke kantor 2016 membangun 16.0.7967 pada Windows 10](https://docs.microsoft.com/office365/troubleshoot/administration/connection-issue-when-sign-in-office-2016).