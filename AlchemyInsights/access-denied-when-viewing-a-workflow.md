---
title: Akses ditolak saat menampilkan alur kerja
ms.author: pebaum
author: pebaum
ms.date: 04/21/2020
ms.audience: ITPro
ms.topic: article
ms.service: o365-administration
ROBOTS: NOINDEX, NOFOLLOW
localization_priority: Normal
ms.assetid: 47ceb983-f9a4-4c55-a40c-03d5c3d75dc9
ms.openlocfilehash: 710775e8b2dee98969df7a4c8410a3e61181aaf6
ms.sourcegitcommit: c6692ce0fa1358ec3529e59ca0ecdfdea4cdc759
ms.translationtype: MT
ms.contentlocale: id-ID
ms.lasthandoff: 09/14/2020
ms.locfileid: "47688805"
---
# <a name="access-denied-when-viewing-a-workflow"></a><span data-ttu-id="c76bf-102">Akses ditolak saat menampilkan alur kerja</span><span class="sxs-lookup"><span data-stu-id="c76bf-102">Access denied when viewing a Workflow</span></span>

<span data-ttu-id="c76bf-103">Alur kerja SharePoint 2013 yang mencoba mengirim email ke grup SharePoint bisa gagal dengan pesan kesalahan "Akses ditolak" Jika keanggotaan grup SharePoint tidak diatur ke semua orang.</span><span class="sxs-lookup"><span data-stu-id="c76bf-103">SharePoint 2013 Workflows that attempt to send an email to a SharePoint group can fail with an "Access Denied" error message if the membership of the SharePoint group is not set to Everyone.</span></span>
  
 <span data-ttu-id="c76bf-104">**Untuk mengatasi masalah ini, lakukan langkah-langkah ini:**</span><span class="sxs-lookup"><span data-stu-id="c76bf-104">**To resolve this issue, do these steps:**</span></span>
  
 1. <span data-ttu-id="c76bf-105">Izinkan semua orang melihat anggota grup SharePoint.</span><span class="sxs-lookup"><span data-stu-id="c76bf-105">Allow everybody to see the members of the SharePoint group.</span></span>
  
 2. <span data-ttu-id="c76bf-106">Hapus grup SharePoint dari baris kepada atau CC dari email.</span><span class="sxs-lookup"><span data-stu-id="c76bf-106">Remove the SharePoint group from the To or CC line of the email.</span></span>
  
 3. <span data-ttu-id="c76bf-107">Menambahkan pengguna secara eksplisit ke baris kepada atau CC jika visibilitas keanggotaan tidak bisa diubah untuk grup SharePoint.</span><span class="sxs-lookup"><span data-stu-id="c76bf-107">Explicitly add the users to the To or CC line if the membership visibility cannot be changed for SharePoint group.</span></span>
  
<span data-ttu-id="c76bf-108">Untuk melihat detail selengkapnya, lihat [http tidak sah ke/_vti_bin/client.SVC/SP.Utilities.Utility.sendemail](https://go.microsoft.com/fwlink/?linkid=2044694&amp;clcid=0x409).</span><span class="sxs-lookup"><span data-stu-id="c76bf-108">To view more details please refer to [HTTP Unauthorized to /_vti_bin/client.svc/sp.utilities.utility.SendEmail](https://go.microsoft.com/fwlink/?linkid=2044694&amp;clcid=0x409).</span></span>
  