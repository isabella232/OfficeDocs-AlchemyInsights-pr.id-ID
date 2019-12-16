---
title: Memecahkan masalah Akses ditolak pesan
ms.author: pebaum
author: pebaum
ms.date: 6/29/2018
ms.audience: ITPro
ms.topic: article
ROBOTS: NOINDEX, NOFOLLOW
localization_priority: Normal
ms.assetid: d678b57a-53ad-4414-9423-d8726a0c532f
ms.openlocfilehash: 57919e6dbd81a5bf3b17fb067485e8eec23b7d4c
ms.sourcegitcommit: 0f0186044a3597e42ad14c32ca58e7224344dcfa
ms.translationtype: MT
ms.contentlocale: id-ID
ms.lasthandoff: 12/15/2019
ms.locfileid: "40051428"
---
# <a name="troubleshoot-access-denied-messages-in-sharepointonedrive-admin-center"></a><span data-ttu-id="ea0ba-102">Memecahkan masalah Akses ditolak pesan di pusat admin SharePoint/OneDrive</span><span class="sxs-lookup"><span data-stu-id="ea0ba-102">Troubleshoot Access Denied messages in Sharepoint/OneDrive Admin Center</span></span>

<span data-ttu-id="ea0ba-103">Jika Anda menerima pesan Akses ditolak saat berusaha menjelajah ke Pusat admin SharePoint/OneDrive, pastikan bahwa Anda [menetapkan lisensi untuk pengguna](https://docs.microsoft.com/office365/admin/subscriptions-and-billing/assign-licenses-to-users?view=o365-worldwide&amp;tabs=One).</span><span class="sxs-lookup"><span data-stu-id="ea0ba-103">If you are receiving an access denied message when attempting to browse to a Sharepoint/OneDrive Admin Center, please make sure that you [assign a license to the user](https://docs.microsoft.com/office365/admin/subscriptions-and-billing/assign-licenses-to-users?view=o365-worldwide&amp;tabs=One).</span></span> <span data-ttu-id="ea0ba-104">Jika pengguna memiliki lisensi, Anda juga harus memastikan bahwa mereka [ditetapkan peran administrator](https://docs.microsoft.com/office365/admin/add-users/about-admin-roles?view=o365-worldwide) yang dapat mengakses pusat admin.</span><span class="sxs-lookup"><span data-stu-id="ea0ba-104">If the user has a license, you should also make sure they are [assigned an administrator role](https://docs.microsoft.com/office365/admin/add-users/about-admin-roles?view=o365-worldwide) that can access the admin centers.</span></span>

<span data-ttu-id="ea0ba-105">Masalah ini juga dapat terjadi ketika pengguna dihapus dan dibuat ulang dengan nama prinsip pengguna (UPN) yang sama.</span><span class="sxs-lookup"><span data-stu-id="ea0ba-105">This issue can also occur when a user is deleted and re-created with the same user principal name (UPN).</span></span> <span data-ttu-id="ea0ba-106">Akun baru dibuat dengan menggunakan nilai yang berbeda PUID (paspor unik ID).</span><span class="sxs-lookup"><span data-stu-id="ea0ba-106">The new account is created by using a different PUID (Passport Unique ID) value.</span></span> <span data-ttu-id="ea0ba-107">Saat pengguna berusaha mengakses koleksi situs atau OneDrive mereka, pengguna memiliki PUID salah.</span><span class="sxs-lookup"><span data-stu-id="ea0ba-107">When the user tries to access a site collection or their OneDrive, the user has an incorrect PUID.</span></span> <span data-ttu-id="ea0ba-108">Skenario kedua melibatkan sinkronisasi direktori dengan direktori aktif unit organisasi (OU).</span><span class="sxs-lookup"><span data-stu-id="ea0ba-108">A second scenario involves directory synchronization with an Active Directory organizational unit (OU).</span></span> <span data-ttu-id="ea0ba-109">Jika pengguna telah masuk ke SharePoint, dan kemudian dipindahkan ke OU berbeda dan resynced dengan SharePoint, mereka mungkin mengalami masalah ini.</span><span class="sxs-lookup"><span data-stu-id="ea0ba-109">If users have already signed in to SharePoint, and then are moved to a different OU and resynced with SharePoint, they may experience this problem.</span></span>

<span data-ttu-id="ea0ba-110">Untuk mengatasi masalah ini, Anda harus memulihkan UPN asli dengan langkah dalam artikel, [memulihkan pengguna di Office 365](https://docs.microsoft.com/office365/admin/add-users/restore-user?view=o365-worldwide).</span><span class="sxs-lookup"><span data-stu-id="ea0ba-110">To resolve this issue, you should restore the original UPN with the steps in the article, [Restore a user in Office 365](https://docs.microsoft.com/office365/admin/add-users/restore-user?view=o365-worldwide).</span></span>

<span data-ttu-id="ea0ba-111">Catatan: jika Pusat admin OneDrive atau SharePoint tidak tersedia untuk beberapa pengguna yang sebelumnya memiliki akses, mungkin ada masalah layanan sementara.</span><span class="sxs-lookup"><span data-stu-id="ea0ba-111">Note: If a OneDrive or SharePoint Admin center is not available to multiple users who previously had access, there may be a temporary service issue.</span></span>  <span data-ttu-id="ea0ba-112">[Periksa dasbor Kesehatan Layanan](https://portal.office.com/adminportal/home#/servicehealth).</span><span class="sxs-lookup"><span data-stu-id="ea0ba-112">[Check the service health dashboard](https://portal.office.com/adminportal/home#/servicehealth).</span></span>


