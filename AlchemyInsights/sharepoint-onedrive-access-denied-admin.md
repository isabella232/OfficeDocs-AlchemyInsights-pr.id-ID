---
title: Memecahkan masalah Akses ditolak pesan
ms.author: pebaum
author: pebaum
ms.date: 04/21/2020
ms.audience: ITPro
ms.topic: article
ROBOTS: NOINDEX, NOFOLLOW
localization_priority: Normal
ms.assetid: d678b57a-53ad-4414-9423-d8726a0c532f
ms.openlocfilehash: 9430b9786b35dda9fb2604fb6ae3c39c8c258d6e
ms.sourcegitcommit: bc7d6f4f3c9f7060d073f5130e1ec856e248d020
ms.translationtype: MT
ms.contentlocale: id-ID
ms.lasthandoff: 06/02/2020
ms.locfileid: "44505382"
---
# <a name="troubleshoot-access-denied-messages-in-sharepointonedrive-admin-center"></a><span data-ttu-id="3b89d-102">Memecahkan masalah Akses ditolak pesan di pusat admin SharePoint/OneDrive</span><span class="sxs-lookup"><span data-stu-id="3b89d-102">Troubleshoot Access Denied messages in Sharepoint/OneDrive Admin Center</span></span>

<span data-ttu-id="3b89d-103">Jika Anda menerima pesan Akses ditolak saat berusaha menjelajah ke Pusat admin SharePoint/OneDrive, pastikan bahwa Anda [menetapkan lisensi untuk pengguna](https://docs.microsoft.com/microsoft-365/admin/add-users/add-users).</span><span class="sxs-lookup"><span data-stu-id="3b89d-103">If you are receiving an access denied message when attempting to browse to a Sharepoint/OneDrive Admin Center, please make sure that you [assign a license to the user](https://docs.microsoft.com/microsoft-365/admin/add-users/add-users).</span></span> <span data-ttu-id="3b89d-104">Jika pengguna memiliki lisensi, Anda juga harus memastikan bahwa mereka [ditetapkan peran administrator](hhttps://docs.microsoft.com/microsoft-365/admin/add-users/about-admin-roles) yang dapat mengakses pusat admin.</span><span class="sxs-lookup"><span data-stu-id="3b89d-104">If the user has a license, you should also make sure they are [assigned an administrator role](hhttps://docs.microsoft.com/microsoft-365/admin/add-users/about-admin-roles) that can access the admin centers.</span></span>

<span data-ttu-id="3b89d-105">Masalah ini juga dapat terjadi ketika pengguna dihapus dan dibuat ulang dengan nama prinsip pengguna (UPN) yang sama.</span><span class="sxs-lookup"><span data-stu-id="3b89d-105">This issue can also occur when a user is deleted and re-created with the same user principal name (UPN).</span></span> <span data-ttu-id="3b89d-106">Akun baru dibuat dengan menggunakan nilai yang berbeda PUID (paspor unik ID).</span><span class="sxs-lookup"><span data-stu-id="3b89d-106">The new account is created by using a different PUID (Passport Unique ID) value.</span></span> <span data-ttu-id="3b89d-107">Saat pengguna berusaha mengakses koleksi situs atau OneDrive mereka, pengguna memiliki PUID salah.</span><span class="sxs-lookup"><span data-stu-id="3b89d-107">When the user tries to access a site collection or their OneDrive, the user has an incorrect PUID.</span></span> <span data-ttu-id="3b89d-108">Skenario kedua melibatkan sinkronisasi direktori dengan direktori aktif unit organisasi (OU).</span><span class="sxs-lookup"><span data-stu-id="3b89d-108">A second scenario involves directory synchronization with an Active Directory organizational unit (OU).</span></span> <span data-ttu-id="3b89d-109">Jika pengguna telah masuk ke SharePoint, dan kemudian dipindahkan ke OU berbeda dan resynced dengan SharePoint, mereka mungkin mengalami masalah ini.</span><span class="sxs-lookup"><span data-stu-id="3b89d-109">If users have already signed in to SharePoint, and then are moved to a different OU and resynced with SharePoint, they may experience this problem.</span></span>

<span data-ttu-id="3b89d-110">Untuk mengatasi masalah ini, Anda harus memulihkan UPN asli dengan langkah dalam artikel, [memulihkan pengguna di Microsoft 365](https://docs.microsoft.com/microsoft-365/admin/add-users/restore-user).</span><span class="sxs-lookup"><span data-stu-id="3b89d-110">To resolve this issue, you should restore the original UPN with the steps in the article, [Restore a user in Microsoft 365](https://docs.microsoft.com/microsoft-365/admin/add-users/restore-user).</span></span>

<span data-ttu-id="3b89d-111">Catatan: jika Pusat admin OneDrive atau SharePoint tidak tersedia untuk beberapa pengguna yang sebelumnya memiliki akses, mungkin ada masalah layanan sementara.</span><span class="sxs-lookup"><span data-stu-id="3b89d-111">Note: If a OneDrive or SharePoint Admin center is not available to multiple users who previously had access, there may be a temporary service issue.</span></span>  <span data-ttu-id="3b89d-112">[Periksa dasbor Kesehatan Layanan](https://portal.office.com/adminportal/home#/servicehealth).</span><span class="sxs-lookup"><span data-stu-id="3b89d-112">[Check the service health dashboard](https://portal.office.com/adminportal/home#/servicehealth).</span></span>


