---
title: Sinkronisasi profil
ms.author: arnek
author: arnek
ms.date: 04/21/2020
ms.audience: ITPro
ms.topic: article
ROBOTS: NOINDEX, NOFOLLOW
localization_priority: Normal
ms.assetid: 6b695be8-eaf5-44ff-b0ae-1e0d89e7ab36
ms.openlocfilehash: dc6e0280961d14aa3e6bd466afbe0cbe89418d17
ms.sourcegitcommit: 631cbb5f03e5371f0995e976536d24e9d13746c3
ms.translationtype: MT
ms.contentlocale: id-ID
ms.lasthandoff: 04/22/2020
ms.locfileid: "43768116"
---
# <a name="when-do-my-profile-changes-sync-to-the-sharepoint-user-profile-application"></a><span data-ttu-id="a184e-102">Kapan perubahan profil saya disinkronkan ke aplikasi profil pengguna SharePoint?</span><span class="sxs-lookup"><span data-stu-id="a184e-102">When do my profile changes sync to the SharePoint User Profile Application?</span></span>

<span data-ttu-id="a184e-103">SharePoint Online menggunakan pekerjaan timer impor direktori aktif (AD impor) untuk mengimpor pengguna dan grup ke profil pengguna aplikasi.</span><span class="sxs-lookup"><span data-stu-id="a184e-103">SharePoint Online uses the Active Directory Import timer job (AD Import) to import users and groups into the User Profile Application.</span></span> 
  
1. <span data-ttu-id="a184e-104">Impor AD Sync perubahan dari SharePoint online direktori penyimpanan ke profil pengguna aplikasi.</span><span class="sxs-lookup"><span data-stu-id="a184e-104">AD Import syncs changes from the SharePoint Online Directory Store to the User Profile Application.</span></span> <span data-ttu-id="a184e-105">Perubahan ini diproses dalam batch.</span><span class="sxs-lookup"><span data-stu-id="a184e-105">These changes are processed in batches.</span></span>
    
2. <span data-ttu-id="a184e-106">Pekerjaan timer berjalan hingga perubahan disinkronkan.</span><span class="sxs-lookup"><span data-stu-id="a184e-106">The timer job runs until the changes are synced.</span></span>
    
> [!NOTE]
> <span data-ttu-id="a184e-107">Waktu yang dibutuhkan untuk menjalankan pekerjaan tergantung pada jumlah perubahan proses.</span><span class="sxs-lookup"><span data-stu-id="a184e-107">The time it takes the job to run depends on the number of changes to process.</span></span> <span data-ttu-id="a184e-108">Sejumlah besar perubahan membutuhkan waktu lebih lama.</span><span class="sxs-lookup"><span data-stu-id="a184e-108">A large number of changes takes longer.</span></span> <span data-ttu-id="a184e-109">Layanan tingkat perjanjian (SLA) menyatakan bahwa perubahan ke pengguna di direktori SharePoint online akan tercermin dalam aplikasi profil pengguna dalam 24 jam.</span><span class="sxs-lookup"><span data-stu-id="a184e-109">The Service Level Agreement (SLA) states that a change to a user in the SharePoint Online Directory will be reflected in the User Profile Application in 24 hours.</span></span> 
  
[<span data-ttu-id="a184e-110">Info lebih lanjut tentang sinkronisasi profil pengguna di SharePoint online</span><span class="sxs-lookup"><span data-stu-id="a184e-110">More info about user profile sync in SharePoint Online</span></span>](https://go.microsoft.com/fwlink/?linkid=875671)
  

