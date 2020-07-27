---
title: Beberapa pengguna mendapatkan galat Akses ditolak saat menambahkan Add-in di Outlook
ms.author: pebaum
author: pebaum
manager: scotv
ms.date: 07/23/2020
ms.audience: Admin
ms.topic: article
ROBOTS: NOINDEX, NOFOLLOW
localization_priority: Priority
ms.collection: Adm_O365
ms.custom:
- "5892"
- "6700008"
ms.openlocfilehash: 624d880c535b7d8888b676ff23c774c6d138a75a
ms.sourcegitcommit: 07e56267dedfc4cec1143072c791670cbf81186b
ms.translationtype: MT
ms.contentlocale: id-ID
ms.lasthandoff: 07/24/2020
ms.locfileid: "45423716"
---
# <a name="multiple-users-get-access-denied-error-while-adding-add-ins-in-outlook"></a><span data-ttu-id="01fce-102">Beberapa pengguna mendapatkan galat Akses ditolak saat menambahkan Add-in di Outlook</span><span class="sxs-lookup"><span data-stu-id="01fce-102">Multiple users get Access Denied error while adding add-ins in Outlook</span></span>

<span data-ttu-id="01fce-103">Anda dapat menentukan administrator di organisasi yang memiliki izin untuk menginstal dan mengelola add-in untuk Outlook.</span><span class="sxs-lookup"><span data-stu-id="01fce-103">You can specify which administrators in your organization have permissions to install and manage add-ins for Outlook.</span></span> <span data-ttu-id="01fce-104">Anda juga dapat menentukan pengguna mana di organisasi Anda yang memiliki izin untuk menginstal dan mengelola add-in untuk penggunaannya sendiri.</span><span class="sxs-lookup"><span data-stu-id="01fce-104">You can also specify which users in your organization have permission to install and manage add-ins for their own use.</span></span>

<span data-ttu-id="01fce-105">Untuk detailnya, lihat [menentukan administrator dan pengguna yang dapat menginstal dan mengelola add-in untuk Outlook](https://docs.microsoft.com/exchange/clients-and-mobile-in-exchange-online/add-ins-for-outlook/specify-who-can-install-and-manage-add-ins).</span><span class="sxs-lookup"><span data-stu-id="01fce-105">For details, see [Specify the administrators and users who can install and manage add-ins for Outlook](https://docs.microsoft.com/exchange/clients-and-mobile-in-exchange-online/add-ins-for-outlook/specify-who-can-install-and-manage-add-ins).</span></span>

<span data-ttu-id="01fce-106">Untuk memverifikasi bahwa Anda telah berhasil menetapkan izin untuk pengguna, ganti <Role Name> dengan nama peran untuk memverifikasi, dan jalankan perintah berikut ini di Exchange Online PowerShell:</span><span class="sxs-lookup"><span data-stu-id="01fce-106">To verify that you've successfully assigned permissions for a user, replace <Role Name> with the name of the role to verify, and run the following command in Exchange Online PowerShell:</span></span>

<span data-ttu-id="01fce-107">Get-ManagementRoleAssignment-peran " <Role Name> "-geteffectiveusers</span><span class="sxs-lookup"><span data-stu-id="01fce-107">Get-ManagementRoleAssignment -Role "<Role Name>" -GetEffectiveUsers</span></span>

<span data-ttu-id="01fce-108">Contoh ini menunjukkan cara memverifikasi siapa yang telah Anda tetapkan izin untuk menginstal Add-in dari Office Store untuk organisasi.</span><span class="sxs-lookup"><span data-stu-id="01fce-108">This example shows you how to verify whom you've assigned permissions to install add-ins from the Office Store for the organization.</span></span>

<span data-ttu-id="01fce-109">Powershell</span><span class="sxs-lookup"><span data-stu-id="01fce-109">PowerShell</span></span>

<span data-ttu-id="01fce-110">-Peran "org Marketplace Apps"-GetEffectiveUsers</span><span class="sxs-lookup"><span data-stu-id="01fce-110">-Role "Org Marketplace Apps" -GetEffectiveUsers</span></span>

<span data-ttu-id="01fce-111">Dalam hasil, Get-ManagementRoleAssignment, Tinjau entri di kolom pengguna efektif.</span><span class="sxs-lookup"><span data-stu-id="01fce-111">In the results, Get-ManagementRoleAssignment, review the entries in the Effective Users column.</span></span>

<span data-ttu-id="01fce-112">Untuk informasi sintaks dan parameter terperinci, lihat [Get-ManagementRoleAssignment](https://docs.microsoft.com/powershell/module/exchange/get-managementroleassignment).</span><span class="sxs-lookup"><span data-stu-id="01fce-112">For detailed syntax and parameter information, see [Get-ManagementRoleAssignment](https://docs.microsoft.com/powershell/module/exchange/get-managementroleassignment).</span></span>
 