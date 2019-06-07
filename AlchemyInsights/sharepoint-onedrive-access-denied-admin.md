---
title: Mengatasi masalah Akses ditolak pesan
ms.author: kirks
author: Techwriter40
ms.date: 6/29/2018
ms.audience: ITPro
ms.topic: article
ROBOTS: NOINDEX, NOFOLLOW
localization_priority: Normal
ms.assetid: d678b57a-53ad-4414-9423-d8726a0c532f
ms.openlocfilehash: c204f1889e03886fdfd3d1c760a4a2beb82b0836
ms.sourcegitcommit: 4b7e478ce700c0b781efec3857ac4dce5bdf00c6
ms.translationtype: MT
ms.contentlocale: id-ID
ms.lasthandoff: 06/07/2019
ms.locfileid: "34760344"
---
# <a name="troubleshoot-access-denied-messages-in-sharepointonedrive-admin-center"></a><span data-ttu-id="83d11-102">Mengatasi masalah Akses ditolak pesan di Sharepoint OneDrive Admin Center</span><span class="sxs-lookup"><span data-stu-id="83d11-102">Troubleshoot Access Denied messages in Sharepoint/OneDrive Admin Center</span></span>

<span data-ttu-id="83d11-103">Jika Anda menerima Akses ditolak pesan ketika mencoba untuk menelusuri Sharepoint OneDrive Admin Center, pastikan bahwa Anda [menetapkan lisensi ke pengguna](https://docs.microsoft.com/office365/admin/subscriptions-and-billing/assign-licenses-to-users?view=o365-worldwide&amp;tabs=One).</span><span class="sxs-lookup"><span data-stu-id="83d11-103">If you are receiving an access denied message when attempting to browse to a Sharepoint/OneDrive Admin Center, please make sure that you [assign a license to the user](https://docs.microsoft.com/office365/admin/subscriptions-and-billing/assign-licenses-to-users?view=o365-worldwide&amp;tabs=One).</span></span> <span data-ttu-id="83d11-104">Jika pengguna memiliki lisensi, Anda juga harus memastikan mereka adalah [menetapkan peran administrator](https://docs.microsoft.com/office365/admin/add-users/about-admin-roles?view=o365-worldwide) yang dapat mengakses pusat admin.</span><span class="sxs-lookup"><span data-stu-id="83d11-104">If the user has a license, you should also make sure they are [assigned an administrator role](https://docs.microsoft.com/office365/admin/add-users/about-admin-roles?view=o365-worldwide) that can access the admin centers.</span></span>

<span data-ttu-id="83d11-105">Masalah ini juga dapat terjadi ketika pengguna dihapus dan kembali dibuat dengan sama pengguna (UPN nama dasar).</span><span class="sxs-lookup"><span data-stu-id="83d11-105">This issue can also occur when a user is deleted and re-created with the same user principal name (UPN).</span></span> <span data-ttu-id="83d11-106">Account yang baru dibuat dengan menggunakan PUID (paspor unik ID) nilai yang berbeda.</span><span class="sxs-lookup"><span data-stu-id="83d11-106">The new account is created by using a different PUID (Passport Unique ID) value.</span></span> <span data-ttu-id="83d11-107">Ketika pengguna mencoba untuk mengakses situs koleksi atau OneDrive mereka, pengguna memiliki PUID salah.</span><span class="sxs-lookup"><span data-stu-id="83d11-107">When the user tries to access a site collection or their OneDrive, the user has an incorrect PUID.</span></span> <span data-ttu-id="83d11-108">Skenario yang kedua melibatkan sinkronisasi direktori dengan unit organisasi Active Directory (OU).</span><span class="sxs-lookup"><span data-stu-id="83d11-108">A second scenario involves directory synchronization with an Active Directory organizational unit (OU).</span></span> <span data-ttu-id="83d11-109">Jika pengguna telah sudah masuk ke SharePoint, dan kemudian pindah ke OU berbeda dan resynced dengan SharePoint, mereka mungkin mengalami masalah ini.</span><span class="sxs-lookup"><span data-stu-id="83d11-109">If users have already signed in to SharePoint, and then are moved to a different OU and resynced with SharePoint, they may experience this problem.</span></span>

<span data-ttu-id="83d11-110">Untuk mengatasi masalah ini, Anda harus mengembalikan UPN asli dengan langkah-langkah dalam artikel, [mengembalikan pengguna di Office 365](https://docs.microsoft.com/office365/admin/add-users/restore-user?view=o365-worldwide).</span><span class="sxs-lookup"><span data-stu-id="83d11-110">To resolve this issue, you should restore the original UPN with the steps in the article, [Restore a user in Office 365](https://docs.microsoft.com/office365/admin/add-users/restore-user?view=o365-worldwide).</span></span>

<span data-ttu-id="83d11-111">Catatan: Jika pusat OneDrive atau SharePoint Admin tidak tersedia untuk beberapa pengguna yang sebelumnya mempunyai akses, mungkin ada masalah sementara layanan.</span><span class="sxs-lookup"><span data-stu-id="83d11-111">Note: If a OneDrive or SharePoint Admin center is not available to multiple users who previously had access, there may be a temporary service issue.</span></span>  <span data-ttu-id="83d11-112">[Periksa layanan kesehatan dashboard](https://portal.office.com/adminportal/home#/servicehealth).</span><span class="sxs-lookup"><span data-stu-id="83d11-112">[Check the service health dashboard](https://portal.office.com/adminportal/home#/servicehealth).</span></span>


