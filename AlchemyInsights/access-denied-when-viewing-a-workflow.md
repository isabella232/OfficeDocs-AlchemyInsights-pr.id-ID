---
title: Akses ditolak saat melihat alur kerja
ms.author: pebaum
author: pebaum
ms.date: 04/21/2020
ms.audience: ITPro
ms.topic: article
ROBOTS: NOINDEX, NOFOLLOW
localization_priority: Normal
ms.assetid: 47ceb983-f9a4-4c55-a40c-03d5c3d75dc9
ms.openlocfilehash: c576bf88225582f2577e0b59506a7482cf9f38d5
ms.sourcegitcommit: 55eff703a17e500681d8fa6a87eb067019ade3cc
ms.translationtype: MT
ms.contentlocale: id-ID
ms.lasthandoff: 04/22/2020
ms.locfileid: "43687333"
---
# <a name="access-denied-when-viewing-a-workflow"></a><span data-ttu-id="122a7-102">Akses ditolak saat melihat alur kerja</span><span class="sxs-lookup"><span data-stu-id="122a7-102">Access denied when viewing a Workflow</span></span>

<span data-ttu-id="122a7-103">SharePoint 2013 alur kerja yang mencoba mengirim email ke grup SharePoint dapat gagal dengan pesan galat "Akses ditolak" Jika keanggotaan grup SharePoint tidak ditetapkan ke semua orang.</span><span class="sxs-lookup"><span data-stu-id="122a7-103">SharePoint 2013 Workflows that attempt to send an email to a SharePoint group can fail with an "Access Denied" error message if the membership of the SharePoint group is not set to Everyone.</span></span>
  
 <span data-ttu-id="122a7-104">**Untuk mengatasi masalah ini, lakukan langkah berikut:**</span><span class="sxs-lookup"><span data-stu-id="122a7-104">**To resolve this issue, do these steps:**</span></span>
  
 1. <span data-ttu-id="122a7-105">Izinkan semua orang untuk melihat anggota kelompok SharePoint.</span><span class="sxs-lookup"><span data-stu-id="122a7-105">Allow everybody to see the members of the SharePoint group.</span></span>
  
 2. <span data-ttu-id="122a7-106">Hapus grup SharePoint dari baris kepada atau CC email.</span><span class="sxs-lookup"><span data-stu-id="122a7-106">Remove the SharePoint group from the To or CC line of the email.</span></span>
  
 3. <span data-ttu-id="122a7-107">Secara eksplisit menambahkan pengguna ke baris kepada atau CC jika visibilitas keanggotaan tidak dapat diubah untuk grup SharePoint.</span><span class="sxs-lookup"><span data-stu-id="122a7-107">Explicitly add the users to the To or CC line if the membership visibility cannot be changed for SharePoint group.</span></span>
  
<span data-ttu-id="122a7-108">Untuk melihat rincian lebih lanjut silakan merujuk ke [http tidak sah untuk/_vti_bin/client.SVC/SP.Utilities.Utility.sendemail](https://go.microsoft.com/fwlink/?linkid=2044694&amp;clcid=0x409).</span><span class="sxs-lookup"><span data-stu-id="122a7-108">To view more details please refer to [HTTP Unauthorized to /_vti_bin/client.svc/sp.utilities.utility.SendEmail](https://go.microsoft.com/fwlink/?linkid=2044694&amp;clcid=0x409).</span></span>
  