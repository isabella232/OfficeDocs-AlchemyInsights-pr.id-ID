---
title: Tidak dapat menghapus item dalam SharePoint atau OneDrive
ms.author: kirks
author: Techwriter40
ms.audience: ITPro
ms.topic: article
ROBOTS: NOINDEX, NOFOLLOW
localization_priority: Normal
ms.assetid: ''
ms.openlocfilehash: 21d7b928fade48a6729c120e6ea33b16dafe799e
ms.sourcegitcommit: 22ce2315c8cf643137ab3420cdc1cda41433d44a
ms.translationtype: MT
ms.contentlocale: id-ID
ms.lasthandoff: 05/14/2019
ms.locfileid: "34057728"
---
# <a name="unable-to-delete-items"></a>Tidak dapat menghapus item

Mengalami masalah saat menghapus item?

- Selalu pastikan Anda memiliki [izin sesuai](https://docs.microsoft.com/en-us/sharepoint/default-sharepoint-groups) untuk menghapus item atau memiliki usaha [site koleksi administrator](https://docs.microsoft.com/en-us/sharepoint/customize-sharepoint-site-permissions#add-change-or-remove-a-site-collection-administrator) yang menghapus item.

- Memastikan bahwa tidak ada setup [kebijakan pengarsipan](https://docs.microsoft.com/en-us/office365/securitycompliance/retention-policies) pada item.

- Memastikan item tidak [memeriksa](https://support.office.com/en-us/article/check-out-check-in-or-discard-changes-to-files-in-a-library-7e2c12a9-a874-4393-9511-1378a700f6de) untuk pengguna lain.

- Akhirnya, administrator dapat menggunakan [pola SharePoint dan praktek](https://docs.microsoft.com/en-us/powershell/sharepoint/sharepoint-pnp/sharepoint-pnp-cmdlets?view=sharepoint-ps#installation) (PnP) yang berisi perpustakaan PowerShell perintah yang memungkinkan Anda untuk melakukan tindakan manajemen yang kompleks seperti memaksa menghapus item keras kepala. 
- [Menghapus PNP File](https://docs.microsoft.com/en-us/powershell/module/sharepoint-pnp/remove-pnpfile?view=sharepoint-ps)
- [Menghapus PNP Folder](https://docs.microsoft.com/en-us/powershell/module/sharepoint-pnp/remove-pnpfolder?view=sharepoint-ps)
- [Menghapus Item daftar PNP](https://docs.microsoft.com/en-us/powershell/module/sharepoint-pnp/remove-pnplistitem?view=sharepoint-ps)
- [Menghapus daftar PNP](https://docs.microsoft.com/en-us/powershell/module/sharepoint-pnp/remove-pnplist?view=sharepoint-ps)
- [Menghapus bidang PNP (kolom)](https://docs.microsoft.com/en-us/powershell/module/sharepoint-pnp/remove-pnpfield?view=sharepoint-ps)