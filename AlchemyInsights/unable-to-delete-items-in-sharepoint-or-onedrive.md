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
ms.openlocfilehash: 3601c5eff121e10b6bddace6f7228204a01080a636e24f3a56373fe8d469c799
ms.sourcegitcommit: b5f7da89a650d2915dc652449623c78be6247175
ms.translationtype: MT
ms.contentlocale: id-ID
ms.lasthandoff: 08/05/2021
ms.locfileid: "54038520"
---
# <a name="unable-to-delete-items"></a>Tidak dapat menghapus item

- Kebijakan penyimpanan bisa menyebabkan hal ini, Anda harus menonaktifkan atau tidak menyertakan masing-masing penyimpanan yang menyebabkan masalah ini. Setelah kebijakan atau penyimpanan dihapus, mungkin butuh waktu hingga 24 jam agar perubahan bisa diterapkan. Pastikan tidak ada penyetelan [kebijakan penyimpanan](https://docs.microsoft.com/microsoft-365/compliance/retention-policies) pada item.

- Situs tersebut mungkin telah melebihi batas penyimpanan, menambah [kuota situs,](https://docs.microsoft.com/powershell/module/sharepoint-online/set-sposite?view=sharepoint-ps) dan menghapus item.

- Pastikan item tidak [di-check out](https://support.office.com/article/check-out-check-in-or-discard-changes-to-files-in-a-library-7e2c12a9-a874-4393-9511-1378a700f6de) ke pengguna lain.

- Terakhir, administrator bisa menggunakan SharePoint Pola dan Praktik (PnP, Patterns [and Practices)](https://docs.microsoft.com/powershell/sharepoint/sharepoint-pnp/sharepoint-pnp-cmdlets?view=sharepoint-ps#installation) yang berisi pustaka perintah PowerShell yang memungkinkan Anda untuk melakukan tindakan manajemen kompleks seperti penghapusan paksa item stub items.
- [Menghapus File PNP](https://docs.microsoft.com/powershell/module/sharepoint-pnp/remove-pnpfile?view=sharepoint-ps)
- [Hapus Folder PNP](https://docs.microsoft.com/powershell/module/sharepoint-pnp/remove-pnpfolder?view=sharepoint-ps)
- [Hapus Item Daftar PNP](https://docs.microsoft.com/powershell/module/sharepoint-pnp/remove-pnplistitem?view=sharepoint-ps)
- [Menghapus Daftar PNP](https://docs.microsoft.com/powershell/module/sharepoint-pnp/remove-pnplist?view=sharepoint-ps)
- [Menghapus Bidang PNP (Kolom)](https://docs.microsoft.com/powershell/module/sharepoint-pnp/remove-pnpfield?view=sharepoint-ps)