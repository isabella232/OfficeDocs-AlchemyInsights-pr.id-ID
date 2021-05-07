---
title: Menyebarkan add-in untuk Aplikasi Microsoft 365
ms.author: pebaum
author: pebaum
manager: scotv
ms.date: 04/30/2021
ms.audience: Admin
ms.topic: article
ms.service: o365-administration
ROBOTS: NOINDEX, NOFOLLOW
localization_priority: Normal
ms.collection: Adm_O365
ms.custom:
- "11107"
- "9005477"
ms.openlocfilehash: a878a35ba9b530ce22ca7c263d20bd942d6896a8
ms.sourcegitcommit: 6c6b0c3885f33b08db929fe0b6496508d31fa2d6
ms.translationtype: MT
ms.contentlocale: id-ID
ms.lasthandoff: 05/06/2021
ms.locfileid: "52233537"
---
# <a name="deploying-add-ins-for-microsoft-365-apps"></a><span data-ttu-id="802ea-102">Menyebarkan add-in untuk Aplikasi Microsoft 365</span><span class="sxs-lookup"><span data-stu-id="802ea-102">Deploying add-ins for Microsoft 365 Apps</span></span>

<span data-ttu-id="802ea-103">Penyebaran Terpusat adalah cara yang disarankan untuk menyebarkan add-in Office kepada pengguna dan grup dalam organisasi Anda.</span><span class="sxs-lookup"><span data-stu-id="802ea-103">Centralized Deployment is the recommended way for deploying Office add-ins to users and groups within your organization.</span></span> <span data-ttu-id="802ea-104">Untuk menyebarkan add-in, ikuti langkah-langkah di bawah ini:</span><span class="sxs-lookup"><span data-stu-id="802ea-104">To deploy add-ins, follow the steps below:</span></span>

