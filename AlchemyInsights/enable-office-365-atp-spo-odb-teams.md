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
ms.openlocfilehash: dd367176f8d6f38f1f94ae6627229234f15c81ff
ms.sourcegitcommit: f4866e94918c7b591ad0cd3b58169d340bcc7f00
ms.translationtype: MT
ms.contentlocale: id-ID
ms.lasthandoff: 05/19/2021
ms.locfileid: "52543931"
---
# <a name="enable-microsoft-defender-for-office-365-for-sharepoint-online-onedrive-and-microsoft-teams"></a>Mengaktifkan Pertahanan Microsoft untuk Office 365 untuk SharePoint Online, OneDrive, dan Microsoft Teams

1. Buka https://protection.office.com dan masuk.
2. Pilih **Kebijakan manajemen**  >  **ancaman** Brankas  >  **Lampiran**.
3. Pilih **Aktifkan Pertahanan untuk Office 365 untuk SharePoint, OneDrive, dan Microsoft Teams**, lalu klik **Simpan.**
4. (Direkomendasikan) Sebagai administrator global atau administrator SharePoint Online, jalankan cmdlet [Set-SPOTenant](/powershell/module/sharepoint-online/Set-SPOTenant?view=sharepoint-ps) dengan parameter **DisallowInfectedFileDownload** diatur ke *true.*
5. (Direkomendasikan) [Setel pemberitahuan untuk](/microsoft-365/security/office-365-security/turn-on-atp-for-spo-odb-and-teams#set-up-alerts-for-detected-files) file yang terdeteksi.

> [!NOTE]
> Pertahanan Microsoft untuk Office 365 tidak akan memindai setiap file dalam SharePoint Online, OneDrive, atau Microsoft Teams. File dipindai secara asinkron, melalui proses yang menggunakan aktivitas berbagi dan acara tamu, bersama dengan heuristics cerdas dan sinyal ancaman untuk mengidentifikasi file berbahaya. Lihat [Pertahanan Microsoft untuk Office 365, SharePoint, OneDrive, dan Microsoft Teams](/microsoft-365/security/office-365-security/atp-for-spo-odb-and-teams).