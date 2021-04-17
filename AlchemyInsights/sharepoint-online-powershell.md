---
title: Sharepoint Online PowerShell
ms.author: pebaum
author: pebaum
manager: scotv
ms.date: 04/21/2020
ms.audience: Admin
ms.topic: article
ms.service: o365-administration
ROBOTS: NOINDEX, NOFOLLOW
localization_priority: Normal
ms.collection: Adm_O365
ms.custom:
- "9000266"
- "1867"
ms.openlocfilehash: 839a70282b4dd619e9dbe8167ef0e409e468b1ad
ms.sourcegitcommit: 8bc60ec34bc1e40685e3976576e04a2623f63a7c
ms.translationtype: MT
ms.contentlocale: id-ID
ms.lasthandoff: 04/15/2021
ms.locfileid: "51830585"
---
# <a name="sharepoint-online-powershell"></a>Sharepoint Online PowerShell

Bekerja dengan PowerShell atau Skrip di dalam Sharepoint Online? Kunjungi tautan di bawah ini untuk informasi selengkapnya.
- [Mulai menggunakan SharePoint Online Management Shell](https://docs.microsoft.com/powershell/sharepoint/sharepoint-online/connect-sharepoint-online?view=sharepoint-ps)
- [Menyambungkan ke SPO PowerShell dengan multifactor authentication (MFA)](https://docs.microsoft.com/powershell/sharepoint/sharepoint-online/connect-sharepoint-online?view=sharepoint-ps#to-connect-with-multifactor-authentication-mfa)
- [Pola dan Praktik SharePoint (PnP)](https://docs.microsoft.com/powershell/sharepoint/sharepoint-pnp/sharepoint-pnp-cmdlets?view=sharepoint-ps) berisi pustaka perintah PowerShell yang memungkinkan Anda untuk melakukan tindakan manajemen kompleks terhadap SPO.

> [!NOTE]
> - Jika mengalami masalah dalam menyambungkan dengan shell manajemen SPO, pastikan telah memperbarui [](https://docs.microsoft.com/powershell/scripting/developer/module/importing-a-powershell-module?view=powershell-7.1) ke versi terbaru dan cobalah mengimpor ulang modul menggunakan *"Import-Module Microsoft.Online.SharePoint.PowerShell".*
> - If you are attempting to run client-side object model scripts, you will need to have the [Sharepoint Online Client Components SDK](https://www.microsoft.com/download/details.aspx?id=42038) installed on your local machine.
> - Jika Anda mengalami masalah menjalankan skrip dari PowerShell, Anda mungkin ingin mempertimbangkan menjalankan PowerShell sebagai Administrator dan mengubah Kebijakan [Eksekusi](https://docs.microsoft.com/powershell/module/microsoft.powershell.core/about/about_execution_policies?view=powershell-6).