---
title: Menambahkan grup ke situs SharePoint
ms.author: pebaum
author: pebaum
manager: pamgreen
ms.audience: Admin
ms.topic: article
ROBOTS: NOINDEX, NOFOLLOW
localization_priority: Normal
ms.collection: Adm_O365
ms.custom: ''
ms.assetid: f7d730bf-0d6e-424c-970c-6137c71cb50b
ms.openlocfilehash: 8ef33cbd44b01deaf0e45813d019f7696ef5def0
ms.sourcegitcommit: 286000b588adef1bbbb28337a9d9e087ec783fa2
ms.translationtype: MT
ms.contentlocale: id-ID
ms.lasthandoff: 04/27/2020
ms.locfileid: "43912969"
---
# <a name="issues-when-creating-a-group-connected-site-in-sharepoint"></a>Masalah saat membuat grup terhubung situs di SharePoint

1. Beberapa masalah umum yang dihadapi saat membuat atau membuat ulang grup situs yang terhubung.
Jika Anda telah menghapus grup dan situs yang terhubung dan ingin membuat situs lain dengan URL yang sama, Anda harus menghapus situs sebelumnya secara permanen.

   - Unduh [SPO Management Shell](https://support.office.com/article/introduction-to-the-sharepoint-online-management-shell-c16941c3-19b4-4710-8056-34c034493429)
   - Untuk informasi lebih lanjut tentang cara memulai dengan PowerShell, lihat memulai [SharePoint online Management Shell](https://docs.microsoft.com/powershell/module/sharepoint-online/remove-sposite).
   - Menghapus situs dari situs dihapus menggunakan cmdlet PowerShell [Hapus-SPODeletedSite](https://docs.microsoft.com/powershell/module/sharepoint-online/remove-sposite?view=sharepoint-ps) . PowerShell diperlukan untuk menghapus secara permanen situs grup.

1. Jika Anda membuat grup situs yang terhubung dan menerima peringatan: **grup lain dengan alias yang sama sudah ada**, periksa grup yang ada dari [pusat admin Microsoft 365](https://admin.microsoft.com/AdminPortal/Home#/groups). Untuk mengatasi masalah ini, Hapus grup yang ada jika tidak lagi diperlukan atau membuat situs dengan alias lain yang ditetapkan.

1. Ada berbagai cara untuk membuat dan menggunakan grup modern dengan SharePoint.

   - Anda dapat menghubungkan situs yang ada ke grup Microsoft 365. Untuk informasi lebih lanjut, lihat [menyambungkan grup Microsoft 365 menggunakan antarmuka pengguna SharePoint](https://docs.microsoft.com/sharepoint/dev/transform/modernize-connect-to-office365-group#connect-an-office-365-group-using-the-sharepoint-user-interface).
   - Untuk membuat situs Microsoft 365 grup yang terhubung, Anda harus membuat [situs tim](https://admin.microsoft.com/sharepoint).
