---
title: Tidak dapat menghapus item di SharePoint atau OneDrive
ms.author: pebaum
author: pebaum
ms.audience: ITPro
ms.topic: article
ms.service: o365-administration
ROBOTS: NOINDEX, NOFOLLOW
localization_priority: Normal
ms.custom:
- "1851"
- "2377"
- "9000255"
ms.assetid: ''
ms.openlocfilehash: db45aa8df40484fdcda7c430f1ca27482a1dd4ce
ms.sourcegitcommit: a9415f3ae8c7ba267b5134bcbdc1e070cea41a0f
ms.translationtype: MT
ms.contentlocale: id-ID
ms.lasthandoff: 11/12/2020
ms.locfileid: "49019586"
---
# <a name="unable-to-delete-items"></a><span data-ttu-id="c9516-102">Tidak dapat menghapus item</span><span class="sxs-lookup"><span data-stu-id="c9516-102">Unable to delete items</span></span>

- <span data-ttu-id="c9516-103">Kebijakan penyimpanan bisa menyebabkan hal ini, Anda perlu menonaktifkan atau mengecualikan penangguhan masing-masing yang menyebabkan masalah ini.</span><span class="sxs-lookup"><span data-stu-id="c9516-103">Retention policies can cause this, you need to either disable or exclude respective hold that's causing this issue.</span></span> <span data-ttu-id="c9516-104">Setelah kebijakan atau penangguhan penyimpanan dihapus, mungkin perlu waktu hingga 24 jam agar perubahan diterapkan.</span><span class="sxs-lookup"><span data-stu-id="c9516-104">After a retention policy or hold is removed, it may take up to 24 hours for the change to take effect.</span></span> <span data-ttu-id="c9516-105">Pastikan bahwa tidak ada penyetelan [kebijakan penyimpanan](https://docs.microsoft.com/microsoft-365/compliance/retention-policies) pada item.</span><span class="sxs-lookup"><span data-stu-id="c9516-105">Ensure that there is not a [retention policy](https://docs.microsoft.com/microsoft-365/compliance/retention-policies) setup on the item.</span></span>

- <span data-ttu-id="c9516-106">Situs mungkin telah melebihi batas penyimpanan, menambah [kuota situs](https://docs.microsoft.com/powershell/module/sharepoint-online/set-sposite?view=sharepoint-ps) dan menghapus item.</span><span class="sxs-lookup"><span data-stu-id="c9516-106">The site might have exceeded storage limit, increase the [site quota](https://docs.microsoft.com/powershell/module/sharepoint-online/set-sposite?view=sharepoint-ps) and delete the item.</span></span>

- <span data-ttu-id="c9516-107">Pastikan item tidak [dicentang](https://support.office.com/article/check-out-check-in-or-discard-changes-to-files-in-a-library-7e2c12a9-a874-4393-9511-1378a700f6de) ke pengguna lain.</span><span class="sxs-lookup"><span data-stu-id="c9516-107">Ensure the item is not [checked out](https://support.office.com/article/check-out-check-in-or-discard-changes-to-files-in-a-library-7e2c12a9-a874-4393-9511-1378a700f6de) to another user.</span></span>

- <span data-ttu-id="c9516-108">Akhirnya, administrator dapat menggunakan [SharePoint Patterns and Practices](https://docs.microsoft.com/powershell/sharepoint/sharepoint-pnp/sharepoint-pnp-cmdlets?view=sharepoint-ps#installation) (PNP) yang berisi pustaka perintah PowerShell yang memungkinkan Anda melakukan tindakan manajemen yang kompleks seperti memaksa penghapusan item yang membandel.</span><span class="sxs-lookup"><span data-stu-id="c9516-108">Finally, administrators can use [SharePoint Patterns and Practices](https://docs.microsoft.com/powershell/sharepoint/sharepoint-pnp/sharepoint-pnp-cmdlets?view=sharepoint-ps#installation) (PnP) which contains a library of PowerShell commands that allow you to perform complex management actions such as force deleting stubborn items.</span></span>
- [<span data-ttu-id="c9516-109">Hapus file PNP</span><span class="sxs-lookup"><span data-stu-id="c9516-109">Remove PNP File</span></span>](https://docs.microsoft.com/powershell/module/sharepoint-pnp/remove-pnpfile?view=sharepoint-ps)
- [<span data-ttu-id="c9516-110">Hapus folder PNP</span><span class="sxs-lookup"><span data-stu-id="c9516-110">Remove PNP Folder</span></span>](https://docs.microsoft.com/powershell/module/sharepoint-pnp/remove-pnpfolder?view=sharepoint-ps)
- [<span data-ttu-id="c9516-111">Hapus item daftar PNP</span><span class="sxs-lookup"><span data-stu-id="c9516-111">Remove PNP List Item</span></span>](https://docs.microsoft.com/powershell/module/sharepoint-pnp/remove-pnplistitem?view=sharepoint-ps)
- [<span data-ttu-id="c9516-112">Hapus daftar PNP</span><span class="sxs-lookup"><span data-stu-id="c9516-112">Remove PNP List</span></span>](https://docs.microsoft.com/powershell/module/sharepoint-pnp/remove-pnplist?view=sharepoint-ps)
- [<span data-ttu-id="c9516-113">Menghapus bidang PNP (kolom)</span><span class="sxs-lookup"><span data-stu-id="c9516-113">Remove PNP Field (Column)</span></span>](https://docs.microsoft.com/powershell/module/sharepoint-pnp/remove-pnpfield?view=sharepoint-ps)