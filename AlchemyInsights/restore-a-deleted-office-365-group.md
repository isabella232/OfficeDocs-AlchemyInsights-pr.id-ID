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
ms.openlocfilehash: b72b7c93ce9fe1b90d1608811b0eeabc8aec1363
ms.sourcegitcommit: a5edaaefdc56f8d5c8220a335f4e8228e2de4ee0
ms.translationtype: MT
ms.contentlocale: id-ID
ms.lasthandoff: 04/08/2021
ms.locfileid: "51645134"
---
# <a name="restore-a-deleted-microsoft-365-group"></a><span data-ttu-id="450ee-102">Memulihkan grup Microsoft 365 yang dihapus</span><span class="sxs-lookup"><span data-stu-id="450ee-102">Restore a deleted Microsoft 365 group</span></span>

<span data-ttu-id="450ee-103">Anda dapat memulihkan grup Microsoft 365 yang dihapus atau Microsoft Teams dalam 30 hari dari penghapusan.</span><span class="sxs-lookup"><span data-stu-id="450ee-103">You can restore a deleted Microsoft 365 group or Microsoft Teams within 30 days from the deletion.</span></span>

1. <span data-ttu-id="450ee-104">Masuk ke [pusat admin Microsoft 365](https://aka.ms/RestoreDeletedGroup) untuk masuk ke daftar tentang grup dan tim yang dihapus.</span><span class="sxs-lookup"><span data-stu-id="450ee-104">Go to the [Microsoft 365 admin center](https://aka.ms/RestoreDeletedGroup) to log in to a list of your the deleted groups and teams.</span></span>

    <span data-ttu-id="450ee-105">**Catatan:** Masuk menggunakan akun yang ditetapkan untuk administrator penyewa atau peran admin grup.</span><span class="sxs-lookup"><span data-stu-id="450ee-105">**Note:** Log in using the account that is assigned to either the tenant administrator or the groups admin role.</span></span>

1. <span data-ttu-id="450ee-106">Pilih grup/Teams Microsoft 365 yang dihapus untuk dipulihkan, lalu klik **pulihkan grup.**</span><span class="sxs-lookup"><span data-stu-id="450ee-106">Select the deleted Microsoft 365 group/Teams to be restored and click **restore group**.</span></span>

    <span data-ttu-id="450ee-107">Jika grup tidak bisa dipulihkan karena alamat SMTP yang berkonflik, gunakan perintah berikut untuk menemukan objek yang menyebabkan konflik dan menghapus alamat SMTP:</span><span class="sxs-lookup"><span data-stu-id="450ee-107">If the group can't be restored because of a conflicting SMTP address, use following command to find the object that’s causing conflict and remove the SMTP address:</span></span>

    `Get-Recipient -Filter "EmailAddresses -eq '<conflictingsmtpaddress>'"`

    <span data-ttu-id="450ee-108">**Catatan:** Dalam beberapa kasus, mungkin akan memakan waktu hingga 24 jam agar grup dan semua datanya dipulihkan.</span><span class="sxs-lookup"><span data-stu-id="450ee-108">**Note:** In some cases, it might take as long as 24 hours for the group and all of its data to be restored.</span></span>

    <span data-ttu-id="450ee-109">Untuk informasi selengkapnya, atau untuk mempelajari cara memulihkan grup menggunakan PowerShell, [lihat Memulihkan grup Microsoft 365 yang dihapus.](https://go.microsoft.com/fwlink/?linkid=867802)</span><span class="sxs-lookup"><span data-stu-id="450ee-109">For more info, or to learn how to restore groups using PowerShell, see [Restore a deleted Microsoft 365 group](https://go.microsoft.com/fwlink/?linkid=867802).</span></span>