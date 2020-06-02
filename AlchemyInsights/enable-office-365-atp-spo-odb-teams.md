---
title: Mengaktifkan Office 365 ATP untuk SharePoint, OneDrive, dan Microsoft teams
ms.author: deniseb
author: denisebmsft
manager: laurawi
ms.date: 04/21/2020
ms.audience: Admin
ms.topic: article
ROBOTS: NOINDEX, NOFOLLOW
localization_priority: Normal
ms.collection: Admin_O365
ms.custom: 3100021
ms.openlocfilehash: 564a7f1f6a37e64dbd7d679878ebadbbe35f3fa0
ms.sourcegitcommit: bc7d6f4f3c9f7060d073f5130e1ec856e248d020
ms.translationtype: MT
ms.contentlocale: id-ID
ms.lasthandoff: 06/02/2020
ms.locfileid: "44506921"
---
# <a name="enable-office-365-advanced-threat-protection-for-sharepoint-online-onedrive-and-microsoft-teams"></a>Mengaktifkan Office 365 lanjut ancaman perlindungan untuk SharePoint online, OneDrive dan Microsoft teams

1. Buka https://protection.office.com dan masuk.
2. Pilih **kebijakan manajemen ancaman**  >  **Policy**  >  **lampiran aman**.
3. Pilih **Aktifkan ATP untuk SharePoint, OneDrive, dan Microsoft teams**, dan kemudian klik **Simpan**.
4. Merekomendasikan Sebagai administrator global atau administrator SharePoint online, Jalankan cmdlet [set-SPOTenant](https://docs.microsoft.com/powershell/module/sharepoint-online/Set-SPOTenant?view=sharepoint-ps) dengan parameter **Disallowinfectedfiledownload** ditetapkan ke *True*.
5. Merekomendasikan [Mengatur peringatan](https://docs.microsoft.com/microsoft-365/security/office-365-security/turn-on-atp-for-spo-odb-and-teams#set-up-alerts-for-detected-files) untuk file terdeteksi.

> [!NOTE]
> ATP akan nuntuk memindai setiap file tunggal di SharePoint online, OneDrive, atau Microsoft teams. File dipindai secara asinkron, melalui proses yang menggunakan kegiatan berbagi dan aktivitas tamu, bersama dengan heuristik cerdas dan sinyal ancaman untuk mengidentifikasi file berbahaya. Lihat [ATP untuk SharePoint, OneDrive, dan Microsoft teams](https://docs.microsoft.com/microsoft-365/security/office-365-security/atp-for-spo-odb-and-teams).