---
title: Sinkronisasi grup
ms.author: v-smandalika
author: v-smandalika
manager: dansimp
ms.date: 02/15/2021
ms.audience: Admin
ms.topic: article
ms.service: o365-administration
ROBOTS: NOINDEX, NOFOLLOW
localization_priority: Priority
ms.collection: Adm_O365
ms.custom:
- "8304"
- "9003234"
ms.openlocfilehash: 52c19b6dcc79968150a188b389c5481c122f7945
ms.sourcegitcommit: 6900c2b7208ca51a9873dfc2e00be6f66cb25e3c
ms.translationtype: MT
ms.contentlocale: id-ID
ms.lasthandoff: 02/15/2021
ms.locfileid: "50256794"
---
# <a name="group-sync"></a><span data-ttu-id="56759-102">Sinkronisasi grup</span><span class="sxs-lookup"><span data-stu-id="56759-102">Group sync</span></span>

<span data-ttu-id="56759-103">Artikel ini menyediakan panduan pada sinkronisasi grup.</span><span class="sxs-lookup"><span data-stu-id="56759-103">This article provides guidance on group synchronization.</span></span>

1. <span data-ttu-id="56759-104">Jika admin global atau pemilik grup tidak dapat mengubah properti grup atau menambahkan anggota atau menetapkan pemilik di portal Azure, pastikan sumber otoritas untuk grup adalah Azure Active Directory (Azure AD) untuk admin global atau pemilik grup untuk mengubah grup.</span><span class="sxs-lookup"><span data-stu-id="56759-104">If a global admin or group owner is not able to modify group properties or add members or assign owners in the Azure portal, ensure the source of the authority for the group is Azure Active Directory (Azure AD) for the global admin or group owner to modify the group.</span></span>
2. <span data-ttu-id="56759-105">Sebelum mencoba menghapus grup yang disinkronkan di Azure AD, pastikan Anda telah [menghapus semua lisensi yang ditetapkan](https://docs.microsoft.com/azure/active-directory/enterprise-users/licensing-group-advanced) untuk menghindari kesalahan.</span><span class="sxs-lookup"><span data-stu-id="56759-105">Before attempting to delete a synced group in Azure AD, ensure you have [deleted all assigned licenses](https://docs.microsoft.com/azure/active-directory/enterprise-users/licensing-group-advanced) to avoid errors.</span></span>

<span data-ttu-id="56759-106">Untuk memahami cara menyinkronkan pengguna, grup, dan kontak, lihat [sinkronisasi AZURE AD Connect](https://docs.microsoft.com/azure/active-directory/hybrid/concept-azure-ad-connect-sync-user-and-contacts), dan ikuti [sinkronisasi grup lokal ke AZURE menggunakan Azure AD Connect](https://docs.microsoft.com/azure/active-directory/hybrid/whatis-hybrid-identity?WT.mc_id=Portal-Microsoft_Azure_Support) untuk menyinkronkan grup pada perm menggunakan AD Connect.</span><span class="sxs-lookup"><span data-stu-id="56759-106">For understanding how to sync users, groups and contacts, see [Azure AD Connect Sync](https://docs.microsoft.com/azure/active-directory/hybrid/concept-azure-ad-connect-sync-user-and-contacts), and follow [Syncing an on-premises group to Azure using Azure AD Connect](https://docs.microsoft.com/azure/active-directory/hybrid/whatis-hybrid-identity?WT.mc_id=Portal-Microsoft_Azure_Support) to sync on-perm groups using AD connect.</span></span>

<span data-ttu-id="56759-107">Ikuti panduan ini [pemecahan masalah kesalahan selama sinkronisasi](https://docs.microsoft.com/azure/active-directory/hybrid/tshoot-connect-sync-errors) untuk memecahkan masalah kesalahan umum selama sinkronisasi.</span><span class="sxs-lookup"><span data-stu-id="56759-107">Follow this guide [Troubleshooting Errors during synchronization](https://docs.microsoft.com/azure/active-directory/hybrid/tshoot-connect-sync-errors) to troubleshoot common errors during synchronization.</span></span>

