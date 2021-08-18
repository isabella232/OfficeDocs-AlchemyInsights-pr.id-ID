---
title: Mengaktifkan Office 365 ATP untuk SharePoint, OneDrive, dan Microsoft Teams
ms.author: deniseb
author: denisebmsft
manager: laurawi
ms.date: 04/21/2020
ms.audience: Admin
ms.topic: article
ms.service: o365-administration
ROBOTS: NOINDEX, NOFOLLOW
localization_priority: Normal
ms.collection: Admin_O365
ms.custom: 3100021
ms.openlocfilehash: 2d132101768e0a835d448604d684ec0c735e6628
ms.sourcegitcommit: ab75f66355116e995b3cb5505465b31989339e28
ms.translationtype: MT
ms.contentlocale: id-ID
ms.lasthandoff: 08/13/2021
ms.locfileid: "58332162"
---
# <a name="enable-microsoft-defender-for-office-365-for-sharepoint-online-onedrive-and-microsoft-teams"></a>Mengaktifkan Pertahanan Microsoft untuk Office 365 Online SharePoint Online, OneDrive, dan Microsoft Teams

1. Buka https://protection.office.com dan masuk.
2. Pilih **Kebijakan manajemen**  >  **ancaman** Brankas  >  **Lampiran**.
3. Pilih **Aktifkan Pertahanan untuk Office 365, SharePoint, OneDrive, dan Microsoft Teams**, lalu klik **Simpan.**
4. (Direkomendasikan) Sebagai administrator global atau administrator SharePoint Online, jalankan cmdlet [Set-SPOTenant](https://docs.microsoft.com/powershell/module/sharepoint-online/Set-SPOTenant?view=sharepoint-ps) dengan parameter **DisallowInfectedFileDownload** diatur ke *true.*
5. (Direkomendasikan) [Setel pemberitahuan untuk](https://docs.microsoft.com/microsoft-365/security/office-365-security/turn-on-atp-for-spo-odb-and-teams#set-up-alerts-for-detected-files) file yang terdeteksi.

**Catatan**: Pertahanan Microsoft untuk Office 365 tidak akan memindai setiap file dalam SharePoint Online, OneDrive, atau Microsoft Teams. File dipindai secara asinkron, melalui proses yang menggunakan aktivitas berbagi dan acara tamu, bersama dengan heuristics cerdas dan sinyal ancaman untuk mengidentifikasi file berbahaya. Lihat [Pertahanan Microsoft untuk Office 365, SharePoint, OneDrive, dan Microsoft Teams](https://docs.microsoft.com/microsoft-365/security/office-365-security/atp-for-spo-odb-and-teams).
