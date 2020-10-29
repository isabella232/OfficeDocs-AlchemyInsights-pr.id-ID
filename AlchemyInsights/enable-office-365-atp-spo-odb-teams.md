---
title: Mengaktifkan Office 365 ATP untuk SharePoint, OneDrive, dan Microsoft teams
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
ms.openlocfilehash: bef43656097c6f27677172899df1ada7900a9b64
ms.sourcegitcommit: 4caf5e6c2fee2903ccaf92cfc9006eb580faa7ba
ms.translationtype: MT
ms.contentlocale: id-ID
ms.lasthandoff: 10/29/2020
ms.locfileid: "48801051"
---
# <a name="enable-microsoft-defender-for-office-365-for-sharepoint-online-onedrive-and-microsoft-teams"></a>Mengaktifkan Microsoft Defender untuk Office 365 untuk SharePoint online, OneDrive, dan Microsoft teams

1. Masuk ke https://protection.office.com dan masuk.
2. Pilih **Threat management**  >  **Policy**  >  **lampiran aman** kebijakan manajemen ancaman.
3. Pilih **Aktifkan ATP untuk SharePoint, OneDrive, dan Microsoft teams** , lalu klik **Simpan** .
4. Telah Sebagai administrator global atau administrator SharePoint online, Jalankan cmdlet [set-SPOTenant](https://docs.microsoft.com/powershell/module/sharepoint-online/Set-SPOTenant?view=sharepoint-ps) dengan set parameter **Disallowinfecfiledownload** ke *True* .
5. Telah [Siapkan pemberitahuan](https://docs.microsoft.com/microsoft-365/security/office-365-security/turn-on-atp-for-spo-odb-and-teams#set-up-alerts-for-detected-files) untuk file yang terdeteksi.

> [!NOTE]
> ATP akan memindai setiap file di SharePoint online, OneDrive, atau Microsoft teams. File dipindai secara asinkron, melalui proses yang menggunakan acara berbagi dan aktivitas tamu, bersama dengan heuristics dan ancaman sinyal cerdas untuk mengidentifikasi file berbahaya. Lihat [ATP untuk SharePoint, OneDrive, dan Microsoft teams](https://docs.microsoft.com/microsoft-365/security/office-365-security/atp-for-spo-odb-and-teams).