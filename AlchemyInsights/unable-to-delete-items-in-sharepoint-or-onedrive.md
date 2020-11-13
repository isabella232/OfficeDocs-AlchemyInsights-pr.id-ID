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
# <a name="unable-to-delete-items"></a>Tidak dapat menghapus item

- Kebijakan penyimpanan bisa menyebabkan hal ini, Anda perlu menonaktifkan atau mengecualikan penangguhan masing-masing yang menyebabkan masalah ini. Setelah kebijakan atau penangguhan penyimpanan dihapus, mungkin perlu waktu hingga 24 jam agar perubahan diterapkan. Pastikan bahwa tidak ada penyetelan [kebijakan penyimpanan](https://docs.microsoft.com/microsoft-365/compliance/retention-policies) pada item.

- Situs mungkin telah melebihi batas penyimpanan, menambah [kuota situs](https://docs.microsoft.com/powershell/module/sharepoint-online/set-sposite?view=sharepoint-ps) dan menghapus item.

- Pastikan item tidak [dicentang](https://support.office.com/article/check-out-check-in-or-discard-changes-to-files-in-a-library-7e2c12a9-a874-4393-9511-1378a700f6de) ke pengguna lain.

- Akhirnya, administrator dapat menggunakan [SharePoint Patterns and Practices](https://docs.microsoft.com/powershell/sharepoint/sharepoint-pnp/sharepoint-pnp-cmdlets?view=sharepoint-ps#installation) (PNP) yang berisi pustaka perintah PowerShell yang memungkinkan Anda melakukan tindakan manajemen yang kompleks seperti memaksa penghapusan item yang membandel.
- [Hapus file PNP](https://docs.microsoft.com/powershell/module/sharepoint-pnp/remove-pnpfile?view=sharepoint-ps)
- [Hapus folder PNP](https://docs.microsoft.com/powershell/module/sharepoint-pnp/remove-pnpfolder?view=sharepoint-ps)
- [Hapus item daftar PNP](https://docs.microsoft.com/powershell/module/sharepoint-pnp/remove-pnplistitem?view=sharepoint-ps)
- [Hapus daftar PNP](https://docs.microsoft.com/powershell/module/sharepoint-pnp/remove-pnplist?view=sharepoint-ps)
- [Menghapus bidang PNP (kolom)](https://docs.microsoft.com/powershell/module/sharepoint-pnp/remove-pnpfield?view=sharepoint-ps)