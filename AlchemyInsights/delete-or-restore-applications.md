---
title: Menghapus atau memulihkan aplikasi
ms.author: v-jmathew
author: v-jmathew
manager: scotv
ms.audience: Admin
ms.topic: article
ms.service: o365-administration
ROBOTS: NOINDEX, NOFOLLOW
localization_priority: Normal
ms.collection: Adm_O365
ms.custom:
- "9004335"
- "7737"
ms.openlocfilehash: 4df9a98644f6bc7a30f9009719c5198db591afc9
ms.sourcegitcommit: eb685eea3ab312d404d55bfd5594a5d6d68811d1
ms.translationtype: MT
ms.contentlocale: id-ID
ms.lasthandoff: 01/27/2021
ms.locfileid: "50014902"
---
# <a name="delete-or-restore-applications"></a><span data-ttu-id="19ffc-102">Menghapus atau memulihkan aplikasi</span><span class="sxs-lookup"><span data-stu-id="19ffc-102">Delete or restore applications</span></span>

<span data-ttu-id="19ffc-103">**Untuk menghapus aplikasi dari penyewa AZURE AD Anda**:</span><span class="sxs-lookup"><span data-stu-id="19ffc-103">**To delete an application from your Azure AD tenant**:</span></span>

1. <span data-ttu-id="19ffc-104">Di **portal AZURE AD**, pilih **aplikasi perusahaan**.</span><span class="sxs-lookup"><span data-stu-id="19ffc-104">In the **Azure AD portal**, select **Enterprise applications**.</span></span> <span data-ttu-id="19ffc-105">Lalu temukan dan pilih aplikasi yang ingin Anda hapus.</span><span class="sxs-lookup"><span data-stu-id="19ffc-105">Then find and select the application you want to delete.</span></span>
2. <span data-ttu-id="19ffc-106">Di bagian **Kelola** di panel kiri, pilih **properti**.</span><span class="sxs-lookup"><span data-stu-id="19ffc-106">In the **Manage** section in the left pane, select **Properties**.</span></span>
3. <span data-ttu-id="19ffc-107">Pilih **Hapus**, lalu pilih **ya** untuk mengonfirmasi bahwa Anda ingin menghapus aplikasi dari penyewa Azure AD Anda.</span><span class="sxs-lookup"><span data-stu-id="19ffc-107">Select **Delete**, and then select **Yes** to confirm you want to delete the app from your Azure AD tenant.</span></span>

<span data-ttu-id="19ffc-108">Untuk informasi selengkapnya tentang cara menghapus aplikasi, lihat [mulai cepat: menghapus aplikasi dari penyewa Azure Active Directory (AZURE AD) Anda](https://docs.microsoft.com/azure/active-directory/manage-apps/delete-application-portal#delete-an-application-from-your-azure-ad-tenant).</span><span class="sxs-lookup"><span data-stu-id="19ffc-108">For more information on how to delete an app, see [Quickstart: Delete an application from your Azure Active Directory (Azure AD) tenant](https://docs.microsoft.com/azure/active-directory/manage-apps/delete-application-portal#delete-an-application-from-your-azure-ad-tenant).</span></span>

<span data-ttu-id="19ffc-109">Di PowerShell, cmdlet [Remove-AzureADApplicationProxyApplication](https://docs.microsoft.com/powershell/module/azuread/remove-azureadapplicationproxyapplication) menghapus konfigurasi proksi aplikasi dari aplikasi tertentu di Azure Active Directory, dan dapat menghapus aplikasi sepenuhnya jika ditentukan.</span><span class="sxs-lookup"><span data-stu-id="19ffc-109">In PowerShell, the [Remove-AzureADApplicationProxyApplication](https://docs.microsoft.com/powershell/module/azuread/remove-azureadapplicationproxyapplication) cmdlet removes Application Proxy configurations from a specific application in Azure Active Directory, and can delete the application completely if specified.</span></span>

<span data-ttu-id="19ffc-110">Anda dapat **memulihkan aplikasi yang dihapus** menggunakan PowerShell.</span><span class="sxs-lookup"><span data-stu-id="19ffc-110">You can **restore a deleted application** using PowerShell.</span></span> <span data-ttu-id="19ffc-111">Setelah aplikasi yang ingin dipulihkan telah diidentifikasi, Anda dapat memulihkannya menggunakan [Pulihkan-Azureaddeletedapplikasi](https://docs.microsoft.com/powershell/module/azuread/restore-azureaddeletedapplication).</span><span class="sxs-lookup"><span data-stu-id="19ffc-111">Once the application you want to restore has been identified, you can restore it using [Restore-AzureADDeletedApplication](https://docs.microsoft.com/powershell/module/azuread/restore-azureaddeletedapplication).</span></span>
