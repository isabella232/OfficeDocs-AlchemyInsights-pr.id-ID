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
ms.openlocfilehash: 352bad1b8fe219f95a37c9ac268c6c4dd8801dfc
ms.sourcegitcommit: 6d341637dbb14e90726a1ce1d68f077ace9bb765
ms.translationtype: MT
ms.contentlocale: id-ID
ms.lasthandoff: 06/04/2019
ms.locfileid: "34719485"
---
# <a name="create-group-connected-site-in-sharepoint-online"></a>Membuat situs terhubung group di SharePoint Online

<p><strong>Ada beberapa masalah umum yang dihadapi ketika membuat atau menciptakan kembali kelompok yang terhubung situs.&nbsp;</strong></p>  <p>1.Jika Anda telah menghapus grup dan situs yang terhubung dan ingin membuat situs lain dengan URL yang sama, Anda akan perlu untuk secara permanen menghapus situs sebelumnya.</p>  <ul>  <li>Download <a title="SPO Management Shell" href="https://support.office.com/en-ie/article/introduction-to-the-sharepoint-online-management-shell-c16941c3-19b4-4710-8056-34c034493429">SPO Management Shell</a> - untuk info lebih lanjut tentang memulai dengan powershell, lihat <a title="memulai dengan SharePoint Online Management Shell" href="https://docs.microsoft.com/en-us/powershell/module/sharepoint-online/remove-sposite?view=sharepoint-ps">Memulai dengan SharePoint Online Management Shell</a>. <br /><br /></li>  <li>Menghapus situs tersebut dari situs dihapus menggunakan <a title="Hapus-SPODeletedSite" href="https://docs.microsoft.com/en-us/powershell/module/sharepoint-online/remove-sposite?view=sharepoint-ps">Hapus-SPODeletedSite</a> powershell cmdlet.</li>  </ul>  <p>Jika Anda membuat situs terhubung group dan menerima peringatan <strong>'kelompok yang lain dengan nama alias yang sama sudah ada'</strong>, periksa grup dari <a title="Office 365 dari pusat Admin" href="https://admin.microsoft.com/Adminportal/Home?source=applauncher#/groups">Kantor 365 dari pusat Admin</a>. Untuk menyelesaikan masalah, menghapus grup yang ada jika tidak lagi diperlukan atau membuat situs dengan alias lain ditetapkan.&nbsp;</p>  <p><strong>Ada berbagai cara untuk membuat dan menggunakan grup modern dengan SharePoint.&nbsp;</strong></p>  <ol>  <li>Anda dapat menghubungkan situs yang ada untuk grup Office 365. Untuk info lebih lanjut, lihat <a title="menghubungkan grup Office 365 menggunakan SharePoint pengguna ineterface" href="https://docs.microsoft.com/en-us/sharepoint/dev/transform/modernize-connect-to-office365-group#connect-an-office-365-group-using-the-sharepoint-user-interface">Menghubungkan sebuah kelompok Office 365 menggunakan SharePoint pengguna ineterface</a>.</li>  <li>Untuk membuat situs terhubung group Office 365, Anda harus membuat situs tim. Untuk info lebih lanjut, lihat <a title="membuat situs tim SharePoint" href="https://support.office.com/en-us/article/create-a-team-site-in-sharepoint-ef10c1e7-15f3-42a3-98aa-b5972711777d">Membuat situs tim di SharePoint.</a></li>  </ol>

