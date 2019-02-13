---
title: Sinkronisasi profil
ms.author: arnek
author: arnek
ms.date: 6/20/2018
ms.audience: ITPro
ms.topic: article
ROBOTS: NOINDEX, NOFOLLOW
localization_priority: Normal
ms.assetid: 6b695be8-eaf5-44ff-b0ae-1e0d89e7ab36
ms.openlocfilehash: d1a72a85767e36fefbfa8eee266befcaf2e48af0
ms.sourcegitcommit: dd43cc0a9470f98b8ef2a3787c823801d674c666
ms.translationtype: MT
ms.contentlocale: id-ID
ms.lasthandoff: 02/12/2019
ms.locfileid: "29920091"
---
# <a name="when-do-my-profile-changes-sync-to-the-sharepoint-user-profile-application"></a><span data-ttu-id="76cb3-102">Kapan perubahan profil Saya sync ke SharePoint pengguna profil aplikasi?</span><span class="sxs-lookup"><span data-stu-id="76cb3-102">When do my profile changes sync to the SharePoint User Profile Application?</span></span>

<span data-ttu-id="76cb3-103">SharePoint Online menggunakan Active Directory impor pekerjaan timer (AD Import) untuk mengimpor pengguna dan grup ke profil pengguna aplikasi.</span><span class="sxs-lookup"><span data-stu-id="76cb3-103">SharePoint Online uses the Active Directory Import timer job (AD Import) to import users and groups into the User Profile Application.</span></span> 
  
1. <span data-ttu-id="76cb3-p101">Iklan impor syncs perubahan dari SharePoint Online direktori toko aplikasi profil pengguna. Perubahan ini diproses dalam batch.</span><span class="sxs-lookup"><span data-stu-id="76cb3-p101">AD Import syncs changes from the SharePoint Online Directory Store to the User Profile Application. These changes are processed in batches.</span></span>
    
2. <span data-ttu-id="76cb3-106">Pekerjaan timer berjalan sampai perubahan disinkronkan.</span><span class="sxs-lookup"><span data-stu-id="76cb3-106">The timer job runs until the changes are synced.</span></span>
    
> [!NOTE]
> <span data-ttu-id="76cb3-p102">Waktu yang dibutuhkan untuk menjalankan pekerjaan tergantung pada jumlah perubahan untuk memproses. Sejumlah besar perubahan memakan waktu lama. Service Level Agreement (SLA) menyatakan bahwa perubahan ke pengguna dalam direktori Online SharePoint akan tercermin dalam profil pengguna aplikasi dalam 24 jam.</span><span class="sxs-lookup"><span data-stu-id="76cb3-p102">The time it takes the job to run depends on the number of changes to process. A large number of changes takes longer. The Service Level Agreement (SLA) states that a change to a user in the SharePoint Online Directory will be reflected in the User Profile Application in 24 hours.</span></span> 
  
[<span data-ttu-id="76cb3-110">Info lebih lanjut tentang sinkronisasi profil pengguna di SharePoint Online</span><span class="sxs-lookup"><span data-stu-id="76cb3-110">More info about user profile sync in SharePoint Online</span></span>](https://go.microsoft.com/fwlink/?linkid=875671)
  

