---
title: Menambahkan grup ke situs SharePoint Anda
ms.author: pebaum
author: pebaum
manager: pamgreen
ms.audience: Admin
ms.topic: article
ms.service: o365-administration
ROBOTS: NOINDEX, NOFOLLOW
localization_priority: Normal
ms.collection: Adm_O365
ms.custom:
- "5200004"
- "5766"
ms.assetid: f7d730bf-0d6e-424c-970c-6137c71cb50b
ms.openlocfilehash: 396efbf9772b5398427a4fcc76e104fa95820af6
ms.sourcegitcommit: 86c95d3f0f268e500b3732243ca85a650b2e7b8f
ms.translationtype: MT
ms.contentlocale: id-ID
ms.lasthandoff: 07/22/2021
ms.locfileid: "53532222"
---
# <a name="common-issues-when-creating-a-group-connected-site-in-sharepoint"></a>Masalah umum saat membuat situs yang tersambung dengan grup di SharePoint

1. Jika Anda telah menghapus sebuah grup dan situs tersambungnya serta ingin membuat situs lain dengan URL yang sama, Anda harus menghapus situs sebelumnya secara permanen.

   - Unduh [SPO Management Shell](https://support.office.com/article/introduction-to-the-sharepoint-online-management-shell-c16941c3-19b4-4710-8056-34c034493429)
   - Untuk informasi selengkapnya tentang mulai menggunakan Powershell, lihat [Mulai menggunakan SharePoint Online Management Shell](/powershell/module/sharepoint-online/remove-sposite).
   - Hapus Situs dari Situs Terhapus menggunakan cmdlet Powershell [Remove-SPODeletedSite.](/powershell/module/sharepoint-online/remove-sposite?view=sharepoint-ps) Powershell diperlukan untuk menghapus situs grup secara permanen.

1. Jika Anda membuat situs yang tersambung dengan grup dan menerima peringatan: Grup lain dengan alias yang sama sudah **ada,** periksa grup yang sudah ada dari [grup pusat admin Microsoft 365](https://admin.microsoft.com/AdminPortal/Home#/groups). Untuk mengatasi masalah ini, hapus grup yang sudah ada jika tidak lagi diperlukan atau buat situs dengan alias berbeda yang ditetapkan.

1. Ada cara berbeda untuk membuat dan menggunakan grup modern dengan SharePoint.

   - Anda dapat menyambungkan situs yang sudah ada ke Microsoft 365 grup. Untuk informasi selengkapnya, [Koneksi grup Microsoft 365 pengguna menggunakan SharePoint pengguna .](/sharepoint/dev/transform/modernize-connect-to-office365-group#connect-an-office-365-group-using-the-sharepoint-user-interface)
   - Untuk membuat Microsoft 365 yang tersambung dengan grup, Anda harus membuat [Situs Tim](https://admin.microsoft.com/sharepoint).
