---
title: SharePoint online PowerShell
ms.author: pebaum
author: pebaum
manager: mnirkhe
ms.date: 04/21/2020
ms.audience: Admin
ms.topic: article
ROBOTS: NOINDEX, NOFOLLOW
localization_priority: Normal
ms.collection: Adm_O365
ms.custom:
- "9000266"
- "1867"
ms.openlocfilehash: 300c07e7f0010eae2bd4fe893ece9d09aab93ba5
ms.sourcegitcommit: 90f37eebec9aaa9e49c2cf4d201152c5e20e384b
ms.translationtype: MT
ms.contentlocale: id-ID
ms.lasthandoff: 08/17/2020
ms.locfileid: "46786892"
---
# <a name="sharepoint-online-powershell"></a><span data-ttu-id="0f605-102">SharePoint online PowerShell</span><span class="sxs-lookup"><span data-stu-id="0f605-102">Sharepoint Online PowerShell</span></span>

<span data-ttu-id="0f605-103">Bekerja dengan PowerShell atau skrip dalam SharePoint online?</span><span class="sxs-lookup"><span data-stu-id="0f605-103">Working with PowerShell or Scripts within Sharepoint Online?</span></span> <span data-ttu-id="0f605-104">Kunjungi link di bawah ini untuk informasi selengkapnya.</span><span class="sxs-lookup"><span data-stu-id="0f605-104">Visit the links below for more information.</span></span>
- [<span data-ttu-id="0f605-105">Mulai menggunakan SharePoint online Management Shell</span><span class="sxs-lookup"><span data-stu-id="0f605-105">Getting started with SharePoint Online Management Shell</span></span>](https://docs.microsoft.com/powershell/sharepoint/sharepoint-online/connect-sharepoint-online?view=sharepoint-ps)
- [<span data-ttu-id="0f605-106">Menyambungkan ke PowerShell SPO dengan autentikasi multifaktor (MFA)</span><span class="sxs-lookup"><span data-stu-id="0f605-106">Connect to SPO PowerShell with multifactor authentication (MFA)</span></span>](https://docs.microsoft.com/powershell/sharepoint/sharepoint-online/connect-sharepoint-online?view=sharepoint-ps#to-connect-with-multifactor-authentication-mfa)
- <span data-ttu-id="0f605-107">[SharePoint Patterns and Practices (PNP)](https://docs.microsoft.com/powershell/sharepoint/sharepoint-pnp/sharepoint-pnp-cmdlets?view=sharepoint-ps) berisi pustaka perintah PowerShell yang memungkinkan Anda melakukan tindakan manajemen KOMPLEKS menuju SPO.</span><span class="sxs-lookup"><span data-stu-id="0f605-107">[SharePoint Patterns and Practices (PnP)](https://docs.microsoft.com/powershell/sharepoint/sharepoint-pnp/sharepoint-pnp-cmdlets?view=sharepoint-ps) contains a library of PowerShell commands that allows you to perform complex management actions towards SPO.</span></span>

> [!NOTE]
> - <span data-ttu-id="0f605-108">Jika Anda mengalami masalah saat menyambungkan ke shell manajemen SPO, pastikan bahwa Anda telah memperbarui ke versi terbaru dan mencoba [mengimpor ulang modul](https://docs.microsoft.com/powershell/developer/module/importing-a-powershell-module) menggunakan *"modul impor Microsoft. online. SharePoint. PowerShell".*</span><span class="sxs-lookup"><span data-stu-id="0f605-108">If you are having issues connecting with the SPO management shell, make sure that you have updated to the latest version and try to [re-import the module](https://docs.microsoft.com/powershell/developer/module/importing-a-powershell-module) using *“Import-Module Microsoft.Online.SharePoint.PowerShell”.*</span></span>
> - <span data-ttu-id="0f605-109">Jika Anda mencoba menjalankan skrip objek sisi klien, Anda harus memiliki [SDK komponen klien SharePoint online](https://www.microsoft.com/download/details.aspx?id=42038) yang terinstal di komputer lokal Anda.</span><span class="sxs-lookup"><span data-stu-id="0f605-109">If you are attempting to run client-side object model scripts, you will need to have the [Sharepoint Online Client Components SDK](https://www.microsoft.com/download/details.aspx?id=42038) installed on your local machine.</span></span>
> - <span data-ttu-id="0f605-110">Jika Anda mengalami masalah dalam menjalankan skrip dari PowerShell, Anda mungkin ingin mempertimbangkan menjalankan PowerShell sebagai administrator dan mengubah [kebijakan eksekusi](https://docs.microsoft.com/powershell/module/microsoft.powershell.core/about/about_execution_policies?view=powershell-6).</span><span class="sxs-lookup"><span data-stu-id="0f605-110">If you are having issues running scripts from PowerShell, you may want to consider running PowerShell as an Administrator and changing the [Execution Policy](https://docs.microsoft.com/powershell/module/microsoft.powershell.core/about/about_execution_policies?view=powershell-6).</span></span>