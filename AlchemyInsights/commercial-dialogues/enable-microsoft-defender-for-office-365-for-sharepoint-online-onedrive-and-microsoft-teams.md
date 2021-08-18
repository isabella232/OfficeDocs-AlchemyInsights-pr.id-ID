---
title: Mengaktifkan Brankas Lampiran untuk SharePoint Online, OneDrive, dan Microsoft Teams
ms.author: v-jmathew
author: v-jmathew
manager: dansimp
audience: Admin
ms.topic: article
ms.service: o365-administration
ROBOTS: NOINDEX, NOFOLLOW
localization_priority: Normal
ms.collection: Adm_O365
ms.custom:
- "9000760"
- "7391"
ms.openlocfilehash: 61372075ac8ccf04606a8003b4ec29f89fc048e5
ms.sourcegitcommit: ab75f66355116e995b3cb5505465b31989339e28
ms.translationtype: MT
ms.contentlocale: id-ID
ms.lasthandoff: 08/13/2021
ms.locfileid: "58332382"
---
# <a name="enable-safe-attachments-for-sharepoint-online-onedrive-and-microsoft-teams"></a>Mengaktifkan Brankas Lampiran untuk SharePoint Online, OneDrive, dan Microsoft Teams

1. Dengan menggunakan kredensial admin global atau keamanan, buka portal Pertahanan Microsoft 365 di , lalu masuk ke Kebijakan & kebijakan <https://security.microsoft.com>  \>  \> **ancaman Brankas Lampiran**  di bagian Kebijakan

   Untuk langsung masuk ke **Brankas Lampiran,** gunakan <https://security.microsoft.com/safeattachmentv2> .

2. Pada halaman **Brankas Lampiran,** klik **Pengaturan global.**
3. Di flyout yang muncul, pilih Aktifkan Pertahanan Microsoft untuk Office 365 untuk **SharePoint, OneDrive, dan Microsoft Teams**, lalu pilih **Simpan**.

    **Tips**: Lakukan langkah-langkah berikut untuk meningkatkan proteksi Lampiran Brankas untuk SharePoint, OneDrive, Microsoft Teams:
    - Untuk mencegah pengguna mengunduh file berbahaya, gunakan nilai untuk `$true` parameter *DisallowInfectedFileDownload* di cmdlet **[Set-SPOTenant](https://docs.microsoft.com/powershell/module/sharepoint-online/Set-SPOTenant)** di SharePoint Online PowerShell. Untuk informasi selengkapnya, [lihat SharePoint Online PowerShell untuk mencegah pengguna mengunduh file berbahaya.](https://docs.microsoft.com/microsoft-365/security/office-365-security/turn-on-mdo-for-spo-odb-and-teams#step-2-recommended-use-sharepoint-online-powershell-to-prevent-users-from-downloading-malicious-files)
    - [Membuat kebijakan pemberitahuan untuk file yang terdeteksi](https://docs.microsoft.com/microsoft-365/security/office-365-security/turn-on-mdo-for-spo-odb-and-teams#step-3-recommended-use-the-microsoft-365-defender-portal-to-create-an-alert-policy-for-detected-files)

Untuk informasi selengkapnya, [lihat Brankas Lampiran untuk Office 365 untuk SharePoint, OneDrive, Microsoft Teams](https://go.microsoft.com/fwlink/?linkid=2092041).
