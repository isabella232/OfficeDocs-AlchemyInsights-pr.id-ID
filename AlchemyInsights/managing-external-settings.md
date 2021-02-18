---
title: Mengelola pengaturan eksternal
ms.author: pebaum
author: pebaum
manager: scotv
ms.date: 02/10/2021
ms.audience: Admin
ms.topic: article
ms.service: o365-administration
ROBOTS: NOINDEX, NOFOLLOW
localization_priority: Priority
ms.collection: Adm_O365
ms.custom:
- "8322"
- "9003227"
ms.openlocfilehash: 7caf46f9988ddbcbb16c0a2751dbda85bd7da34c
ms.sourcegitcommit: 616ae0cbd5769e12ae428e00088840cf05e52b6a
ms.translationtype: MT
ms.contentlocale: id-ID
ms.lasthandoff: 02/17/2021
ms.locfileid: "50294317"
---
# <a name="managing-external-settings"></a><span data-ttu-id="f84ba-102">Mengelola pengaturan eksternal</span><span class="sxs-lookup"><span data-stu-id="f84ba-102">Managing External Settings</span></span>

<span data-ttu-id="f84ba-103">**Pengumuman**</span><span class="sxs-lookup"><span data-stu-id="f84ba-103">**Announcement**</span></span>

- <span data-ttu-id="f84ba-104">[Penghentian dukungan masuk WebView dari Google mulai 4 januari 2021](https://docs.microsoft.com/azure/active-directory/external-identities/google-federation?WT.mc_id=Portal-Microsoft_Azure_Support#deprecation-of-webview-sign-in-support).</span><span class="sxs-lookup"><span data-stu-id="f84ba-104">[Deprecation of WebView sign-in support from Google starting January 4, 2021](https://docs.microsoft.com/azure/active-directory/external-identities/google-federation?WT.mc_id=Portal-Microsoft_Azure_Support#deprecation-of-webview-sign-in-support).</span></span> <span data-ttu-id="f84ba-105">Menguji apakah aplikasi terpengaruh oleh mengikuti Panduan Google tentang kompatibilitas pengujian</span><span class="sxs-lookup"><span data-stu-id="f84ba-105">Test whether your apps are affected by following Google’s guidance on testing compatibility</span></span>
- <span data-ttu-id="f84ba-106">Pastikan untuk menggunakan WebView sistem atau browser sistem saat masuk ke pengguna Anda dengan akun Google konsumen</span><span class="sxs-lookup"><span data-stu-id="f84ba-106">Make sure to use the system webview or the system browser when signing in your users with consumer Google accounts</span></span>

<span data-ttu-id="f84ba-107">**Mengelola pengaturan undangan**</span><span class="sxs-lookup"><span data-stu-id="f84ba-107">**Manage Invitation Settings**</span></span>

<span data-ttu-id="f84ba-108">Konfirmasi bahwa Anda telah [mengonfigurasi pengaturan kolaborasi eksternal](https://docs.microsoft.com/azure/active-directory/external-identities/delegate-invitations?WT.mc_id=Portal-Microsoft_Azure_Support) untuk memperbolehkan orang yang tepat mengirimkan undangan.</span><span class="sxs-lookup"><span data-stu-id="f84ba-108">Confirm that you have [configured the external collaboration settings](https://docs.microsoft.com/azure/active-directory/external-identities/delegate-invitations?WT.mc_id=Portal-Microsoft_Azure_Support) to allow the appropriate people to send invitations.</span></span>

<span data-ttu-id="f84ba-109">**Mengelola izin akses pengguna tamu**</span><span class="sxs-lookup"><span data-stu-id="f84ba-109">**Manage Guest User Access Permissions**</span></span>

1. <span data-ttu-id="f84ba-110">Admin global dapat mengelola izin akses tamu dalam direktori melalui portal Azure dengan mengonfigurasi izin akses tamu pada halaman pengaturan kolaborasi eksternal.</span><span class="sxs-lookup"><span data-stu-id="f84ba-110">Global admins can manage guest access permissions in the directory through the Azure portal by configuring the guest access permissions on the External Collaboration Settings page.</span></span> <span data-ttu-id="f84ba-111">[Pelajari selengkapnya tentang pengaturan ini](https://docs.microsoft.com/azure/active-directory/fundamentals/users-default-permissions?WT.mc_id=Portal-Microsoft_Azure_Support).</span><span class="sxs-lookup"><span data-stu-id="f84ba-111">[Learn more about this setting](https://docs.microsoft.com/azure/active-directory/fundamentals/users-default-permissions?WT.mc_id=Portal-Microsoft_Azure_Support).</span></span>
2. <span data-ttu-id="f84ba-112">Jika Anda ingin agar tamu mengakses aplikasi seperti teams atau SharePoint, pastikan bahwa Anda telah mengonfigurasi aplikasi tersebut untuk memperbolehkan akses tamu.</span><span class="sxs-lookup"><span data-stu-id="f84ba-112">If you would like your guests to access apps such as Teams or SharePoint, confirm that you've configured those apps to allow guest access.</span></span> <span data-ttu-id="f84ba-113">Pelajari selengkapnya tentang [pengaturan tim](https://docs.microsoft.com/microsoftteams/guest-access?WT.mc_id=Portal-Microsoft_Azure_Support) dan [SharePoint](https://docs.microsoft.com/sharepoint/external-sharing-overview?WT.mc_id=Portal-Microsoft_Azure_Support).</span><span class="sxs-lookup"><span data-stu-id="f84ba-113">Learn more about the [Teams settings](https://docs.microsoft.com/microsoftteams/guest-access?WT.mc_id=Portal-Microsoft_Azure_Support) and [SharePoint](https://docs.microsoft.com/sharepoint/external-sharing-overview?WT.mc_id=Portal-Microsoft_Azure_Support).</span></span>

<span data-ttu-id="f84ba-114">**Mengonfigurasi undangan:**</span><span class="sxs-lookup"><span data-stu-id="f84ba-114">**Configuring invitations:**</span></span>

- [<span data-ttu-id="f84ba-115">Aktifkan kolaborasi eksternal B2B dan Kelola siapa yang bisa mengundang tamu</span><span class="sxs-lookup"><span data-stu-id="f84ba-115">Enable B2B external collaboration and manage who can invite guests</span></span>](https://docs.microsoft.com/azure/active-directory/b2b/delegate-invitations?WT.mc_id=Portal-Microsoft_Azure_Support)
- [<span data-ttu-id="f84ba-116">Memperbolehkan atau memblokir undangan kepada pengguna dari organisasi tertentu</span><span class="sxs-lookup"><span data-stu-id="f84ba-116">Allow or block invitations to users from specific organizations</span></span>](https://docs.microsoft.com/azure/active-directory/b2b/allow-deny-list?WT.mc_id=Portal-Microsoft_Azure_Support)

<span data-ttu-id="f84ba-117">**Mengonfigurasi penyedia identitas yang diperbolehkan:**</span><span class="sxs-lookup"><span data-stu-id="f84ba-117">**Configuring allowed identity providers:**</span></span>

- [<span data-ttu-id="f84ba-118">Google Federation</span><span class="sxs-lookup"><span data-stu-id="f84ba-118">Google Federation</span></span>](https://docs.microsoft.com/azure/active-directory/b2b/google-federation?WT.mc_id=Portal-Microsoft_Azure_Support)
- [<span data-ttu-id="f84ba-119">Gabungan langsung</span><span class="sxs-lookup"><span data-stu-id="f84ba-119">Direct Federation</span></span>](https://docs.microsoft.com/azure/active-directory/b2b/direct-federation?WT.mc_id=Portal-Microsoft_Azure_Support)
- [<span data-ttu-id="f84ba-120">Autentikasi kode akses satu kali email</span><span class="sxs-lookup"><span data-stu-id="f84ba-120">Email one-time Passcode Authentication</span></span>](https://docs.microsoft.com/azure/active-directory/b2b/one-time-passcode?WT.mc_id=Portal-Microsoft_Azure_Support)
