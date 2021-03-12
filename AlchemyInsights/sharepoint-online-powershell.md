---
title: SharePoint online PowerShell
ms.author: pebaum
author: pebaum
manager: mnirkhe
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
ms.openlocfilehash: b7580f0e609d21bdc13fc07fda0bfd15bdb7a7ca
ms.sourcegitcommit: 0eb4f9bde53395b5fd4b5cd4ffc56ca96db91298
ms.translationtype: MT
ms.contentlocale: id-ID
ms.lasthandoff: 03/10/2021
ms.locfileid: "50709073"
---
# <a name="sharepoint-online-powershell"></a><span data-ttu-id="052d8-102">SharePoint online PowerShell</span><span class="sxs-lookup"><span data-stu-id="052d8-102">Sharepoint Online PowerShell</span></span>

<span data-ttu-id="052d8-103">Bekerja dengan PowerShell atau skrip dalam SharePoint online?</span><span class="sxs-lookup"><span data-stu-id="052d8-103">Working with PowerShell or Scripts within Sharepoint Online?</span></span> <span data-ttu-id="052d8-104">Kunjungi link di bawah ini untuk informasi selengkapnya.</span><span class="sxs-lookup"><span data-stu-id="052d8-104">Visit the links below for more information.</span></span>
- [<span data-ttu-id="052d8-105">Mulai menggunakan SharePoint online Management Shell</span><span class="sxs-lookup"><span data-stu-id="052d8-105">Getting started with SharePoint Online Management Shell</span></span>](https://docs.microsoft.com/powershell/sharepoint/sharepoint-online/connect-sharepoint-online?view=sharepoint-ps)
- [<span data-ttu-id="052d8-106">Menyambungkan ke PowerShell SPO dengan autentikasi multifaktor (MFA)</span><span class="sxs-lookup"><span data-stu-id="052d8-106">Connect to SPO PowerShell with multifactor authentication (MFA)</span></span>](https://docs.microsoft.com/powershell/sharepoint/sharepoint-online/connect-sharepoint-online?view=sharepoint-ps#to-connect-with-multifactor-authentication-mfa)
- <span data-ttu-id="052d8-107">[SharePoint Patterns and Practices (PNP)](https://docs.microsoft.com/powershell/sharepoint/sharepoint-pnp/sharepoint-pnp-cmdlets?view=sharepoint-ps) berisi pustaka perintah PowerShell yang memungkinkan Anda melakukan tindakan manajemen KOMPLEKS menuju SPO.</span><span class="sxs-lookup"><span data-stu-id="052d8-107">[SharePoint Patterns and Practices (PnP)](https://docs.microsoft.com/powershell/sharepoint/sharepoint-pnp/sharepoint-pnp-cmdlets?view=sharepoint-ps) contains a library of PowerShell commands that allows you to perform complex management actions towards SPO.</span></span>

> [!NOTE]
> - <span data-ttu-id="052d8-108">Jika Anda mengalami masalah saat menyambungkan ke shell manajemen SPO, pastikan bahwa Anda telah memperbarui ke versi terbaru dan mencoba [mengimpor ulang modul](https://docs.microsoft.com/powershell/scripting/developer/module/importing-a-powershell-module?view=powershell-7.1) menggunakan *"modul impor Microsoft. online. SharePoint. PowerShell".*</span><span class="sxs-lookup"><span data-stu-id="052d8-108">If you are having issues connecting with the SPO management shell, make sure that you have updated to the latest version and try to [re-import the module](https://docs.microsoft.com/powershell/scripting/developer/module/importing-a-powershell-module?view=powershell-7.1) using *“Import-Module Microsoft.Online.SharePoint.PowerShell”.*</span></span>
> - <span data-ttu-id="052d8-109">Jika Anda mencoba menjalankan skrip objek sisi klien, Anda harus memiliki [SDK komponen klien SharePoint online](https://www.microsoft.com/download/details.aspx?id=42038) yang terinstal di komputer lokal Anda.</span><span class="sxs-lookup"><span data-stu-id="052d8-109">If you are attempting to run client-side object model scripts, you will need to have the [Sharepoint Online Client Components SDK](https://www.microsoft.com/download/details.aspx?id=42038) installed on your local machine.</span></span>
> - <span data-ttu-id="052d8-110">Jika Anda mengalami masalah dalam menjalankan skrip dari PowerShell, Anda mungkin ingin mempertimbangkan menjalankan PowerShell sebagai administrator dan mengubah [kebijakan eksekusi](https://docs.microsoft.com/powershell/module/microsoft.powershell.core/about/about_execution_policies?view=powershell-6).</span><span class="sxs-lookup"><span data-stu-id="052d8-110">If you are having issues running scripts from PowerShell, you may want to consider running PowerShell as an Administrator and changing the [Execution Policy](https://docs.microsoft.com/powershell/module/microsoft.powershell.core/about/about_execution_policies?view=powershell-6).</span></span>