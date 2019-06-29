---
title: Tidak dapat menghapus item dalam SharePoint atau OneDrive
ms.author: kirks
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
ms.openlocfilehash: d25214f26a3168e3e350b5cc31ca870e65d48ad9
ms.sourcegitcommit: 5fb7a4b28859690020efdea630d03e70cc0e6334
ms.translationtype: MT
ms.contentlocale: id-ID
ms.lasthandoff: 06/28/2019
ms.locfileid: "35366536"
---
# <a name="unable-to-delete-items"></a>Tidak dapat menghapus item

Mengalami masalah saat menghapus item?

- Selalu pastikan Anda memiliki [izin sesuai](https://docs.microsoft.com/sharepoint/default-sharepoint-groups) untuk menghapus item atau memiliki usaha [site koleksi administrator](https://docs.microsoft.com/sharepoint/customize-sharepoint-site-permissions#add-change-or-remove-a-site-collection-administrator) yang menghapus item.

- Memastikan bahwa tidak ada setup [kebijakan pengarsipan](https://docs.microsoft.com/office365/securitycompliance/retention-policies) pada item.

- Memastikan item tidak [memeriksa](https://support.office.com/article/check-out-check-in-or-discard-changes-to-files-in-a-library-7e2c12a9-a874-4393-9511-1378a700f6de) untuk pengguna lain.

- Akhirnya, administrator dapat menggunakan [pola SharePoint dan praktek](https://docs.microsoft.com/powershell/sharepoint/sharepoint-pnp/sharepoint-pnp-cmdlets?view=sharepoint-ps#installation) (PnP) yang berisi perpustakaan PowerShell perintah yang memungkinkan Anda untuk melakukan tindakan manajemen yang kompleks seperti memaksa menghapus item keras kepala.
- [Menghapus PNP File](https://docs.microsoft.com/powershell/module/sharepoint-pnp/remove-pnpfile?view=sharepoint-ps)
- [Menghapus PNP Folder](https://docs.microsoft.com/powershell/module/sharepoint-pnp/remove-pnpfolder?view=sharepoint-ps)
- [Menghapus Item daftar PNP](https://docs.microsoft.com/powershell/module/sharepoint-pnp/remove-pnplistitem?view=sharepoint-ps)
- [Menghapus daftar PNP](https://docs.microsoft.com/powershell/module/sharepoint-pnp/remove-pnplist?view=sharepoint-ps)
- [Menghapus bidang PNP (kolom)](https://docs.microsoft.com/powershell/module/sharepoint-pnp/remove-pnpfield?view=sharepoint-ps)