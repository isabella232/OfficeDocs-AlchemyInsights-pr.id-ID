---
title: Masalah Pemilik Pendaftaran Aplikasi
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
- "9004352"
- "9655"
ms.openlocfilehash: 9dc3b1d54bb263d5e53e02a4e4dadc8cf3c1e400
ms.sourcegitcommit: 1f43598a726cdb9904aa501eb8db87f143020d9e
ms.translationtype: MT
ms.contentlocale: id-ID
ms.lasthandoff: 03/23/2021
ms.locfileid: "51404776"
---
# <a name="app-registration-owner-issues"></a><span data-ttu-id="d8342-102">Masalah Pemilik Pendaftaran Aplikasi</span><span class="sxs-lookup"><span data-stu-id="d8342-102">App Registration Owner issues</span></span>

<span data-ttu-id="d8342-103">Berikut adalah metode yang tersedia untuk menambahkan prinsipal sebagai pemilik bagi pendaftaran aplikasi:</span><span class="sxs-lookup"><span data-stu-id="d8342-103">Following are the available methods to add principals as owners for app registrations:</span></span>

- <span data-ttu-id="d8342-104">Menggunakan Modul PowerShell Azure AD -</span><span class="sxs-lookup"><span data-stu-id="d8342-104">Using Azure AD PowerShell Module -</span></span>

    `Connect-AzureAd`

    `Add-AzureADApplicationOwner -ObjectId <Application ObjectId>-RefObjectId <ObjectID of principal to assign as owner>`

    <span data-ttu-id="d8342-105">Referensi: [Add-AzureADApplicationOwner (AzureAD)](https://docs.microsoft.com/powershell/module/azuread/add-azureadapplicationowner)</span><span class="sxs-lookup"><span data-stu-id="d8342-105">Reference: [Add-AzureADApplicationOwner (AzureAD)](https://docs.microsoft.com/powershell/module/azuread/add-azureadapplicationowner)</span></span>
- <span data-ttu-id="d8342-106">Menggunakan Azure CLI - `az ad app owner add`</span><span class="sxs-lookup"><span data-stu-id="d8342-106">Using Azure CLI - `az ad app owner add`</span></span>

    <span data-ttu-id="d8342-107">Referensi: [pemilik aplikasi az ad](https://docs.microsoft.com/cli/azure/ad/app/owner)</span><span class="sxs-lookup"><span data-stu-id="d8342-107">Reference: [az ad app owner](https://docs.microsoft.com/cli/azure/ad/app/owner)</span></span>
- <span data-ttu-id="d8342-108">Menggunakan MS Graph -</span><span class="sxs-lookup"><span data-stu-id="d8342-108">Using MS Graph -</span></span>

    <span data-ttu-id="d8342-109">Referensi: [Menambahkan pemilik - Microsoft Graph v1.0](https://docs.microsoft.com/graph/api/application-post-owners)</span><span class="sxs-lookup"><span data-stu-id="d8342-109">Reference: [Add owner - Microsoft Graph v1.0](https://docs.microsoft.com/graph/api/application-post-owners)</span></span>
- <span data-ttu-id="d8342-110">Menggunakan Portal Azure AD - Navigasikan [ke portal.azure.com](https://portal.azure.com/) > Azure Active directory > Pendaftaran Aplikasi > Pilih aplikasi Anda > Pemilik > Tambahkan Pemilik</span><span class="sxs-lookup"><span data-stu-id="d8342-110">Using the Azure AD Portal - Navigate to [portal.azure.com](https://portal.azure.com/) > Azure Active directory > App Registration > Select your application > Owners > Add Owners</span></span>

<span data-ttu-id="d8342-111">**Tidak dapat menampilkan aplikasi Anda di App Registrations blade meskipun Anda adalah pemilik aplikasi tersebut?**</span><span class="sxs-lookup"><span data-stu-id="d8342-111">**Cannot view your application on App Registrations blade even though you are the owner of that application?**</span></span>

<span data-ttu-id="d8342-112">Pemilik aplikasi bukanlah peran administratif.</span><span class="sxs-lookup"><span data-stu-id="d8342-112">Owner of an app is not an administrative role.</span></span> <span data-ttu-id="d8342-113">Jika pengaturan [Batasi akses ke portal administrasi Azure AD](https://docs.microsoft.com/azure/active-directory/fundamentals/users-default-permissions) diaktifkan, maka hanya admin yang dapat menampilkan aplikasi di portal Pendaftaran Aplikasi.</span><span class="sxs-lookup"><span data-stu-id="d8342-113">If the setting [Restrict access to Azure AD administration portal](https://docs.microsoft.com/azure/active-directory/fundamentals/users-default-permissions) is enabled, then only admin will be able to view the applications on App Registration portal.</span></span> <span data-ttu-id="d8342-114">Agar pemilik dapat menampilkan aplikasi, nonaktifkan pengaturan ini (Atur ke TIDAK) atau tetapkan peran admin ke pemilik hanya untuk aplikasi tertentu.</span><span class="sxs-lookup"><span data-stu-id="d8342-114">For an owner to be able to view the applications, either disable this setting (Set this to NO) or assign admin role to the owner for only the specific application.</span></span> <span data-ttu-id="d8342-115">Namun, untuk hal ini, Anda akan memerlukan lisensi Azure AD Premium P2 dan mengaktifkan [Manajemen Identitas Hak Istimewa.](https://docs.microsoft.com/azure/active-directory/privileged-identity-management/pim-configure)</span><span class="sxs-lookup"><span data-stu-id="d8342-115">However for this, you will require an Azure AD Premium P2 license and enable [Privileged Identity Management](https://docs.microsoft.com/azure/active-directory/privileged-identity-management/pim-configure).</span></span>
