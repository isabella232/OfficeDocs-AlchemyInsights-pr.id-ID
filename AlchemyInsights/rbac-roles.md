---
title: 'Peran RBAC '
ms.author: v-aiyengar
author: AshaIyengar21
manager: dansimp
ms.audience: Admin
ms.topic: article
ms.service: o365-administration
ROBOTS: NOINDEX, NOFOLLOW
localization_priority: Normal
ms.collection: Adm_O365
ms.custom:
- "9003230"
- "7265"
ms.openlocfilehash: 7c4c9d1a76f395dfb2f831d555199b76c354ca57
ms.sourcegitcommit: 2e4a5153e530bf15744a52e982eeb0d99757e9d2
ms.translationtype: MT
ms.contentlocale: id-ID
ms.lasthandoff: 12/04/2020
ms.locfileid: "49583548"
---
# <a name="rbac-rules"></a><span data-ttu-id="c05a5-102">Aturan RBAC</span><span class="sxs-lookup"><span data-stu-id="c05a5-102">RBAC rules</span></span>

<span data-ttu-id="c05a5-103">Jika Anda mendapatkan kesalahan izin:</span><span class="sxs-lookup"><span data-stu-id="c05a5-103">If you get the permission error:</span></span> 

- <span data-ttu-id="c05a5-104">**Klien dengan ID objek tidak memiliki otorisasi untuk melakukan tindakan di atas lingkup (kode: Otorisasigagal)**: ketika Anda mencoba membuat sumber daya, periksa apakah saat ini Anda masuk dengan pengguna yang diberi peran yang memiliki izin menulis ke sumber daya di lingkup yang dipilih.</span><span class="sxs-lookup"><span data-stu-id="c05a5-104">**The client with object id does not have authorization to perform action over scope (code: AuthorizationFailed)**: when you try to create a resource, check that you are currently signed in with a user that is assigned a role that has write permission to the resource at the selected scope.</span></span> <span data-ttu-id="c05a5-105">Misalnya, untuk mengelola mesin virtual dalam grup sumber daya, Anda harus memiliki peran [kontributor mesin virtual](https://docs.microsoft.com/azure/role-based-access-control/built-in-roles?WT.mc_id=Portal-Microsoft_Azure_Support#virtual-machine-contributor) di grup sumber daya (atau lingkup induk).</span><span class="sxs-lookup"><span data-stu-id="c05a5-105">For example, to manage virtual machines in a resource group, you should have the [Virtual Machine Contributor](https://docs.microsoft.com/azure/role-based-access-control/built-in-roles?WT.mc_id=Portal-Microsoft_Azure_Support#virtual-machine-contributor) role on the resource group (or parent scope).</span></span> <span data-ttu-id="c05a5-106">Untuk daftar izin untuk setiap peran bawaan, lihat [peran bawaan untuk sumber daya Azure](https://docs.microsoft.com/azure/role-based-access-control/built-in-roles?WT.mc_id=Portal-Microsoft_Azure_Support).</span><span class="sxs-lookup"><span data-stu-id="c05a5-106">For a list of the permissions for each built-in role, see [Built-in roles for Azure resources](https://docs.microsoft.com/azure/role-based-access-control/built-in-roles?WT.mc_id=Portal-Microsoft_Azure_Support).</span></span>
- <span data-ttu-id="c05a5-107">**Anda tidak memiliki izin untuk membuat permintaan dukungan**: ketika mencoba membuat atau memperbarui tiket dukungan, periksa apakah Anda saat ini masuk dengan pengguna yang ditetapkan peran yang memiliki izin Microsoft. support/supportticket/Write, seperti [kontributor permintaan dukungan](https://docs.microsoft.com/azure/role-based-access-control/built-in-roles?WT.mc_id=Portal-Microsoft_Azure_Support#support-request-contributor).</span><span class="sxs-lookup"><span data-stu-id="c05a5-107">**You don't have permission to create a support request**: when you try to create or update a support ticket, check that you are currently signed in with a user that is assigned a role that has the Microsoft.Support/supportTickets/write permission, such as [Support Request Contributor](https://docs.microsoft.com/azure/role-based-access-control/built-in-roles?WT.mc_id=Portal-Microsoft_Azure_Support#support-request-contributor).</span></span>
- <span data-ttu-id="c05a5-108">**Tidak ada lagi penetapan peran yang bisa dibuat (kode: peran Roleassignmentlimitterlamp)**: ketika Anda mencoba menetapkan peran, cobalah untuk mengurangi jumlah penetapan peran dengan menetapkan peran ke grup.</span><span class="sxs-lookup"><span data-stu-id="c05a5-108">**No more role assignments can be created (code: RoleAssignmentLimitExceeded)**: when you try to assign a role, try to reduce the number of role assignments by assigning roles to groups instead.</span></span> <span data-ttu-id="c05a5-109">Azure mendukung hingga **2000** penetapan peran per langganan.</span><span class="sxs-lookup"><span data-stu-id="c05a5-109">Azure supports up to **2000** role assignments per subscription.</span></span>

<span data-ttu-id="c05a5-110">Untuk detail selengkapnya tentang peran Azure RBAC, lihat [peran AZURE RBAC](https://docs.microsoft.com/azure/role-based-access-control/role-assignments-portal?WT.mc_id=Portal-Microsoft_Azure_Support).</span><span class="sxs-lookup"><span data-stu-id="c05a5-110">For more details on Azure RBAC roles, see [Azure RBAC roles](https://docs.microsoft.com/azure/role-based-access-control/role-assignments-portal?WT.mc_id=Portal-Microsoft_Azure_Support).</span></span>
