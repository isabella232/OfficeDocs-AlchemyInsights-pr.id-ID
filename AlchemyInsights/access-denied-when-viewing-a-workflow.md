---
title: Akses ditolak saat melihat alur kerja
ms.author: pebaum
author: Techwriter40
ms.date: 11/27/2018
ms.audience: ITPro
ms.topic: article
ROBOTS: NOINDEX, NOFOLLOW
localization_priority: Normal
ms.assetid: 47ceb983-f9a4-4c55-a40c-03d5c3d75dc9
ms.openlocfilehash: 4ca65583fbd98867026e9e3cc8f36fe38798aa85
ms.sourcegitcommit: b43f77221f47b50c41197a448a9c26c423ce1ad5
ms.translationtype: MT
ms.contentlocale: id-ID
ms.lasthandoff: 11/15/2019
ms.locfileid: "36747751"
---
# <a name="access-denied-when-viewing-a-workflow"></a><span data-ttu-id="94df4-102">Akses ditolak saat melihat alur kerja</span><span class="sxs-lookup"><span data-stu-id="94df4-102">Access denied when viewing a Workflow</span></span>

<span data-ttu-id="94df4-103">SharePoint 2013 alur kerja yang mencoba mengirim email ke grup SharePoint dapat gagal dengan pesan galat "Akses ditolak" Jika keanggotaan grup SharePoint tidak ditetapkan ke semua orang.</span><span class="sxs-lookup"><span data-stu-id="94df4-103">SharePoint 2013 Workflows that attempt to send an email to a SharePoint group can fail with an "Access Denied" error message if the membership of the SharePoint group is not set to Everyone.</span></span>
  
 <span data-ttu-id="94df4-104">**Untuk mengatasi masalah ini, lakukan langkah berikut:**</span><span class="sxs-lookup"><span data-stu-id="94df4-104">**To resolve this issue, do these steps:**</span></span>
  
 1. <span data-ttu-id="94df4-105">Izinkan semua orang untuk melihat anggota kelompok SharePoint.</span><span class="sxs-lookup"><span data-stu-id="94df4-105">Allow everybody to see the members of the SharePoint group.</span></span>
  
 2. <span data-ttu-id="94df4-106">Hapus grup SharePoint dari baris kepada atau CC email.</span><span class="sxs-lookup"><span data-stu-id="94df4-106">Remove the SharePoint group from the To or CC line of the email.</span></span>
  
 3. <span data-ttu-id="94df4-107">Secara eksplisit menambahkan pengguna ke baris kepada atau CC jika visibilitas keanggotaan tidak dapat diubah untuk grup SharePoint.</span><span class="sxs-lookup"><span data-stu-id="94df4-107">Explicitly add the users to the To or CC line if the membership visibility cannot be changed for SharePoint group.</span></span>
  
<span data-ttu-id="94df4-108">Untuk melihat rincian lebih lanjut silakan merujuk ke [http tidak sah untuk/_vti_bin/client.SVC/SP.Utilities.Utility.sendemail](https://go.microsoft.com/fwlink/?linkid=2044694&amp;clcid=0x409).</span><span class="sxs-lookup"><span data-stu-id="94df4-108">To view more details please refer to [HTTP Unauthorized to /_vti_bin/client.svc/sp.utilities.utility.SendEmail](https://go.microsoft.com/fwlink/?linkid=2044694&amp;clcid=0x409).</span></span>
  