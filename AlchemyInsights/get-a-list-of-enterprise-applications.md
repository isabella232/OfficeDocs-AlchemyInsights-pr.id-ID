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
ms.openlocfilehash: 99e4f7e676610103355736ce847930c6c5d2d7532c4756ac4551a8d9b3020176
ms.sourcegitcommit: b5f7da89a650d2915dc652449623c78be6247175
ms.translationtype: MT
ms.contentlocale: id-ID
ms.lasthandoff: 08/05/2021
ms.locfileid: "54116731"
---
# <a name="get-a-list-of-enterprise-applications"></a>Mendapatkan daftar Aplikasi Perusahaan

1. Untuk **mendapatkan** daftar aplikasi perusahaan (semua aplikasi atau yang difilter menurut Tampilkan nama, ID, Pengidentifikasi URI, dll.) melalui perintah Powershell, lihat [Get-AzureADApplication (AzureAD).](https://docs.microsoft.com/powershell/module/azuread/get-azureadapplication)
2. Untuk mendapatkan daftar objek prinsipal layanan (semua objek atau difilter menurut ID) melalui perintah Powershell, lihat [Get-AzureADServicePrincipal (AzureAD).](https://docs.microsoft.com/powershell/module/azuread/get-azureadserviceprincipal)
3. Jika Anda ingin **mendapatkan daftar aplikasi yang dikonfigurasi SAML, skrip PowerShell berikut ini** mungkin membantu Anda:

    Setiap Aplikasi yang menggunakan aplikasi OAuth atau aplikasi SAML (aplikasi galeri dan non-galeri) memiliki dua objek yang dibuat di AAD saat registrasi terjadi. Yang pertama disebut Objek Aplikasi dan yang lainnya adalah objek Prinsipal Layanan. Ketika Anda membuang properti Objek Prinsipal Layanan menggunakan PowerShell, Anda akan mendapati bahwa setiap aplikasi memiliki sejumlah Tag tertentu yang terkait dengannya seperti:

    - Aplikasi OAuth memiliki tag yang disebut "**WindowsAzureActiveDirectoryIntegratedApp**"
    - Aplikasi SAML Galeri akan memiliki tag disebut "**WindowsAzureActiveDirectoryGalleryApplicationPrimaryV1**"
    - Aplikasi SAML Non-Galeri akan memiliki tag bernama "**WindowsAzureActiveDirectoryCustomSingleSignOnApplication**"

    Karenanya, Anda bisa menggunakan tag ini dan mencari tahu jenis aplikasinya. Tag "**WindowsAzureActiveDirectoryIntegratedApp**" umum digunakan untuk semua tipe aplikasi. Anda dapat menggunakan snippet berikut untuk mencantumkan semua aplikasi SAML (baik galeri maupun non galeri):

    `$type = "SAML APP"`

    `Get-AzureADServicePrincipal -All true | Where-Object {(.Tags -contains "WindowsAzureActiveDirectoryGalleryApplicationNonPrimaryV1") -or (_.Tags -contains "WindowsAzureActiveDirectoryCustomSingleSignOnApplication")} | Select DisplayName, @{Name="AppType"; Expression={type}}_.`

    Untuk informasi selengkapnya, lihat [Mengidentifikasi aplikasi yang mendukung SAML di Azure AD](https://docs.microsoft.com/answers/questions/24259/identify-saml-enabled-apps-in-azure-ad.html).

4. **Hanya menemukan dan mencantumkan aplikasi Web:** Gunakan perintah di bawah ini untuk mendapatkan semua aplikasi Azure AD dengan tipe aplikasi "Web app/API"

    Get-AzureADApplication -Semua:$true | Where-Object { $_. PublicClient -ne $true } | FT
5. **Temukan dan list Aplikasi asli** saja: Jalankan perintah berikut untuk mendapatkan semua aplikasi klien asli (desktop/perangkat seluler).

    Get-AzureADApplication -Semua:$true | Where-Object { $_. PublicClient -eq $true } | FT
6. **Ekspor Semua Detail Aplikasi Azure AD terdaftar ke CSV:** Perintah di bawah ini mengekspor semua aplikasi Azure AD dengan detail yang diperlukan ke file csv:

    - Get-AzureADApplication -Semua:$true | Select-Object DisplayName, AppID, PublicClient, AvailableToOtherTenants, HomePage, LogoutUrl |
    - Export-Csv "C:\AzureADApps.csv" -NoTypeInformation -Encoding UTF8

7. **Perlu mengekspor daftar aplikasi Azure yang tidak digunakan –** Laporan audit

    Azure AD hanya dapat memperlihatkan log aplikasi hingga 30 hari jika Anda memiliki lisensi Azure AD Premium baru.
    Anda memiliki dua opsi untuk mempertahankan data lebih dari 30 hari. Anda dapat menggunakan [API Pelaporan Azure AD untuk](https://docs.microsoft.com/azure/active-directory/reports-monitoring/concept-reporting-api) mengambil data secara terprogram dan menyimpannya dalam database. Alternatifnya, Anda dapat mengintegrasikan log audit ke sistem TERVERIFIKASI pihak ketiga.

    Anda juga dapat mengunduh daftar aplikasi untuk semua aplikasi dan aplikasi yang dimiliki di bawah Azure Active directory>App Registrations>Unduh>Semua aplikasi/aplikasi yang dimiliki.

    Untuk mendapatkan daftar aplikasi melalui MS Graph, lihat Aplikasi daftar [- Microsoft Graph v1.0](https://docs.microsoft.com/graph/api/application-list) dan tipe sumber daya aplikasi [- Microsoft Graph v1.0](https://docs.microsoft.com/graph/api/resources/application).
