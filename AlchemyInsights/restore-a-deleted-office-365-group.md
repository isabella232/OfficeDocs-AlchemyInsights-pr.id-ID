---
title: Memulihkan grup Microsoft 365 yang dihapus
ms.author: pebaum
author: pebaum
manager: scotv
ms.date: 04/21/2020
ms.audience: Admin
ms.topic: article
ms.service: o365-administration
ROBOTS: NOINDEX, NOFOLLOW
localization_priority: Normal
ms.collection: Adm_O365
ms.custom:
- "98"
- "1200024"
ms.assetid: bc0396ea-c426-4d1d-bb89-ced602d06fb6
ms.openlocfilehash: 6f640093cd099f20d3a95eede5c141ad74838b0b
ms.sourcegitcommit: 7b2e5078dd65f11af6650e692a7ea48e91f544e0
ms.translationtype: MT
ms.contentlocale: id-ID
ms.lasthandoff: 04/02/2021
ms.locfileid: "51505689"
---
# <a name="restore-a-deleted-microsoft-365-group"></a><span data-ttu-id="6017c-102">Memulihkan grup Microsoft 365 yang dihapus</span><span class="sxs-lookup"><span data-stu-id="6017c-102">Restore a deleted Microsoft 365 group</span></span>

<span data-ttu-id="6017c-103">Anda dapat memulihkan grup Microsoft 365 yang dihapus atau Microsoft Teams dalam 30 hari dari penghapusan.</span><span class="sxs-lookup"><span data-stu-id="6017c-103">You can restore a deleted Microsoft 365 group or Microsoft Teams within 30 days from the deletion.</span></span>

1. <span data-ttu-id="6017c-104">Untuk masuk ke pusat admin Microsoft 365 serta mencantumkan grup dan tim yang dihapus, masuk ke pusat [admin Microsoft 365.](https://aka.ms/RestoreDeletedGroup)</span><span class="sxs-lookup"><span data-stu-id="6017c-104">To login to Microsoft 365 admin center and list the deleted groups and teams, go to the [Microsoft 365 admin center](https://aka.ms/RestoreDeletedGroup).</span></span>

    <span data-ttu-id="6017c-105">**Catatan:** Masuk menggunakan akun yang ditetapkan untuk administrator penyewa atau peran admin grup.</span><span class="sxs-lookup"><span data-stu-id="6017c-105">**Note:** Log in using the account that is assigned to either the tenant administrator or the groups admin role.</span></span>

1. <span data-ttu-id="6017c-106">Pilih grup/Teams Microsoft 365 yang dihapus untuk dipulihkan, lalu klik **pulihkan grup.**</span><span class="sxs-lookup"><span data-stu-id="6017c-106">Select the deleted Microsoft 365 group/Teams to be restored and click **restore group**.</span></span>

    <span data-ttu-id="6017c-107">Jika grup tidak bisa dipulihkan karena alamat SMTP yang berkonflik, gunakan perintah berikut untuk menemukan objek yang menyebabkan konflik dan menghapus alamat SMTP:</span><span class="sxs-lookup"><span data-stu-id="6017c-107">If the group can't be restored because of a conflicting SMTP address, use following command to find the object that’s causing conflict and remove the SMTP address:</span></span>

    `Get-Recipient -Filter "EmailAddresses -eq '<conflictingsmtpaddress>'"`

    <span data-ttu-id="6017c-108">**Catatan:** Dalam beberapa kasus, mungkin akan memakan waktu hingga 24 jam agar grup dan semua datanya dipulihkan.</span><span class="sxs-lookup"><span data-stu-id="6017c-108">**Note:** In some cases, it might take as long as 24 hours for the group and all of its data to be restored.</span></span>

    <span data-ttu-id="6017c-109">Untuk informasi selengkapnya, atau untuk mempelajari cara memulihkan grup menggunakan PowerShell, [lihat Memulihkan grup Microsoft 365 yang dihapus.](https://go.microsoft.com/fwlink/?linkid=867802)</span><span class="sxs-lookup"><span data-stu-id="6017c-109">For more info, or to learn how to restore groups using PowerShell, see [Restore a deleted Microsoft 365 group](https://go.microsoft.com/fwlink/?linkid=867802).</span></span>