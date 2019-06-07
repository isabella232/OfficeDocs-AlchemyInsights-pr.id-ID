---
title: Tidak dapat menghapus item dalam SharePoint atau OneDrive
ms.author: kirks
author: Techwriter40
ms.audience: ITPro
ms.topic: article
ROBOTS: NOINDEX, NOFOLLOW
localization_priority: Normal
ms.assetid: ''
ms.openlocfilehash: 82a19c8ea218834b71901e95747da0c99243893e
ms.sourcegitcommit: 4b7e478ce700c0b781efec3857ac4dce5bdf00c6
ms.translationtype: MT
ms.contentlocale: id-ID
ms.lasthandoff: 06/07/2019
ms.locfileid: "34757928"
---
# <a name="unable-to-delete-items"></a><span data-ttu-id="e4eed-102">Tidak dapat menghapus item</span><span class="sxs-lookup"><span data-stu-id="e4eed-102">Unable to delete items</span></span>

<span data-ttu-id="e4eed-103">Mengalami masalah saat menghapus item?</span><span class="sxs-lookup"><span data-stu-id="e4eed-103">Having issues deleting items?</span></span>

- <span data-ttu-id="e4eed-104">Selalu pastikan Anda memiliki [izin sesuai](https://docs.microsoft.com/sharepoint/default-sharepoint-groups) untuk menghapus item atau memiliki usaha [site koleksi administrator](https://docs.microsoft.com/sharepoint/customize-sharepoint-site-permissions#add-change-or-remove-a-site-collection-administrator) yang menghapus item.</span><span class="sxs-lookup"><span data-stu-id="e4eed-104">Always make sure you have the [appropriate permissions](https://docs.microsoft.com/sharepoint/default-sharepoint-groups) to delete the item or have a [site collection administrator](https://docs.microsoft.com/sharepoint/customize-sharepoint-site-permissions#add-change-or-remove-a-site-collection-administrator) attempt remove the item.</span></span>

- <span data-ttu-id="e4eed-105">Memastikan bahwa tidak ada setup [kebijakan pengarsipan](https://docs.microsoft.com/office365/securitycompliance/retention-policies) pada item.</span><span class="sxs-lookup"><span data-stu-id="e4eed-105">Ensure that there is not a [retention policy](https://docs.microsoft.com/office365/securitycompliance/retention-policies) setup on the item.</span></span>

- <span data-ttu-id="e4eed-106">Memastikan item tidak [memeriksa](https://support.office.com/article/check-out-check-in-or-discard-changes-to-files-in-a-library-7e2c12a9-a874-4393-9511-1378a700f6de) untuk pengguna lain.</span><span class="sxs-lookup"><span data-stu-id="e4eed-106">Ensure the item is not [checked out](https://support.office.com/article/check-out-check-in-or-discard-changes-to-files-in-a-library-7e2c12a9-a874-4393-9511-1378a700f6de) to another user.</span></span>

- <span data-ttu-id="e4eed-107">Akhirnya, administrator dapat menggunakan [pola SharePoint dan praktek](https://docs.microsoft.com/powershell/sharepoint/sharepoint-pnp/sharepoint-pnp-cmdlets?view=sharepoint-ps#installation) (PnP) yang berisi perpustakaan PowerShell perintah yang memungkinkan Anda untuk melakukan tindakan manajemen yang kompleks seperti memaksa menghapus item keras kepala.</span><span class="sxs-lookup"><span data-stu-id="e4eed-107">Finally, administrators can use [SharePoint Patterns and Practices](https://docs.microsoft.com/powershell/sharepoint/sharepoint-pnp/sharepoint-pnp-cmdlets?view=sharepoint-ps#installation) (PnP) which contains a library of PowerShell commands that allow you to perform complex management actions such as force deleting stubborn items.</span></span> 
- [<span data-ttu-id="e4eed-108">Menghapus PNP File</span><span class="sxs-lookup"><span data-stu-id="e4eed-108">Remove PNP File</span></span>](https://docs.microsoft.com/powershell/module/sharepoint-pnp/remove-pnpfile?view=sharepoint-ps)
- [<span data-ttu-id="e4eed-109">Menghapus PNP Folder</span><span class="sxs-lookup"><span data-stu-id="e4eed-109">Remove PNP Folder</span></span>](https://docs.microsoft.com/powershell/module/sharepoint-pnp/remove-pnpfolder?view=sharepoint-ps)
- [<span data-ttu-id="e4eed-110">Menghapus Item daftar PNP</span><span class="sxs-lookup"><span data-stu-id="e4eed-110">Remove PNP List Item</span></span>](https://docs.microsoft.com/powershell/module/sharepoint-pnp/remove-pnplistitem?view=sharepoint-ps)
- [<span data-ttu-id="e4eed-111">Menghapus daftar PNP</span><span class="sxs-lookup"><span data-stu-id="e4eed-111">Remove PNP List</span></span>](https://docs.microsoft.com/powershell/module/sharepoint-pnp/remove-pnplist?view=sharepoint-ps)
- [<span data-ttu-id="e4eed-112">Menghapus bidang PNP (kolom)</span><span class="sxs-lookup"><span data-stu-id="e4eed-112">Remove PNP Field (Column)</span></span>](https://docs.microsoft.com/powershell/module/sharepoint-pnp/remove-pnpfield?view=sharepoint-ps)