---
title: Buat pengguna
ms.author: v-aiyengar
author: AshaIyengar21
manager: dansimp
ms.date: 03/11/2021
ms.audience: Admin
ms.topic: article
ms.service: o365-administration
ROBOTS: NOINDEX, NOFOLLOW
localization_priority: Normal
ms.collection: Adm_O365
ms.custom:
- "9003231"
- "9403"
ms.openlocfilehash: 800baae2d748708d8cb7a5fb0e73fce5dcf455cb
ms.sourcegitcommit: 2d617ae59eed0ce8b571339ceefce6473c03b94c
ms.translationtype: MT
ms.contentlocale: id-ID
ms.lasthandoff: 05/19/2021
ms.locfileid: "52569734"
---
# <a name="create-user"></a><span data-ttu-id="1ead9-102">Buat pengguna</span><span class="sxs-lookup"><span data-stu-id="1ead9-102">Create user</span></span>

<span data-ttu-id="1ead9-103">**PENGUMUMAN:**</span><span class="sxs-lookup"><span data-stu-id="1ead9-103">**ANNOUNCEMENT:**</span></span>

- <span data-ttu-id="1ead9-104">[Penghentian dukungan masuk WebView dari Google dimulai 4 Januari 2021.](/azure/active-directory/external-identities/google-federation#deprecation-of-webview-sign-in-support)</span><span class="sxs-lookup"><span data-stu-id="1ead9-104">[Deprecation of WebView sign-in support from Google starting January 4, 2021](/azure/active-directory/external-identities/google-federation#deprecation-of-webview-sign-in-support) .</span></span> <span data-ttu-id="1ead9-105">Uji apakah aplikasi Anda akan terpengaruh oleh [panduan Google tentang](https://go.microsoft.com/fwlink/?linkid=2157323) kompatibilitas pengujian.</span><span class="sxs-lookup"><span data-stu-id="1ead9-105">Test whether your apps may be affected by following [Google’s guidance](https://go.microsoft.com/fwlink/?linkid=2157323) on testing compatibility.</span></span>
- <span data-ttu-id="1ead9-106">Pastikan Anda menggunakan sistem webview atau browser sistem saat masuk pengguna Anda dengan akun Google konsumen.</span><span class="sxs-lookup"><span data-stu-id="1ead9-106">Make sure you use the system webview or system browser when signing in your users with consumer Google accounts.</span></span> <span data-ttu-id="1ead9-107">Untuk informasi selengkapnya, [lihat Masalah saat masuk ke aplikasi menggunakan browser Chrome saja](/office365/troubleshoot/miscellaneous/chrome-behavior-affects-applications).</span><span class="sxs-lookup"><span data-stu-id="1ead9-107">For more information, see [Issues signing in to application(s) using Chrome browser only](/office365/troubleshoot/miscellaneous/chrome-behavior-affects-applications).</span></span>

<span data-ttu-id="1ead9-108">**Saya tidak dapat membuat pengguna baru di direktori Azure AD**</span><span class="sxs-lookup"><span data-stu-id="1ead9-108">**I can't create a new user in my Azure AD directory**</span></span>

1. <span data-ttu-id="1ead9-109">Pastikan bahwa Anda memiliki wewenang untuk membuat pengguna standar baru.</span><span class="sxs-lookup"><span data-stu-id="1ead9-109">Ensure that you are authorized to create a new standard user.</span></span> <span data-ttu-id="1ead9-110">Hanya administrator global atau Peran administrator pengguna di Azure Active Directory (AD) yang bisa membuat pengguna standar baru.</span><span class="sxs-lookup"><span data-stu-id="1ead9-110">Only the Global administrator or User administrator role in Azure Active Directory (AD) can create a new standard user.</span></span> <span data-ttu-id="1ead9-111">Jika Anda tidak berada dalam salah satu peran ini, minta administrator untuk menambahkan Anda ke salah satu peran ini atau untuk membuat akun pengguna baru untuk Anda.</span><span class="sxs-lookup"><span data-stu-id="1ead9-111">If you're not in one of these roles, ask an administrator to add you to one of these roles or to create the new user account for you.</span></span>
1. <span data-ttu-id="1ead9-112">Pastikan bahwa nama pengguna berada di domain yang diverifikasi di Azure AD Anda.</span><span class="sxs-lookup"><span data-stu-id="1ead9-112">Ensure that the user name is in a domain that is verified in your Azure AD.</span></span> <span data-ttu-id="1ead9-113">Jika tidak memiliki nama domain kustom terverifikasi di Azure AD, Anda dapat menggunakan domain awal Azure AD, yang diakhiri dengan \*.onmicrosoft.com.</span><span class="sxs-lookup"><span data-stu-id="1ead9-113">If you do not have any verified custom domain names in your Azure AD, you can use your Azure AD initial domain, which ends with \*.onmicrosoft.com.</span></span>
1. <span data-ttu-id="1ead9-114">Pastikan bahwa nama pengguna berada di domain yang tidak t bagian dari Azure AD dari AD lokal Anda.</span><span class="sxs-lookup"><span data-stu-id="1ead9-114">Ensure that the user name is in a domain that is not federated to Azure AD from your on-premises AD.</span></span> <span data-ttu-id="1ead9-115">Pengguna tidak bisa ditambahkan di awan dengan nama domain yang di federasinya dari lokal.</span><span class="sxs-lookup"><span data-stu-id="1ead9-115">Users cannot be added in the cloud with domain names that are federated from on-premises.</span></span>
1. <span data-ttu-id="1ead9-116">Pastikan tidak ada pengguna atau kontak lain yang telah memiliki nama pengguna yang ingin Anda tetapkan ke pengguna baru.</span><span class="sxs-lookup"><span data-stu-id="1ead9-116">Ensure that no other user or contact already has the user name that you want to assign to the new user.</span></span> <span data-ttu-id="1ead9-117">Nama pengguna harus unik di Azure AD.</span><span class="sxs-lookup"><span data-stu-id="1ead9-117">User names must be unique across Azure AD.</span></span>
1. <span data-ttu-id="1ead9-118">Lihat [peran dan administrator Azure AD](https://portal.azure.com/#blade/Microsoft_AAD_IAM/ActiveDirectoryMenuBlade/RolesAndAdministrators) untuk Azure AD Anda.</span><span class="sxs-lookup"><span data-stu-id="1ead9-118">See [Azure AD roles and administrators](https://portal.azure.com/#blade/Microsoft_AAD_IAM/ActiveDirectoryMenuBlade/RolesAndAdministrators) for your Azure AD.</span></span>
1. <span data-ttu-id="1ead9-119">Lihat nama [domain untuk](https://portal.azure.com/#blade/Microsoft_AAD_IAM/ActiveDirectoryMenuBlade/RolesAndAdministrators) Azure AD Anda.</span><span class="sxs-lookup"><span data-stu-id="1ead9-119">See the [domain names](https://portal.azure.com/#blade/Microsoft_AAD_IAM/ActiveDirectoryMenuBlade/RolesAndAdministrators) for your Azure AD.</span></span>
1. <span data-ttu-id="1ead9-120">Tinjau [Log audit](https://portal.azure.com/#blade/Microsoft_AAD_IAM/ActiveDirectoryMenuBlade/RolesAndAdministrators) untuk melihat informasi lebih mendetail tentang pengguna yang baru dibuat atau dihapus seperti siapa yang melakukan tindakan dan kapan.</span><span class="sxs-lookup"><span data-stu-id="1ead9-120">Review [Audit logs](https://portal.azure.com/#blade/Microsoft_AAD_IAM/ActiveDirectoryMenuBlade/RolesAndAdministrators) to see more detailed information about a recently created or deleted user like who performed the action and when.</span></span>
1. <span data-ttu-id="1ead9-121">Untuk informasi selengkapnya tentang menambahkan pengguna baru, [lihat Menggunakan portal Azure untuk membuat pengguna baru di Azure AD](/azure/active-directory/active-directory-users-create-azure-portal).</span><span class="sxs-lookup"><span data-stu-id="1ead9-121">For more information on adding new users, see [Use the Azure portal to create a new user in your Azure AD](/azure/active-directory/active-directory-users-create-azure-portal).</span></span>
1. <span data-ttu-id="1ead9-122">[Peran administratif Azure AD](/azure/active-directory/active-directory-assign-admin-roles): Izin peran administrator di Azure Active Directory</span><span class="sxs-lookup"><span data-stu-id="1ead9-122">[Azure AD administrative roles](/azure/active-directory/active-directory-assign-admin-roles): Administrator role permissions in Azure Active Directory</span></span>
1. <span data-ttu-id="1ead9-123">Anda juga dapat [menggunakan Azure AD PowerShell untuk membuat pengguna baru.](/powershell/module/azuread/new-azureaduser?view=azureadps-2.0)</span><span class="sxs-lookup"><span data-stu-id="1ead9-123">You can also [use Azure AD PowerShell to create a new user](/powershell/module/azuread/new-azureaduser?view=azureadps-2.0).</span></span>
