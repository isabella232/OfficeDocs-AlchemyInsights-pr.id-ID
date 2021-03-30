---
title: Mendapatkan daftar Aplikasi Perusahaan
ms.author: v-jmathew
author: v-jmathew
manager: scotv
audience: Admin
ms.topic: article
ms.service: o365-administration
ROBOTS: NOINDEX, NOFOLLOW
localization_priority: Normal
ms.collection: Adm_O365
ms.custom:
- "9004342"
- "9837"
ms.openlocfilehash: f5c1a77e415d4bbaa5718a6668af95934db7e5ae
ms.sourcegitcommit: e5f261f95ffc6074cce89e62ef8c4e9fd519d3ee
ms.translationtype: MT
ms.contentlocale: id-ID
ms.lasthandoff: 03/26/2021
ms.locfileid: "51404929"
---
# <a name="get-a-list-of-enterprise-applications"></a><span data-ttu-id="8e73a-102">Mendapatkan daftar Aplikasi Perusahaan</span><span class="sxs-lookup"><span data-stu-id="8e73a-102">Get a list of Enterprise Applications</span></span>

1. <span data-ttu-id="8e73a-103">Untuk **mendapatkan** daftar aplikasi perusahaan (semua aplikasi atau yang difilter menurut Tampilkan nama, ID, Pengidentifikasi URI, dll.) melalui perintah Powershell, lihat [Get-AzureADApplication (AzureAD).](https://docs.microsoft.com/powershell/module/azuread/get-azureadapplication)</span><span class="sxs-lookup"><span data-stu-id="8e73a-103">To **get a list of enterprise applications** (all applications or filtered by Display name, ID, Identifier URIs, etc.) through Powershell command, see [Get-AzureADApplication (AzureAD)](https://docs.microsoft.com/powershell/module/azuread/get-azureadapplication).</span></span>
2. <span data-ttu-id="8e73a-104">Untuk mendapatkan daftar objek prinsipal layanan (semua objek atau difilter menurut ID) melalui perintah Powershell, lihat [Get-AzureADServicePrincipal (AzureAD).](https://docs.microsoft.com/powershell/module/azuread/get-azureadserviceprincipal)</span><span class="sxs-lookup"><span data-stu-id="8e73a-104">To get a list of service principal objects (all objects or filtered by ID) through Powershell command, see [Get-AzureADServicePrincipal (AzureAD)](https://docs.microsoft.com/powershell/module/azuread/get-azureadserviceprincipal).</span></span>
3. <span data-ttu-id="8e73a-105">Jika Anda ingin **mendapatkan daftar aplikasi yang dikonfigurasi SAML, skrip PowerShell berikut ini** mungkin membantu Anda:</span><span class="sxs-lookup"><span data-stu-id="8e73a-105">If you want to **get a list of SAML configured apps, following PowerShell scripts** may help you:</span></span>

    <span data-ttu-id="8e73a-106">Setiap Aplikasi yang menggunakan aplikasi OAuth atau aplikasi SAML (aplikasi galeri dan non-galeri) memiliki dua objek yang dibuat di AAD saat registrasi terjadi.</span><span class="sxs-lookup"><span data-stu-id="8e73a-106">Every Application be it an OAuth app or SAML app (both gallery and non-gallery apps) would have two objects created in AAD when their registration happens.</span></span> <span data-ttu-id="8e73a-107">Yang pertama disebut Objek Aplikasi dan yang lainnya adalah objek Prinsipal Layanan.</span><span class="sxs-lookup"><span data-stu-id="8e73a-107">One is called the Application Object and the other is the Service Principal object.</span></span> <span data-ttu-id="8e73a-108">Ketika Anda membuang properti Objek Prinsipal Layanan menggunakan PowerShell, Anda akan mendapati bahwa setiap aplikasi memiliki sejumlah Tag tertentu yang terkait dengannya seperti:</span><span class="sxs-lookup"><span data-stu-id="8e73a-108">When you dump the properties of a Service Principal Object using PowerShell, you would find that every application has a certain number of Tags associated with it like:</span></span>

    - <span data-ttu-id="8e73a-109">Aplikasi OAuth memiliki tag yang disebut "**WindowsAzureActiveDirectoryIntegratedApp**"</span><span class="sxs-lookup"><span data-stu-id="8e73a-109">OAuth apps would have a tag called "**WindowsAzureActiveDirectoryIntegratedApp**"</span></span>
    - <span data-ttu-id="8e73a-110">Aplikasi SAML Galeri akan memiliki tag disebut "**WindowsAzureActiveDirectoryGalleryApplicationPrimaryV1**"</span><span class="sxs-lookup"><span data-stu-id="8e73a-110">Gallery SAML Apps would have a tag called "**WindowsAzureActiveDirectoryGalleryApplicationPrimaryV1**"</span></span>
    - <span data-ttu-id="8e73a-111">Aplikasi SAML Non-Galeri akan memiliki tag bernama "**WindowsAzureActiveDirectoryCustomSingleSignOnApplication**"</span><span class="sxs-lookup"><span data-stu-id="8e73a-111">Non-Gallery SAML Apps would have a tag called "**WindowsAzureActiveDirectoryCustomSingleSignOnApplication**"</span></span>

    <span data-ttu-id="8e73a-112">Karenanya, Anda bisa menggunakan tag ini dan mencari tahu jenis aplikasinya.</span><span class="sxs-lookup"><span data-stu-id="8e73a-112">Hence, you can use these tags and find out what kind of app it is.</span></span> <span data-ttu-id="8e73a-113">Tag "**WindowsAzureActiveDirectoryIntegratedApp**" umum digunakan untuk semua tipe aplikasi.</span><span class="sxs-lookup"><span data-stu-id="8e73a-113">The tag "**WindowsAzureActiveDirectoryIntegratedApp**" is common to all types of apps.</span></span> <span data-ttu-id="8e73a-114">Anda dapat menggunakan snippet berikut untuk mencantumkan semua aplikasi SAML (baik galeri maupun non galeri):</span><span class="sxs-lookup"><span data-stu-id="8e73a-114">You can use following snippet to list all the SAML apps (both gallery and non-gallery):</span></span>

    `$type = "SAML APP"`

    `Get-AzureADServicePrincipal -All true | Where-Object {(.Tags -contains "WindowsAzureActiveDirectoryGalleryApplicationNonPrimaryV1") -or (_.Tags -contains "WindowsAzureActiveDirectoryCustomSingleSignOnApplication")} | Select DisplayName, @{Name="AppType"; Expression={type}}_.`

    <span data-ttu-id="8e73a-115">Untuk informasi selengkapnya, lihat [Mengidentifikasi aplikasi yang mendukung SAML di Azure AD](https://docs.microsoft.com/answers/questions/24259/identify-saml-enabled-apps-in-azure-ad.html).</span><span class="sxs-lookup"><span data-stu-id="8e73a-115">For more information, see [Identify SAML-enabled apps in Azure AD](https://docs.microsoft.com/answers/questions/24259/identify-saml-enabled-apps-in-azure-ad.html).</span></span>

4. <span data-ttu-id="8e73a-116">**Hanya menemukan dan mencantumkan aplikasi Web:** Gunakan perintah di bawah ini untuk mendapatkan semua aplikasi Azure AD dengan tipe aplikasi "Web app/API"</span><span class="sxs-lookup"><span data-stu-id="8e73a-116">**Find and list only Web applications**: Use the below command to get all Azure AD applications with the application type "Web app/API"</span></span>

    <span data-ttu-id="8e73a-117">Get-AzureADApplication -Semua:$true | Where-Object { $_. PublicClient -ne $true } | FT</span><span class="sxs-lookup"><span data-stu-id="8e73a-117">Get-AzureADApplication -All:$true | Where-Object { $_.PublicClient -ne $true } | FT</span></span>
5. <span data-ttu-id="8e73a-118">**Temukan dan list Aplikasi asli** saja: Jalankan perintah berikut untuk mendapatkan semua aplikasi klien asli (desktop/perangkat seluler).</span><span class="sxs-lookup"><span data-stu-id="8e73a-118">**Find and list Native applications alone**: Run the following command to get all the native client (desktop/mobile device) applications.</span></span>

    <span data-ttu-id="8e73a-119">Get-AzureADApplication -Semua:$true | Where-Object { $_. PublicClient -eq $true } | FT</span><span class="sxs-lookup"><span data-stu-id="8e73a-119">Get-AzureADApplication -All:$true | Where-Object { $_.PublicClient -eq $true } | FT</span></span>
6. <span data-ttu-id="8e73a-120">**Ekspor Semua Detail Aplikasi Azure AD terdaftar ke CSV:** Perintah di bawah ini mengekspor semua aplikasi Azure AD dengan detail yang diperlukan ke file csv:</span><span class="sxs-lookup"><span data-stu-id="8e73a-120">**Export All Registered Azure AD Application Details to CSV**: The below command exports all the Azure AD apps with required details to csv file:</span></span>

    - <span data-ttu-id="8e73a-121">Get-AzureADApplication -Semua:$true | Select-Object DisplayName, AppID, PublicClient, AvailableToOtherTenants, HomePage, LogoutUrl |</span><span class="sxs-lookup"><span data-stu-id="8e73a-121">Get-AzureADApplication -All:$true | Select-Object DisplayName, AppID, PublicClient, AvailableToOtherTenants, HomePage, LogoutUrl |</span></span>
    - <span data-ttu-id="8e73a-122">Export-Csv "C:\AzureADApps.csv" -NoTypeInformation -Encoding UTF8</span><span class="sxs-lookup"><span data-stu-id="8e73a-122">Export-Csv "C:\AzureADApps.csv" -NoTypeInformation -Encoding UTF8</span></span>

7. <span data-ttu-id="8e73a-123">**Perlu mengekspor daftar aplikasi Azure yang tidak digunakan –** Laporan audit</span><span class="sxs-lookup"><span data-stu-id="8e73a-123">**Need to export a list of unused Azure apps** – Audit report</span></span>

    <span data-ttu-id="8e73a-124">Azure AD hanya dapat memperlihatkan log aplikasi hingga 30 hari jika Anda memiliki lisensi Azure AD Premium.</span><span class="sxs-lookup"><span data-stu-id="8e73a-124">Azure AD can show application logs for only up to 30 days provided you have Azure AD Premium license.</span></span>
    <span data-ttu-id="8e73a-125">Anda memiliki dua opsi untuk mempertahankan data lebih dari 30 hari.</span><span class="sxs-lookup"><span data-stu-id="8e73a-125">You have two options to retain the data for longer than 30 days.</span></span> <span data-ttu-id="8e73a-126">Anda dapat menggunakan [API Pelaporan Azure AD untuk](https://docs.microsoft.com/azure/active-directory/reports-monitoring/concept-reporting-api) mengambil data secara terprogram dan menyimpannya dalam database.</span><span class="sxs-lookup"><span data-stu-id="8e73a-126">You can use the [Azure AD Reporting APIs](https://docs.microsoft.com/azure/active-directory/reports-monitoring/concept-reporting-api) to retrieve the data programmatically and store it in a database.</span></span> <span data-ttu-id="8e73a-127">Alternatifnya, Anda dapat mengintegrasikan log audit ke sistem TERVERIFIKASI pihak ketiga.</span><span class="sxs-lookup"><span data-stu-id="8e73a-127">Alternatively, you can integrate audit logs into a third party SIEM system.</span></span>

    <span data-ttu-id="8e73a-128">Anda juga dapat mengunduh daftar aplikasi untuk semua aplikasi dan aplikasi yang dimiliki di bawah Azure Active directory>App Registrations>Unduh>Semua aplikasi/aplikasi yang dimiliki.</span><span class="sxs-lookup"><span data-stu-id="8e73a-128">You can also download the app list for all applications and owned applications under Azure Active directory>App Registrations>Download>All applications/Owned applications.</span></span>

    <span data-ttu-id="8e73a-129">Untuk mendapatkan daftar aplikasi melalui MS Graph, lihat Daftar aplikasi [- Microsoft Graph v1.0](https://docs.microsoft.com/graph/api/application-list) dan tipe sumber daya aplikasi [- Microsoft Graph v1.0](https://docs.microsoft.com/graph/api/resources/application).</span><span class="sxs-lookup"><span data-stu-id="8e73a-129">To get a list of applications through MS Graph, see [List applications - Microsoft Graph v1.0](https://docs.microsoft.com/graph/api/application-list) and [application resource type - Microsoft Graph v1.0](https://docs.microsoft.com/graph/api/resources/application).</span></span>
