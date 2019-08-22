---
title: Akses ditolak saat melihat alur kerja
ms.author: kirks
author: Techwriter40
ms.date: 11/27/2018
ms.audience: ITPro
ms.topic: article
ROBOTS: NOINDEX, NOFOLLOW
localization_priority: Normal
ms.assetid: 47ceb983-f9a4-4c55-a40c-03d5c3d75dc9
ms.openlocfilehash: 53bd9285e49e220f880eea21923f261302003127
ms.sourcegitcommit: 1d98db8acb9959aba3b5e308a567ade6b62da56c
ms.translationtype: MT
ms.contentlocale: id-ID
ms.lasthandoff: 08/22/2019
ms.locfileid: "36495826"
---
# <a name="access-denied-when-viewing-a-workflow"></a><span data-ttu-id="ecd16-102">Akses ditolak saat melihat alur kerja</span><span class="sxs-lookup"><span data-stu-id="ecd16-102">Access denied when viewing a Workflow</span></span>

<span data-ttu-id="ecd16-103">Workflow 2013 SharePoint yang mencoba untuk mengirim email ke grup SharePoint dapat gagal dengan pesan galat "Akses ditolak" Jika keanggotaan grup SharePoint tidak diset untuk semua orang.</span><span class="sxs-lookup"><span data-stu-id="ecd16-103">SharePoint 2013 Workflows that attempt to send an email to a SharePoint group can fail with an "Access Denied" error message if the membership of the SharePoint group is not set to Everyone.</span></span>
  
 <span data-ttu-id="ecd16-104">**Untuk mengatasi masalah ini, lakukan langkah-langkah berikut:**</span><span class="sxs-lookup"><span data-stu-id="ecd16-104">**To resolve this issue, do these steps:**</span></span>
  
 1. <span data-ttu-id="ecd16-105">Memungkinkan semua orang untuk melihat anggota grup SharePoint.</span><span class="sxs-lookup"><span data-stu-id="ecd16-105">Allow everybody to see the members of the SharePoint group.</span></span>
  
 2. <span data-ttu-id="ecd16-106">Menghapus Grup SharePoint dari kepada atau CC baris email.</span><span class="sxs-lookup"><span data-stu-id="ecd16-106">Remove the SharePoint group from the To or CC line of the email.</span></span>
  
 3. <span data-ttu-id="ecd16-107">Secara eksplisit menambahkan pengguna ke kepada atau CC baris jika visibilitas keanggotaan tidak dapat diubah untuk grup SharePoint.</span><span class="sxs-lookup"><span data-stu-id="ecd16-107">Explicitly add the users to the To or CC line if the membership visibility cannot be changed for SharePoint group.</span></span>
  
<span data-ttu-id="ecd16-108">Untuk melihat rincian lebih lanjut silakan lihat [HTTP tidak sah untuk /_vti_bin/client.svc/sp.utilities.utility.SendEmail](https://go.microsoft.com/fwlink/?linkid=2044694&amp;clcid=0x409).</span><span class="sxs-lookup"><span data-stu-id="ecd16-108">To view more details please refer to [HTTP Unauthorized to /_vti_bin/client.svc/sp.utilities.utility.SendEmail](https://go.microsoft.com/fwlink/?linkid=2044694&amp;clcid=0x409).</span></span>
  