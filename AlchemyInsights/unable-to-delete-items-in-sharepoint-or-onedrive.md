---
title: Tidak dapat menghapus item di SharePoint atau OneDrive
ms.author: pebaum
author: pebaum
ms.audience: ITPro
ms.topic: article
ROBOTS: NOINDEX, NOFOLLOW
localization_priority: Normal
ms.custom:
- "1851"
- "2377"
- "9000255"
ms.assetid: ''
ms.openlocfilehash: abfcb91c6040aeed759d697ca63546ccea8ede97
ms.sourcegitcommit: c5e800313a6f211386a384716e5fa18e7fcc8c1c
ms.translationtype: MT
ms.contentlocale: id-ID
ms.lasthandoff: 01/28/2020
ms.locfileid: "41571263"
---
# <a name="unable-to-delete-items"></a><span data-ttu-id="b4c85-102">Tidak dapat menghapus item</span><span class="sxs-lookup"><span data-stu-id="b4c85-102">Unable to delete items</span></span>

<span data-ttu-id="b4c85-103">Kebijakan retensi dapat menyebabkan ini, Anda perlu menonaktifkan atau mengecualikan masing-masing memegang yang menyebabkan masalah ini.</span><span class="sxs-lookup"><span data-stu-id="b4c85-103">Retention policies can cause this, you need to either disable or exclude respective hold that's causing this issue.</span></span> <span data-ttu-id="b4c85-104">Setelah kebijakan retensi atau tahan dihapus, mungkin diperlukan waktu hingga 24 jam agar perubahan diterapkan.</span><span class="sxs-lookup"><span data-stu-id="b4c85-104">After a retention policy or hold is removed, it may take up to 24 hours for the change to take effect.</span></span> <span data-ttu-id="b4c85-105">Pastikan bahwa tidak ada pengaturan [kebijakan penyimpanan](https://docs.microsoft.com/office365/securitycompliance/retention-policies) pada item.</span><span class="sxs-lookup"><span data-stu-id="b4c85-105">Ensure that there is not a [retention policy](https://docs.microsoft.com/office365/securitycompliance/retention-policies) setup on the item.</span></span>

<span data-ttu-id="b4c85-106">Situs mungkin telah melebihi batas penyimpanan, meningkatkan [kuota situs](https://docs.microsoft.com/powershell/module/sharepoint-online/set-sposite?view=sharepoint-ps) dan menghapus item.</span><span class="sxs-lookup"><span data-stu-id="b4c85-106">The site might have exceeded storage limit, increase the [site quota](https://docs.microsoft.com/powershell/module/sharepoint-online/set-sposite?view=sharepoint-ps) and delete the item.</span></span>

<span data-ttu-id="b4c85-107">Pastikan item tidak [diperiksa](https://support.office.com/article/check-out-check-in-or-discard-changes-to-files-in-a-library-7e2c12a9-a874-4393-9511-1378a700f6de) ke pengguna lain.</span><span class="sxs-lookup"><span data-stu-id="b4c85-107">Ensure the item is not [checked out](https://support.office.com/article/check-out-check-in-or-discard-changes-to-files-in-a-library-7e2c12a9-a874-4393-9511-1378a700f6de) to another user.</span></span>

<span data-ttu-id="b4c85-108">Akhirnya, administrator dapat menggunakan [pola dan praktik SharePoint](https://docs.microsoft.com/powershell/sharepoint/sharepoint-pnp/sharepoint-pnp-cmdlets?view=sharepoint-ps#installation) (PNP) yang berisi pustaka perintah PowerShell yang memungkinkan Anda untuk melakukan tindakan manajemen yang kompleks seperti memaksa menghapus item yang membandel.</span><span class="sxs-lookup"><span data-stu-id="b4c85-108">Finally, administrators can use [SharePoint Patterns and Practices](https://docs.microsoft.com/powershell/sharepoint/sharepoint-pnp/sharepoint-pnp-cmdlets?view=sharepoint-ps#installation) (PnP) which contains a library of PowerShell commands that allow you to perform complex management actions such as force deleting stubborn items.</span></span>
- [<span data-ttu-id="b4c85-109">Hapus berkas PNP</span><span class="sxs-lookup"><span data-stu-id="b4c85-109">Remove PNP File</span></span>](https://docs.microsoft.com/powershell/module/sharepoint-pnp/remove-pnpfile?view=sharepoint-ps)
- [<span data-ttu-id="b4c85-110">Hapus folder PNP</span><span class="sxs-lookup"><span data-stu-id="b4c85-110">Remove PNP Folder</span></span>](https://docs.microsoft.com/powershell/module/sharepoint-pnp/remove-pnpfolder?view=sharepoint-ps)
- [<span data-ttu-id="b4c85-111">Hapus item daftar PNP</span><span class="sxs-lookup"><span data-stu-id="b4c85-111">Remove PNP List Item</span></span>](https://docs.microsoft.com/powershell/module/sharepoint-pnp/remove-pnplistitem?view=sharepoint-ps)
- [<span data-ttu-id="b4c85-112">Hapus daftar PNP</span><span class="sxs-lookup"><span data-stu-id="b4c85-112">Remove PNP List</span></span>](https://docs.microsoft.com/powershell/module/sharepoint-pnp/remove-pnplist?view=sharepoint-ps)
- [<span data-ttu-id="b4c85-113">Hapus kolom PNP (kolom)</span><span class="sxs-lookup"><span data-stu-id="b4c85-113">Remove PNP Field (Column)</span></span>](https://docs.microsoft.com/powershell/module/sharepoint-pnp/remove-pnpfield?view=sharepoint-ps)