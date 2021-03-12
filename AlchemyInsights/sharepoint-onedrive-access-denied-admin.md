---
title: Memecahkan masalah pesan Akses ditolak
ms.author: pebaum
author: pebaum
ms.date: 04/21/2020
ms.audience: ITPro
ms.topic: article
ms.service: o365-administration
ROBOTS: NOINDEX, NOFOLLOW
localization_priority: Normal
ms.assetid: d678b57a-53ad-4414-9423-d8726a0c532f
ms.openlocfilehash: 3189fa61d28253569278024d4191ee63b917509f
ms.sourcegitcommit: 0eb4f9bde53395b5fd4b5cd4ffc56ca96db91298
ms.translationtype: MT
ms.contentlocale: id-ID
ms.lasthandoff: 03/10/2021
ms.locfileid: "50707957"
---
# <a name="troubleshoot-access-denied-messages-in-sharepointonedrive-admin-center"></a><span data-ttu-id="29c94-102">Memecahkan masalah akses pesan yang ditolak di pusat admin SharePoint/OneDrive</span><span class="sxs-lookup"><span data-stu-id="29c94-102">Troubleshoot Access Denied messages in Sharepoint/OneDrive Admin Center</span></span>

<span data-ttu-id="29c94-103">Jika Anda menerima pesan Akses ditolak saat mencoba menelusuri ke Pusat admin SharePoint/OneDrive, pastikan bahwa Anda [menetapkan lisensi untuk pengguna tersebut](https://docs.microsoft.com/microsoft-365/admin/add-users/add-users).</span><span class="sxs-lookup"><span data-stu-id="29c94-103">If you are receiving an access denied message when attempting to browse to a Sharepoint/OneDrive Admin Center, please make sure that you [assign a license to the user](https://docs.microsoft.com/microsoft-365/admin/add-users/add-users).</span></span> <span data-ttu-id="29c94-104">Jika pengguna memiliki lisensi, Anda juga harus memastikan bahwa mereka [diberi peran administrator](https://docs.microsoft.com/microsoft-365/admin/add-users/about-admin-roles) yang bisa mengakses pusat admin.</span><span class="sxs-lookup"><span data-stu-id="29c94-104">If the user has a license, you should also make sure they are [assigned an administrator role](https://docs.microsoft.com/microsoft-365/admin/add-users/about-admin-roles) that can access the admin centers.</span></span>

<span data-ttu-id="29c94-105">Masalah ini juga bisa terjadi ketika pengguna dihapus dan dibuat ulang dengan nama prinsip pengguna (UPN) yang sama.</span><span class="sxs-lookup"><span data-stu-id="29c94-105">This issue can also occur when a user is deleted and re-created with the same user principal name (UPN).</span></span> <span data-ttu-id="29c94-106">Akun baru dibuat menggunakan nilai PUID (ID unik paspor) yang berbeda.</span><span class="sxs-lookup"><span data-stu-id="29c94-106">The new account is created by using a different PUID (Passport Unique ID) value.</span></span> <span data-ttu-id="29c94-107">Saat pengguna mencoba mengakses kumpulan situs atau OneDrive mereka, pengguna tersebut memiliki PUID yang salah.</span><span class="sxs-lookup"><span data-stu-id="29c94-107">When the user tries to access a site collection or their OneDrive, the user has an incorrect PUID.</span></span> <span data-ttu-id="29c94-108">Skenario kedua melibatkan sinkronisasi direktori dengan unit organisasi direktori aktif (OU).</span><span class="sxs-lookup"><span data-stu-id="29c94-108">A second scenario involves directory synchronization with an Active Directory organizational unit (OU).</span></span> <span data-ttu-id="29c94-109">Jika pengguna sudah masuk ke SharePoint, lalu dipindahkan ke OU berbeda dan resynced dengan SharePoint, mereka mungkin mengalami masalah ini.</span><span class="sxs-lookup"><span data-stu-id="29c94-109">If users have already signed in to SharePoint, and then are moved to a different OU and resynced with SharePoint, they may experience this problem.</span></span>

<span data-ttu-id="29c94-110">Untuk mengatasi masalah ini, Anda harus memulihkan UPN asli dengan langkah-langkah dalam artikel, [memulihkan pengguna di Microsoft 365](https://docs.microsoft.com/microsoft-365/admin/add-users/restore-user).</span><span class="sxs-lookup"><span data-stu-id="29c94-110">To resolve this issue, you should restore the original UPN with the steps in the article, [Restore a user in Microsoft 365](https://docs.microsoft.com/microsoft-365/admin/add-users/restore-user).</span></span>

<span data-ttu-id="29c94-111">Catatan: jika OneDrive atau pusat admin SharePoint tidak tersedia untuk beberapa pengguna yang sebelumnya memiliki Access, mungkin ada masalah layanan sementara.</span><span class="sxs-lookup"><span data-stu-id="29c94-111">Note: If a OneDrive or SharePoint Admin center is not available to multiple users who previously had access, there may be a temporary service issue.</span></span>  <span data-ttu-id="29c94-112">[Periksa dasbor Kesehatan Layanan](https://portal.office.com/adminportal/home#/servicehealth).</span><span class="sxs-lookup"><span data-stu-id="29c94-112">[Check the service health dashboard](https://portal.office.com/adminportal/home#/servicehealth).</span></span>


