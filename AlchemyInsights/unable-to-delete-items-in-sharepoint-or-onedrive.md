---
title: Tidak dapat menghapus item di SharePoint atau OneDrive
ms.author: pebaum
author: Techwriter40
ms.audience: ITPro
ms.topic: article
ROBOTS: NOINDEX, NOFOLLOW
localization_priority: Normal
ms.custom:
- "1851"
- "2377"
- "9000255"
ms.assetid: ''
ms.openlocfilehash: 3cc168846999c6880b95edfaedb2df8cf6e843a6
ms.sourcegitcommit: 037331d71f06750d972c0b6278b23bb15c4806ca
ms.translationtype: MT
ms.contentlocale: id-ID
ms.lasthandoff: 10/18/2019
ms.locfileid: "36748564"
---
# <a name="unable-to-delete-items"></a><span data-ttu-id="fb366-102">Tidak dapat menghapus item</span><span class="sxs-lookup"><span data-stu-id="fb366-102">Unable to delete items</span></span>

<span data-ttu-id="fb366-103">Setelah masalah menghapus item SharePoint?</span><span class="sxs-lookup"><span data-stu-id="fb366-103">Having issues deleting SharePoint items?</span></span>

- <span data-ttu-id="fb366-104">Selalu pastikan Anda memiliki izin yang [sesuai](https://docs.microsoft.com/sharepoint/default-sharepoint-groups) untuk menghapus item atau meminta [administrator kumpulan situs](https://docs.microsoft.com/sharepoint/customize-sharepoint-site-permissions#add-change-or-remove-a-site-collection-administrator) mencoba menghapus item.</span><span class="sxs-lookup"><span data-stu-id="fb366-104">Always make sure you have the [appropriate permissions](https://docs.microsoft.com/sharepoint/default-sharepoint-groups) to delete the item or have a [site collection administrator](https://docs.microsoft.com/sharepoint/customize-sharepoint-site-permissions#add-change-or-remove-a-site-collection-administrator) attempt remove the item.</span></span>

- <span data-ttu-id="fb366-105">Pastikan bahwa tidak ada pengaturan [kebijakan penyimpanan](https://docs.microsoft.com/office365/securitycompliance/retention-policies) pada item.</span><span class="sxs-lookup"><span data-stu-id="fb366-105">Ensure that there is not a [retention policy](https://docs.microsoft.com/office365/securitycompliance/retention-policies) setup on the item.</span></span>

- <span data-ttu-id="fb366-106">Pastikan item tidak [diperiksa](https://support.office.com/article/check-out-check-in-or-discard-changes-to-files-in-a-library-7e2c12a9-a874-4393-9511-1378a700f6de) ke pengguna lain.</span><span class="sxs-lookup"><span data-stu-id="fb366-106">Ensure the item is not [checked out](https://support.office.com/article/check-out-check-in-or-discard-changes-to-files-in-a-library-7e2c12a9-a874-4393-9511-1378a700f6de) to another user.</span></span>

- <span data-ttu-id="fb366-107">Akhirnya, administrator dapat menggunakan [pola dan praktik SharePoint](https://docs.microsoft.com/powershell/sharepoint/sharepoint-pnp/sharepoint-pnp-cmdlets?view=sharepoint-ps#installation) (PNP) yang berisi pustaka perintah PowerShell yang memungkinkan Anda untuk melakukan tindakan manajemen yang kompleks seperti memaksa menghapus item yang membandel.</span><span class="sxs-lookup"><span data-stu-id="fb366-107">Finally, administrators can use [SharePoint Patterns and Practices](https://docs.microsoft.com/powershell/sharepoint/sharepoint-pnp/sharepoint-pnp-cmdlets?view=sharepoint-ps#installation) (PnP) which contains a library of PowerShell commands that allow you to perform complex management actions such as force deleting stubborn items.</span></span>
- [<span data-ttu-id="fb366-108">Hapus berkas PNP</span><span class="sxs-lookup"><span data-stu-id="fb366-108">Remove PNP File</span></span>](https://docs.microsoft.com/powershell/module/sharepoint-pnp/remove-pnpfile?view=sharepoint-ps)
- [<span data-ttu-id="fb366-109">Hapus folder PNP</span><span class="sxs-lookup"><span data-stu-id="fb366-109">Remove PNP Folder</span></span>](https://docs.microsoft.com/powershell/module/sharepoint-pnp/remove-pnpfolder?view=sharepoint-ps)
- [<span data-ttu-id="fb366-110">Hapus item daftar PNP</span><span class="sxs-lookup"><span data-stu-id="fb366-110">Remove PNP List Item</span></span>](https://docs.microsoft.com/powershell/module/sharepoint-pnp/remove-pnplistitem?view=sharepoint-ps)
- [<span data-ttu-id="fb366-111">Hapus daftar PNP</span><span class="sxs-lookup"><span data-stu-id="fb366-111">Remove PNP List</span></span>](https://docs.microsoft.com/powershell/module/sharepoint-pnp/remove-pnplist?view=sharepoint-ps)
- [<span data-ttu-id="fb366-112">Hapus kolom PNP (kolom)</span><span class="sxs-lookup"><span data-stu-id="fb366-112">Remove PNP Field (Column)</span></span>](https://docs.microsoft.com/powershell/module/sharepoint-pnp/remove-pnpfield?view=sharepoint-ps)