---
title: Memberikan akses kepada pengguna ke SharePoint dan OneDrive
ms.author: kirks
author: Techwriter40
manager: pamgreen
ms.date: 11/14/2018
ms.audience: Admin
ms.topic: article
ROBOTS: NOINDEX, NOFOLLOW
localization_priority: Normal
ms.collection: Adm_O365
ms.custom: ''
ms.assetid: cebb7a4a-33e1-474e-a5d0-dbd02a80b1e9
ms.openlocfilehash: 9326932e93970edc96396a141c9b36b14e7b4d4d
ms.sourcegitcommit: 241e21b6da226563bf70bdb1f5bad3d91c38cd2c
ms.translationtype: MT
ms.contentlocale: id-ID
ms.lasthandoff: 06/05/2019
ms.locfileid: "34736651"
---
# <a name="give-users-access-to-sharepoint-and-onedrive"></a><span data-ttu-id="b5a8d-102">Memberikan akses kepada pengguna ke SharePoint dan OneDrive</span><span class="sxs-lookup"><span data-stu-id="b5a8d-102">Give users access to SharePoint and OneDrive</span></span>

<span data-ttu-id="b5a8d-103">Masalah ini paling sering terjadi ketika pengguna dihapus dan kembali dibuat dengan sama pengguna (UPN nama dasar).</span><span class="sxs-lookup"><span data-stu-id="b5a8d-103">This issue most frequently occurs when a user is deleted and re-created with the same user principal name (UPN).</span></span> <span data-ttu-id="b5a8d-104">Account yang baru dibuat dengan menggunakan PUID (paspor unik ID) nilai yang berbeda.</span><span class="sxs-lookup"><span data-stu-id="b5a8d-104">The new account is created by using a different PUID (Passport Unique ID) value.</span></span> <span data-ttu-id="b5a8d-105">Ketika pengguna mencoba untuk mengakses situs koleksi atau OneDrive mereka, pengguna memiliki PUID salah.</span><span class="sxs-lookup"><span data-stu-id="b5a8d-105">When the user tries to access a site collection or their OneDrive, the user has an incorrect PUID.</span></span> <span data-ttu-id="b5a8d-106">Skenario yang kedua melibatkan sinkronisasi direktori dengan unit organisasi Active Directory (OU).</span><span class="sxs-lookup"><span data-stu-id="b5a8d-106">A second scenario involves directory synchronization with an Active Directory organizational unit (OU).</span></span> <span data-ttu-id="b5a8d-107">Jika pengguna telah sudah masuk ke SharePoint, dan kemudian pindah ke OU berbeda dan resynced dengan SharePoint, mereka mungkin mengalami masalah ini.</span><span class="sxs-lookup"><span data-stu-id="b5a8d-107">If users have already signed in to SharePoint, and then are moved to a different OU and resynced with SharePoint, they may experience this problem.</span></span>

<span data-ttu-id="b5a8d-108">Untuk mengatasi masalah ini, Anda harus mengembalikan UPN asli dengan langkah-langkah dalam artikel,[mengembalikan pengguna di Office 365](https://docs.microsoft.com/en-us/office365/admin/add-users/restore-user?view=o365-worldwide).</span><span class="sxs-lookup"><span data-stu-id="b5a8d-108">To resolve this issue you should restore the original UPN with the steps in the article,[Restore a user in Office 365](https://docs.microsoft.com/en-us/office365/admin/add-users/restore-user?view=o365-worldwide).</span></span>

<span data-ttu-id="b5a8d-109">Setelah ini selesai, Anda dapat memverifikasi pengguna memiliki hak admin situs OneDrive dengan mengikuti langkah-langkah untuk [menambahkan admin's untuk pengguna OneDrive](https://docs.microsoft.com/en-us/sharepoint/manage-user-profiles?redirectSourcePath=%252fen-us%252farticle%252fmanage-user-profiles-in-the-sharepoint-admin-center-494bec9c-6654-41f0-920f-f7f937ea9723#add-and-remove-admins-for-a-users-onedrive)</span><span class="sxs-lookup"><span data-stu-id="b5a8d-109">After this is done, you can verify the user has admin rights to the OneDrive site by following the steps to [Add admin's for a user's OneDrive](https://docs.microsoft.com/en-us/sharepoint/manage-user-profiles?redirectSourcePath=%252fen-us%252farticle%252fmanage-user-profiles-in-the-sharepoint-admin-center-494bec9c-6654-41f0-920f-f7f937ea9723#add-and-remove-admins-for-a-users-onedrive)</span></span>

<span data-ttu-id="b5a8d-110">Untuk informasi lebih lanjut tentang tingkat izin, lihat artikel, [pemahaman tingkat izin di SharePoint](https://docs.microsoft.com/en-us/sharepoint/understanding-permission-levels).</span><span class="sxs-lookup"><span data-stu-id="b5a8d-110">For more information on permission levels, see the article, [Understanding permission levels in SharePoint](https://docs.microsoft.com/en-us/sharepoint/understanding-permission-levels).</span></span>
