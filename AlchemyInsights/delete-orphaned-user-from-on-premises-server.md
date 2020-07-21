---
title: Menghapus pengguna yatim piatu dari server lokal
ms.author: pebaum
author: pebaum
manager: scotv
ms.date: 07/20/2020
ms.audience: Admin
ms.topic: article
ROBOTS: NOINDEX, NOFOLLOW
localization_priority: Priority
ms.collection: Adm_O365
ms.custom:
- "1725"
- "9000179"
ms.openlocfilehash: 7927c0684d2f5289f92506d7d05d5b1a3b43b658
ms.sourcegitcommit: b0b050a83db28566b68e3ec09810c6b94280008e
ms.translationtype: MT
ms.contentlocale: id-ID
ms.lasthandoff: 07/20/2020
ms.locfileid: "45198182"
---
# <a name="delete-orphaned-user-from-on-premises-server"></a><span data-ttu-id="90fd7-102">Menghapus pengguna yatim piatu dari server lokal</span><span class="sxs-lookup"><span data-stu-id="90fd7-102">Delete orphaned user from on-premises server</span></span>

<span data-ttu-id="90fd7-103">Untuk menghapus pengguna yang ditinggalkan, ikuti langkah berikut:</span><span class="sxs-lookup"><span data-stu-id="90fd7-103">To remove an orphaned user, follow these steps:</span></span>

1. <span data-ttu-id="90fd7-104">Memaksa sinkronisasi direktori dengan mengikuti petunjuk dalam [apa yang hibrid identitas dengan Azure Active Directory?](https://technet.microsoft.com/library/jj151771.aspx#bkmk_synchronizedirectories).</span><span class="sxs-lookup"><span data-stu-id="90fd7-104">Force directory synchronization by following the instructions in [What is hybrid identity with Azure Active Directory?](https://technet.microsoft.com/library/jj151771.aspx#bkmk_synchronizedirectories).</span></span>

2. <span data-ttu-id="90fd7-105">Untuk memverifikasi sinkronisasi direktori, lihat [apa yang dimaksud dengan identitas hibrid dengan Azure Active Directory?](https://technet.microsoft.com/library/jj151797.aspx).</span><span class="sxs-lookup"><span data-stu-id="90fd7-105">To verify directory synchronization, see [What is hybrid identity with Azure Active Directory?](https://technet.microsoft.com/library/jj151797.aspx).</span></span>

3. <span data-ttu-id="90fd7-106">Jika fungsi sinkronisasi dengan benar tetapi penghapusan objek direktori aktif tidak dialihkan ke Azure AD, secara manual menghapus objek ditinggalkan dengan menggunakan salah satu dari cmdlets Azure Active Directory modul untuk Windows PowerShell berikut ini:</span><span class="sxs-lookup"><span data-stu-id="90fd7-106">If sync functions correctly but the Active Directory object deletion does not propagate to Azure AD, manually remove the orphaned object by using one of the following Azure Active Directory Module for Windows PowerShell cmdlets:</span></span>

    <span data-ttu-id="90fd7-107">Hapus-MsolContact</span><span class="sxs-lookup"><span data-stu-id="90fd7-107">Remove-MsolContact</span></span>  
    <span data-ttu-id="90fd7-108">Hapus-MsolGroup</span><span class="sxs-lookup"><span data-stu-id="90fd7-108">Remove-MsolGroup</span></span>  
    <span data-ttu-id="90fd7-109">Hapus-MsolUser</span><span class="sxs-lookup"><span data-stu-id="90fd7-109">Remove-MsolUser</span></span>

    <span data-ttu-id="90fd7-110">Misalnya, untuk menghapus ditinggalkan ID pengguna john.smith@contoso.com, awalnya dibuat dengan menggunakan sinkronisasi direktori, Jalankan cmdlet:</span><span class="sxs-lookup"><span data-stu-id="90fd7-110">For example, to remove orphaned user ID john.smith@contoso.com, originally created by using directory synchronization, run the cmdlet:</span></span>

    <span data-ttu-id="90fd7-111">Hapus-MsolUser-UserPrincipalName John.Smith@Contoso.com</span><span class="sxs-lookup"><span data-stu-id="90fd7-111">Remove-MsolUser –UserPrincipalName John.Smith@Contoso.com</span></span>