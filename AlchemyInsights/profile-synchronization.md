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
ms.openlocfilehash: b9b90dad6c5fa41afcd4e4c9a929594735eca066
ms.sourcegitcommit: 1d98db8acb9959aba3b5e308a567ade6b62da56c
ms.translationtype: MT
ms.contentlocale: id-ID
ms.lasthandoff: 08/22/2019
ms.locfileid: "36554336"
---
# <a name="when-do-my-profile-changes-sync-to-the-sharepoint-user-profile-application"></a><span data-ttu-id="110b5-102">Kapan perubahan profil Saya sync ke SharePoint pengguna profil aplikasi?</span><span class="sxs-lookup"><span data-stu-id="110b5-102">When do my profile changes sync to the SharePoint User Profile Application?</span></span>

<span data-ttu-id="110b5-103">SharePoint Online menggunakan Active Directory impor pekerjaan timer (AD Import) untuk mengimpor pengguna dan grup ke profil pengguna aplikasi.</span><span class="sxs-lookup"><span data-stu-id="110b5-103">SharePoint Online uses the Active Directory Import timer job (AD Import) to import users and groups into the User Profile Application.</span></span> 
  
1. <span data-ttu-id="110b5-104">Iklan impor syncs perubahan dari SharePoint Online direktori toko aplikasi profil pengguna.</span><span class="sxs-lookup"><span data-stu-id="110b5-104">AD Import syncs changes from the SharePoint Online Directory Store to the User Profile Application.</span></span> <span data-ttu-id="110b5-105">Perubahan ini diproses dalam batch.</span><span class="sxs-lookup"><span data-stu-id="110b5-105">These changes are processed in batches.</span></span>
    
2. <span data-ttu-id="110b5-106">Pekerjaan timer berjalan sampai perubahan disinkronkan.</span><span class="sxs-lookup"><span data-stu-id="110b5-106">The timer job runs until the changes are synced.</span></span>
    
> [!NOTE]
> <span data-ttu-id="110b5-107">Waktu yang dibutuhkan untuk menjalankan pekerjaan tergantung pada jumlah perubahan untuk memproses.</span><span class="sxs-lookup"><span data-stu-id="110b5-107">The time it takes the job to run depends on the number of changes to process.</span></span> <span data-ttu-id="110b5-108">Sejumlah besar perubahan memakan waktu lama.</span><span class="sxs-lookup"><span data-stu-id="110b5-108">A large number of changes takes longer.</span></span> <span data-ttu-id="110b5-109">Service Level Agreement (SLA) menyatakan bahwa perubahan ke pengguna dalam direktori Online SharePoint akan tercermin dalam profil pengguna aplikasi dalam 24 jam.</span><span class="sxs-lookup"><span data-stu-id="110b5-109">The Service Level Agreement (SLA) states that a change to a user in the SharePoint Online Directory will be reflected in the User Profile Application in 24 hours.</span></span> 
  
[<span data-ttu-id="110b5-110">Info lebih lanjut tentang sinkronisasi profil pengguna di SharePoint Online</span><span class="sxs-lookup"><span data-stu-id="110b5-110">More info about user profile sync in SharePoint Online</span></span>](https://go.microsoft.com/fwlink/?linkid=875671)
  

