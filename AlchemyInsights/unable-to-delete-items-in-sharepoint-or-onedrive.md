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
ms.sourcegitcommit: a65d196d00adb70045af5caca9828fe44b951f61
ms.translationtype: MT
ms.contentlocale: id-ID
ms.lasthandoff: 09/04/2019
ms.locfileid: "36748564"
---
# <a name="unable-to-delete-items"></a>Tidak dapat menghapus item

Setelah masalah menghapus item SharePoint?

- Selalu pastikan Anda memiliki izin yang [sesuai](https://docs.microsoft.com/sharepoint/default-sharepoint-groups) untuk menghapus item atau meminta [administrator kumpulan situs](https://docs.microsoft.com/sharepoint/customize-sharepoint-site-permissions#add-change-or-remove-a-site-collection-administrator) mencoba menghapus item.

- Pastikan bahwa tidak ada pengaturan [kebijakan penyimpanan](https://docs.microsoft.com/office365/securitycompliance/retention-policies) pada item.

- Pastikan item tidak [diperiksa](https://support.office.com/article/check-out-check-in-or-discard-changes-to-files-in-a-library-7e2c12a9-a874-4393-9511-1378a700f6de) ke pengguna lain.

- Akhirnya, administrator dapat menggunakan [pola dan praktik SharePoint](https://docs.microsoft.com/powershell/sharepoint/sharepoint-pnp/sharepoint-pnp-cmdlets?view=sharepoint-ps#installation) (PNP) yang berisi pustaka perintah PowerShell yang memungkinkan Anda untuk melakukan tindakan manajemen yang kompleks seperti memaksa menghapus item yang membandel.
- [Hapus berkas PNP](https://docs.microsoft.com/powershell/module/sharepoint-pnp/remove-pnpfile?view=sharepoint-ps)
- [Hapus folder PNP](https://docs.microsoft.com/powershell/module/sharepoint-pnp/remove-pnpfolder?view=sharepoint-ps)
- [Hapus item daftar PNP](https://docs.microsoft.com/powershell/module/sharepoint-pnp/remove-pnplistitem?view=sharepoint-ps)
- [Hapus daftar PNP](https://docs.microsoft.com/powershell/module/sharepoint-pnp/remove-pnplist?view=sharepoint-ps)
- [Hapus kolom PNP (kolom)](https://docs.microsoft.com/powershell/module/sharepoint-pnp/remove-pnpfield?view=sharepoint-ps)