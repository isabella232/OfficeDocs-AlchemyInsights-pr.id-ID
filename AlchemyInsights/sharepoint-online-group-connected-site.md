---
title: Menambahkan grup ke situs SharePoint
ms.author: pebaum
author: Techwriter40
manager: pamgreen
ms.audience: Admin
ms.topic: article
ROBOTS: NOINDEX, NOFOLLOW
localization_priority: Normal
ms.collection: Adm_O365
ms.custom: ''
ms.assetid: f7d730bf-0d6e-424c-970c-6137c71cb50b
ms.openlocfilehash: 423db4e5bbb85e75aee3548d5b6b46a64ebc6fa0
ms.sourcegitcommit: a65d196d00adb70045af5caca9828fe44b951f61
ms.translationtype: MT
ms.contentlocale: id-ID
ms.lasthandoff: 09/04/2019
ms.locfileid: "36750523"
---
# <a name="issues-when-creating-or-group-connected-sites-in-sharepoint-online"></a>Masalah saat membuat atau grup terhubung situs di SharePoint online

Ada beberapa masalah umum yang dihadapi saat membuat atau membuat ulang grup situs yang terhubung.

 Jika Anda telah menghapus grup dan situs yang terhubung dan ingin membuat situs lain dengan URL yang sama, Anda harus menghapus situs sebelumnya secara permanen.

Unduh [SPO Management Shell](https://support.office.com/article/introduction-to-the-sharepoint-online-management-shell-c16941c3-19b4-4710-8056-34c034493429)

 Untuk informasi lebih lanjut tentang memulai dengan PowerShell, lihat memulai [SharePoint online Management Shell](https://docs.microsoft.com/powershell/module/sharepoint-online/remove-sposite?view=sharepoint-ps)

Menghapus situs dari situs dihapus menggunakan cmdlet PowerShell [Hapus-SPODeletedSite](https://docs.microsoft.com/powershell/module/sharepoint-online/remove-sposite?view=sharepoint-ps) .

Jika Anda membuat grup situs yang terhubung dan menerima peringatan grup lain dengan alias yang sama sudah ada, periksa grup yang ada dari [Office 365 dari Pusat admin](https://admin.microsoft.com/Adminportal/Home?source=applauncher#/groups). Untuk mengatasi masalah ini, Hapus grup yang ada jika tidak lagi diperlukan atau membuat situs dengan alias lain yang ditetapkan.

Ada berbagai cara untuk membuat dan menggunakan grup modern dengan SharePoint.

Anda dapat menghubungkan situs yang ada ke grup 365 Office. Untuk informasi lebih lanjut, lihat [menyambungkan grup 365 Office menggunakan pengguna SharePoint ineterface](https://docs.microsoft.com/sharepoint/dev/transform/modernize-connect-to-office365-group#connect-an-office-365-group-using-the-sharepoint-user-interface).

Untuk membuat situs Office 365 grup yang terhubung, Anda harus membuat situs tim. Untuk informasi lebih lanjut, lihat [membuat tim situs di SharePoint](https://support.office.com/article/create-a-team-site-in-sharepoint-ef10c1e7-15f3-42a3-98aa-b5972711777d).

