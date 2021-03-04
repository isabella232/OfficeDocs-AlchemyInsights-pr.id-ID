---
title: Penyebaran GPO
ms.author: v-aiyengar
author: AshaIyengar21
manager: dansimp
ms.date: 02/24/2021
ms.audience: Admin
ms.topic: article
ms.service: o365-administration
ROBOTS: NOINDEX, NOFOLLOW
localization_priority: Normal
ms.collection: Adm_O365
ms.custom:
- "9004400"
- "8602"
ms.openlocfilehash: d31f77e70e8456a4076a8146025f1f8ada977a06
ms.sourcegitcommit: 969219d6dff18d86d679d4d8741d1e39e4ce9539
ms.translationtype: MT
ms.contentlocale: id-ID
ms.lasthandoff: 03/03/2021
ms.locfileid: "50427568"
---
# <a name="gpo-deployment"></a><span data-ttu-id="65d04-102">Penyebaran GPO</span><span class="sxs-lookup"><span data-stu-id="65d04-102">GPO Deployment</span></span>

<span data-ttu-id="65d04-103">Pengaturan untuk objek pengguna dan komputer di layanan domain direktori aktif Azure (Azure AD DS) sering kali dikelola menggunakan objek kebijakan grup (GPO).</span><span class="sxs-lookup"><span data-stu-id="65d04-103">Settings for user and computer objects in Azure Active Directory Domain Services (Azure AD DS) are often managed using Group Policy Objects (GPOs).</span></span> <span data-ttu-id="65d04-104">Azure AD DS menyertakan GPO bawaan untuk pengguna AADDC dan AADDC.</span><span class="sxs-lookup"><span data-stu-id="65d04-104">Azure AD DS includes built-in GPOs for the AADDC Users and AADDC Computers containers.</span></span> <span data-ttu-id="65d04-105">Anda dapat mengustomisasi GPO bawaan ini untuk mengonfigurasi kebijakan grup sebagaimana diperlukan untuk lingkungan Anda.</span><span class="sxs-lookup"><span data-stu-id="65d04-105">You can customize these built-in GPOs to configure group policy as needed for your environment.</span></span> <span data-ttu-id="65d04-106">Anggota grup administrator Azure AD DC memiliki hak istimewa administrasi kebijakan grup di domain Azure AD DS, dan juga dapat membuat GPO kustom dan unit organisasi (OU).</span><span class="sxs-lookup"><span data-stu-id="65d04-106">Members of the Azure AD DC administrators group have group policy administration privileges in the Azure AD DS domain, and can also create custom GPOs and organizational units (OUs).</span></span> <span data-ttu-id="65d04-107">Untuk informasi selengkapnya tentang kebijakan grup dan cara kerjanya, lihat [gambaran umum kebijakan grup](https://docs.microsoft.com/previous-versions/windows/it-pro/windows-server-2012-R2-and-2012/hh831791(v=ws.11)).</span><span class="sxs-lookup"><span data-stu-id="65d04-107">For more information on what group policy is and how it works, see [Group Policy Overview](https://docs.microsoft.com/previous-versions/windows/it-pro/windows-server-2012-R2-and-2012/hh831791(v=ws.11)).</span></span>

<span data-ttu-id="65d04-108">Dalam lingkungan hibrid, kebijakan grup yang dikonfigurasi di lingkungan AD DS lokal tidak disinkronkan ke Azure AD DS.</span><span class="sxs-lookup"><span data-stu-id="65d04-108">In a hybrid environment, group policies configured in an on-premises AD DS environment aren't synchronized to Azure AD DS.</span></span> <span data-ttu-id="65d04-109">Untuk menentukan pengaturan konfigurasi untuk pengguna atau komputer di Azure AD DS, Edit salah satu GPO default atau buat GPO kustom.</span><span class="sxs-lookup"><span data-stu-id="65d04-109">To define configuration settings for users or computers in Azure AD DS, edit one of the default GPOs or create a custom GPO.</span></span>

<span data-ttu-id="65d04-110">Artikel ini [mengelola kebijakan grup](https://docs.microsoft.com/azure/active-directory-domain-services/manage-group-policy) memperlihatkan kepada Anda cara menginstal alat manajemen kebijakan grup, bagaimana ton mengedit GPO bawaan, dan cara membuat GPO kustom.</span><span class="sxs-lookup"><span data-stu-id="65d04-110">This article [Manage Group Policy](https://docs.microsoft.com/azure/active-directory-domain-services/manage-group-policy) shows you how to install the Group Policy Management tools, how ton edit the built-in GPOs, and how to create custom GPOs.</span></span>
