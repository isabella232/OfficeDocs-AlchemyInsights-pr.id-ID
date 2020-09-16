---
title: Menambahkan grup ke situs SharePoint
ms.author: pebaum
author: pebaum
manager: pamgreen
ms.audience: Admin
ms.topic: article
ms.service: o365-administration
ROBOTS: NOINDEX, NOFOLLOW
localization_priority: Normal
ms.collection: Adm_O365
ms.custom: ''
ms.assetid: f7d730bf-0d6e-424c-970c-6137c71cb50b
ms.openlocfilehash: 9bec2f71465e43e1c3cba038e0e68949672ceb8a
ms.sourcegitcommit: c6692ce0fa1358ec3529e59ca0ecdfdea4cdc759
ms.translationtype: MT
ms.contentlocale: id-ID
ms.lasthandoff: 09/15/2020
ms.locfileid: "47771208"
---
# <a name="issues-when-creating-a-group-connected-site-in-sharepoint"></a>Masalah saat membuat situs yang tersambung ke grup di SharePoint

1. Beberapa masalah umum terjadi ketika membuat atau membuat ulang situs yang terhubung dengan grup.
Jika Anda telah menghapus grup dan situs yang terhubung dan ingin membuat situs lain dengan URL yang sama, Anda harus menghapus situs sebelumnya secara permanen.

   - Unduh [shell manajemen SPO](https://support.office.com/article/introduction-to-the-sharepoint-online-management-shell-c16941c3-19b4-4710-8056-34c034493429)
   - Untuk informasi selengkapnya tentang memulai menggunakan PowerShell, lihat [mulai menggunakan SharePoint online Management Shell](https://docs.microsoft.com/powershell/module/sharepoint-online/remove-sposite).
   - Hapus situs dari situs yang dihapus menggunakan cmdlet PowerShell [Hapus-SPODeletedSite](https://docs.microsoft.com/powershell/module/sharepoint-online/remove-sposite?view=sharepoint-ps) . PowerShell diperlukan untuk menghapus situs grup secara permanen.

1. Jika Anda membuat situs yang terhubung ke grup dan menerima peringatan: **grup lain dengan alias yang sama sudah ada**, periksa grup yang sudah ada dari [pusat admin Microsoft 365](https://admin.microsoft.com/AdminPortal/Home#/groups). Untuk mengatasi masalah ini, Hapus grup yang sudah ada jika tidak lagi diperlukan atau buat situs dengan alias berbeda yang ditetapkan.

1. Ada cara berbeda untuk membuat dan menggunakan grup modern dengan SharePoint.

   - Anda dapat menyambungkan situs yang sudah ada ke grup Microsoft 365. Untuk informasi selengkapnya, lihat [menyambungkan grup Microsoft 365 menggunakan antarmuka pengguna SharePoint](https://docs.microsoft.com/sharepoint/dev/transform/modernize-connect-to-office365-group#connect-an-office-365-group-using-the-sharepoint-user-interface).
   - Untuk membuat situs yang tersambung dengan grup Microsoft 365, Anda harus membuat [situs tim](https://admin.microsoft.com/sharepoint).
