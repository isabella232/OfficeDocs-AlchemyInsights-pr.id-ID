---
title: Mengaktifkan Office 365 ATP untuk SharePoint, OneDrive, dan tim Microsoft
ms.author: deniseb
author: denisebmsft
manager: laurawi
ms.date: 04/01/2019
ms.audience: Admin
ms.topic: article
ROBOTS: NOINDEX, NOFOLLOW
localization_priority: Normal
ms.collection: Admin_O365
ms.custom: 3100021
ms.openlocfilehash: ae2f574663ae3233a056589c2d5a578171f3b2f4
ms.sourcegitcommit: 601aec31e6556286fe5e0fd62827a037cbb6fe17
ms.translationtype: MT
ms.contentlocale: id-ID
ms.lasthandoff: 04/02/2019
ms.locfileid: "31030998"
---
# <a name="enable-office-365-advanced-threat-protection-for-sharepoint-online-onedrive-and-microsoft-teams"></a>Mengaktifkan Office 365 lanjutan ancaman perlindungan untuk SharePoint Online, OneDrive, dan tim Microsoft

1. Pergi ke https://protection.office.com dan masuk.
2. Memilih **manajemen ancaman** > **kebijakan** > **Lampiran aman**.
3. Pilih **Aktifkan ATP untuk SharePoint, OneDrive, dan Microsoft tim**, dan kemudian klik **Simpan**.
4. (Disarankan) Sebagai administrator global atau seorang administrator SharePoint Online, Jalankan cmdlet [Set-SPOTenant](https://docs.microsoft.com/powershell/module/sharepoint-online/Set-SPOTenant?view=sharepoint-ps) dengan parameter **DisallowInfectedFileDownload** diatur ke *true*.
5. (Disarankan) [Mengatur tanda](https://docs.microsoft.com/office365/securitycompliance/turn-on-atp-for-spo-odb-and-teams#set-up-alerts-for-detected-files) untuk file terdeteksi.

> [!NOTE]
> ATP akan tidak memindai setiap satu file di SharePoint Online, OneDrive, atau Microsoft Teams. File scan asynchronously, melalui sebuah proses yang menggunakan berbagi dan tamu acara kegiatan, bersama dengan cerdas heuristik dan ancaman sinyal untuk mengidentifikasi file jahat. Lihat [https://docs.microsoft.com/office365/securitycompliance/atp-for-spo-odb-and-teams](https://docs.microsoft.com/office365/securitycompliance/atp-for-spo-odb-and-teams).