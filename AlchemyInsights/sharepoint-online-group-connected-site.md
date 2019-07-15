---
title: Menambahkan grup ke situs SharePoint
ms.author: kirks
author: Techwriter40
manager: pamgreen
ms.audience: Admin
ms.topic: article
ROBOTS: NOINDEX, NOFOLLOW
localization_priority: Normal
ms.collection: Adm_O365
ms.custom: ''
ms.assetid: f7d730bf-0d6e-424c-970c-6137c71cb50b
ms.openlocfilehash: f0126f7f753275e9bbf8c3a09a6af5faf9a27862
ms.sourcegitcommit: 4b7e478ce700c0b781efec3857ac4dce5bdf00c6
ms.translationtype: MT
ms.contentlocale: id-ID
ms.lasthandoff: 06/07/2019
ms.locfileid: "34758734"
---
# <a name="create-group-connected-site-in-sharepoint-online"></a>Membuat situs terhubung group di SharePoint Online

Ada beberapa masalah umum yang dihadapi ketika membuat atau menciptakan kembali kelompok yang terhubung situs.

 Jika Anda telah menghapus grup dan situs yang terhubung dan ingin membuat situs lain dengan URL yang sama, Anda akan perlu untuk secara permanen menghapus situs sebelumnya.

Download [SPO Management Shell](https://support.office.com/article/introduction-to-the-sharepoint-online-management-shell-c16941c3-19b4-4710-8056-34c034493429)

 Untuk info lebih lanjut tentang memulai dengan powershell, lihat [persiapan dengan SharePoint Online Management Shell](https://docs.microsoft.com/powershell/module/sharepoint-online/remove-sposite?view=sharepoint-ps)

Menghapus situs dari situs dihapus menggunakan cmdlet powershell [Hapus-SPODeletedSite](https://docs.microsoft.com/powershell/module/sharepoint-online/remove-sposite?view=sharepoint-ps) .

Jika Anda membuat situs terhubung group dan menerima peringatan kelompok lain dengan nama alias yang sama sudah ada, periksa grup dari [Office 365 dari Admin Center](https://admin.microsoft.com/Adminportal/Home?source=applauncher#/groups). Untuk menyelesaikan masalah, menghapus grup yang ada jika tidak lagi diperlukan atau membuat situs dengan alias lain ditetapkan.

Ada berbagai cara untuk membuat dan menggunakan grup modern dengan SharePoint.

Anda dapat menghubungkan situs yang ada untuk grup Office 365. Untuk info lebih lanjut, lihat [Connect grup Office 365 menggunakan SharePoint pengguna ineterface](https://docs.microsoft.com/sharepoint/dev/transform/modernize-connect-to-office365-group#connect-an-office-365-group-using-the-sharepoint-user-interface).

Untuk membuat situs terhubung group Office 365, Anda harus membuat situs tim. Untuk info lebih lanjut, lihat [membuat situs tim di SharePoint](https://support.office.com/article/create-a-team-site-in-sharepoint-ef10c1e7-15f3-42a3-98aa-b5972711777d).
