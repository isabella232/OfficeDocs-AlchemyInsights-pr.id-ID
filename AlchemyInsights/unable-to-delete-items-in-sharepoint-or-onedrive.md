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
ms.openlocfilehash: 8647b65c52a782ca48ca58bb2700556db528796b
ms.sourcegitcommit: bc7d6f4f3c9f7060d073f5130e1ec856e248d020
ms.translationtype: MT
ms.contentlocale: id-ID
ms.lasthandoff: 06/02/2020
ms.locfileid: "44511979"
---
# <a name="unable-to-delete-items"></a>Tidak dapat menghapus item

Kebijakan retensi dapat menyebabkan ini, Anda perlu menonaktifkan atau mengecualikan masing-masing memegang yang menyebabkan masalah ini. Setelah kebijakan retensi atau tahan dihapus, mungkin diperlukan waktu hingga 24 jam agar perubahan diterapkan. Pastikan bahwa tidak ada pengaturan [kebijakan penyimpanan](https://docs.microsoft.com/microsoft-365/compliance/retention-policies) pada item.

Situs mungkin telah melebihi batas penyimpanan, meningkatkan [kuota situs](https://docs.microsoft.com/powershell/module/sharepoint-online/set-sposite?view=sharepoint-ps) dan menghapus item.

Pastikan item tidak [diperiksa](https://support.office.com/article/check-out-check-in-or-discard-changes-to-files-in-a-library-7e2c12a9-a874-4393-9511-1378a700f6de) ke pengguna lain.

Akhirnya, administrator dapat menggunakan [pola dan praktik SharePoint](https://docs.microsoft.com/powershell/sharepoint/sharepoint-pnp/sharepoint-pnp-cmdlets?view=sharepoint-ps#installation) (PNP) yang berisi pustaka perintah PowerShell yang memungkinkan Anda untuk melakukan tindakan manajemen yang kompleks seperti memaksa menghapus item yang membandel.
- [Hapus berkas PNP](https://docs.microsoft.com/powershell/module/sharepoint-pnp/remove-pnpfile?view=sharepoint-ps)
- [Hapus folder PNP](https://docs.microsoft.com/powershell/module/sharepoint-pnp/remove-pnpfolder?view=sharepoint-ps)
- [Hapus item daftar PNP](https://docs.microsoft.com/powershell/module/sharepoint-pnp/remove-pnplistitem?view=sharepoint-ps)
- [Hapus daftar PNP](https://docs.microsoft.com/powershell/module/sharepoint-pnp/remove-pnplist?view=sharepoint-ps)
- [Hapus kolom PNP (kolom)](https://docs.microsoft.com/powershell/module/sharepoint-pnp/remove-pnpfield?view=sharepoint-ps)