<span data-ttu-id="802ea-105">**Catatan:** Untuk menginstal add-in bagi Office pengguna individu, lihat Menampilkan, mengelola, dan menginstal [add-in Office tertentu.](https://support.microsoft.com/topic/view-manage-and-install-add-ins-in-office-programs-16278816-1948-4028-91e5-76dca5380f8d)</span><span class="sxs-lookup"><span data-stu-id="802ea-105">**Note:** To install add-ins for Office as an individual user, see [View, manage, and install add-ins in Office programs](https://support.microsoft.com/topic/view-manage-and-install-add-ins-in-office-programs-16278816-1948-4028-91e5-76dca5380f8d).</span></span> <span data-ttu-id="802ea-106">Selain itu, pastikan akuisisi individual Office add-in Bursa telah diaktifkan.</span><span class="sxs-lookup"><span data-stu-id="802ea-106">Also, make sure that individual acquisition of Office Store add-ins is enabled.</span></span> <span data-ttu-id="802ea-107">Untuk detailnya, [lihat Mencegah pengunduhan add-in dengan](https://docs.microsoft.com/microsoft-365/admin/manage/manage-addins-in-the-admin-center?view=o365-worldwide#prevent-add-in-downloads-by-turning-off-the-office-store-across-all-clients-except-outlook)menonaktifkan Bursa Office di semua klien (Kecuali Outlook) .</span><span class="sxs-lookup"><span data-stu-id="802ea-107">For details, see [Prevent add-in downloads by turning off the Office Store across all clients (Except Outlook)](https://docs.microsoft.com/microsoft-365/admin/manage/manage-addins-in-the-admin-center?view=o365-worldwide#prevent-add-in-downloads-by-turning-off-the-office-store-across-all-clients-except-outlook).</span></span>

1. <span data-ttu-id="802ea-108">Pastikan lingkungan Anda memenuhi persyaratan penyebaran add-in menggunakan Penyebaran Terpusat.</span><span class="sxs-lookup"><span data-stu-id="802ea-108">Ensure that your environment meets the requirements for deployment of add-ins using Centralized Deployment.</span></span> <span data-ttu-id="802ea-109">Untuk detailnya, lihat [Persyaratan.](https://docs.microsoft.com/microsoft-365/admin/manage/centralized-deployment-of-add-ins?#requirements)</span><span class="sxs-lookup"><span data-stu-id="802ea-109">For details, see [Requirements](https://docs.microsoft.com/microsoft-365/admin/manage/centralized-deployment-of-add-ins?#requirements).</span></span>
2. <span data-ttu-id="802ea-110">Masuk ke **Pengaturan**  >  **Dapatkan Aplikasi**  >  **Terintegrasi** di Microsoft 365 admin pusat admin untuk menyebarkan add-in.</span><span class="sxs-lookup"><span data-stu-id="802ea-110">Go to **Settings** > **Integrated Apps** > **Get apps** in the Microsoft 365 admin center to deploy add-ins.</span></span> 

<span data-ttu-id="802ea-111">Catatan:</span><span class="sxs-lookup"><span data-stu-id="802ea-111">Notes:</span></span> 

- <span data-ttu-id="802ea-112">Aplikasi Terintegrasi mengharuskan admin memiliki izin Admin Global Exchange Admin.</span><span class="sxs-lookup"><span data-stu-id="802ea-112">Integrated Apps requires that the admin has Global Admin or Exchange Admin permissions.</span></span>

- <span data-ttu-id="802ea-113">Ketika menyebarkan add-in ke beberapa pengguna, kami menyarankan penetapan dilakukan menggunakan grup dan bukan pengguna individu.</span><span class="sxs-lookup"><span data-stu-id="802ea-113">When deploying add-ins to multiple users, we recommend making assignments by using groups instead of individual users.</span></span> <span data-ttu-id="802ea-114">Untuk detailnya, [lihat Pertimbangan saat menetapkan add-in ke pengguna dan grup](https://docs.microsoft.com/microsoft-365/admin/manage/manage-deployment-of-add-ins?view=o365-worldwide#considerations-when-assigning-an-add-in-to-users-and-groups).</span><span class="sxs-lookup"><span data-stu-id="802ea-114">For details, see [Considerations when assigning an add-in to users and groups](https://docs.microsoft.com/microsoft-365/admin/manage/manage-deployment-of-add-ins?view=o365-worldwide#considerations-when-assigning-an-add-in-to-users-and-groups).</span></span>

- <span data-ttu-id="802ea-115">Penyebaran Terpusat tidak mendukung pengguna dalam grup bertumpuk atau grup yang memiliki grup induk.</span><span class="sxs-lookup"><span data-stu-id="802ea-115">Centralized Deployment doesn't support users in nested groups or groups that have parent groups.</span></span> <span data-ttu-id="802ea-116">Untuk detailnya, [lihat Penetapan pengguna dan grup](https://docs.microsoft.com/microsoft-365/admin/manage/centralized-deployment-of-add-ins?view=o365-worldwide#user-and-group-assignments).</span><span class="sxs-lookup"><span data-stu-id="802ea-116">For details, see [User and group assignments](https://docs.microsoft.com/microsoft-365/admin/manage/centralized-deployment-of-add-ins?view=o365-worldwide#user-and-group-assignments).</span></span>

- <span data-ttu-id="802ea-117">Pastikan bahwa Layanan Manajemen Aplikasi Microsoft 365 (GUID: '0517ffae-825d-4aff-999e-3f2336b8a20a') telah diaktifkan untuk masuk bagi pengguna.</span><span class="sxs-lookup"><span data-stu-id="802ea-117">Ensure that the Microsoft 365 App Management Service (GUID: '0517ffae-825d-4aff-999e-3f2336b8a20a') is enabled for users to sign in.</span></span> <span data-ttu-id="802ea-118">Untuk detailnya, [lihat Mengonfigurasi properti aplikasi](https://docs.microsoft.com/azure/active-directory/manage-apps/add-application-portal-configure#configure-app-properties).</span><span class="sxs-lookup"><span data-stu-id="802ea-118">For details, see [Configure app properties](https://docs.microsoft.com/azure/active-directory/manage-apps/add-application-portal-configure#configure-app-properties).</span></span>

- <span data-ttu-id="802ea-119">Jika Anda mengalami masalah dalam menyebarkan add-in menggunakan Aplikasi Terintegrasi, coba sebarkan menggunakan [Add-In.](https://admin.microsoft.com/AdminPortal/Home?#/Settings/AddIns)</span><span class="sxs-lookup"><span data-stu-id="802ea-119">If you experience issues deploying add-ins by using Integrated Apps, try deploying by using [Add-Ins](https://admin.microsoft.com/AdminPortal/Home?#/Settings/AddIns).</span></span>

<span data-ttu-id="802ea-120">Untuk informasi selengkapnya, lihat:</span><span class="sxs-lookup"><span data-stu-id="802ea-120">For more information, see:</span></span>

<span data-ttu-id="802ea-121">[Menyebarkan add-in di pusat admin](https://docs.microsoft.com/microsoft-365/admin/manage/manage-deployment-of-add-ins) 
 [Mengelola add-in di pusat admin](https://docs.microsoft.com/microsoft-365/admin/manage/manage-addins-in-the-admin-center) 
 [Menggunakan cmdlet PowerShell Penyebaran Terpusat untuk mengelola add-in](https://docs.microsoft.com/microsoft-365/enterprise/use-the-centralized-deployment-powershell-cmdlets-to-manage-add-ins) 
 [Menerbitkan Office Add-in menggunakan Penyebaran Terpusat melalui pusat admin](https://docs.microsoft.com/office/dev/add-ins/publish/centralized-deployment#publish-an-office-add-in-via-centralized-deployment) 
 Microsoft 365 [Pemecahan masalah: Pengguna tidak melihat add-in](https://docs.microsoft.com/office365/troubleshoot/access-management/user-not-seeing-add-ins) 
 [Memecahkan masalah kesalahan pengguna Office Add-in](https://docs.microsoft.com/office/dev/add-ins/testing/testing-and-troubleshooting)</span><span class="sxs-lookup"><span data-stu-id="802ea-121">[Deploy add-ins in the admin center](https://docs.microsoft.com/microsoft-365/admin/manage/manage-deployment-of-add-ins)
[Manage add-ins in the admin center](https://docs.microsoft.com/microsoft-365/admin/manage/manage-addins-in-the-admin-center)
[Use the Centralized Deployment PowerShell cmdlets to manage add-ins](https://docs.microsoft.com/microsoft-365/enterprise/use-the-centralized-deployment-powershell-cmdlets-to-manage-add-ins)
[Publish Office Add-ins using Centralized Deployment via the Microsoft 365 admin center](https://docs.microsoft.com/office/dev/add-ins/publish/centralized-deployment#publish-an-office-add-in-via-centralized-deployment)
[Troubleshoot: User not seeing add-ins](https://docs.microsoft.com/office365/troubleshoot/access-management/user-not-seeing-add-ins)
[Troubleshoot user errors with Office Add-ins](https://docs.microsoft.com/office/dev/add-ins/testing/testing-and-troubleshooting)</span></span>