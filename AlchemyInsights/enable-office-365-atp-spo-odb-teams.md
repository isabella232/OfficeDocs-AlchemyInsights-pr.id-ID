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
ms.openlocfilehash: fdfdc97a198898051a3388672d01994d96dd5e97
ms.sourcegitcommit: 55eff703a17e500681d8fa6a87eb067019ade3cc
ms.translationtype: MT
ms.contentlocale: id-ID
ms.lasthandoff: 04/22/2020
ms.locfileid: "43703429"
---
# <a name="enable-office-365-advanced-threat-protection-for-sharepoint-online-onedrive-and-microsoft-teams"></a>Mengaktifkan Office 365 lanjut ancaman perlindungan untuk SharePoint online, OneDrive dan Microsoft teams

1. Buka https://protection.office.com dan masuk.
2. Pilih > **Policy**kebijakan >  **manajemen ancaman****lampiran aman**.
3. Pilih **Aktifkan ATP untuk SharePoint, OneDrive, dan Microsoft teams**, dan kemudian klik **Simpan**.
4. Merekomendasikan Sebagai administrator global atau administrator SharePoint online, Jalankan cmdlet [set-SPOTenant](https://docs.microsoft.com/powershell/module/sharepoint-online/Set-SPOTenant?view=sharepoint-ps) dengan parameter **Disallowinfectedfiledownload** ditetapkan ke *True*.
5. Merekomendasikan [Mengatur peringatan](https://docs.microsoft.com/office365/securitycompliance/turn-on-atp-for-spo-odb-and-teams#set-up-alerts-for-detected-files) untuk file terdeteksi.

> [!NOTE]
> ATP akan nuntuk memindai setiap file tunggal di SharePoint online, OneDrive, atau Microsoft teams. File dipindai secara asinkron, melalui proses yang menggunakan kegiatan berbagi dan aktivitas tamu, bersama dengan heuristik cerdas dan sinyal ancaman untuk mengidentifikasi file berbahaya. Lihat [https://docs.microsoft.com/office365/securitycompliance/atp-for-spo-odb-and-teams](https://docs.microsoft.com/office365/securitycompliance/atp-for-spo-odb-and-teams)semuanya.