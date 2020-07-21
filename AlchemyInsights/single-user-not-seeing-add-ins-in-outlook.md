---
title: Satu pengguna tidak melihat Add-in di Outlook
ms.author: pebaum
author: pebaum
manager: scotv
ms.date: 07/16/2020
ms.audience: Admin
ms.topic: article
ROBOTS: NOINDEX, NOFOLLOW
localization_priority: Priority
ms.collection: Adm_O365
ms.custom: ''
ms.openlocfilehash: 1f547c3f593b3256bd44f518aacbc36ed1c4c848
ms.sourcegitcommit: a05276bd623466ad211e1f8d9f0c616672dd3640
ms.translationtype: MT
ms.contentlocale: id-ID
ms.lasthandoff: 07/16/2020
ms.locfileid: "45197962"
---
# <a name="single-user-not-seeing-add-ins-in-outlook"></a>Satu pengguna tidak melihat Add-in di Outlook

Pengguna mungkin menjadi bagian dari peran yang tidak memiliki AppsForOfficeEnabled parameter yang benar. Jalankan cmdlet ini untuk mengetahui apakah peran yang benar terkait dengan pengguna:

Get-ManagementRoleAssignment-RoleAssignee user@domain.com-Delegating $false | Format-tabel-Auto peran, RoleAssigneeName, RoleAssigneeType

Untuk informasi lebih lanjut, lihat [menentukan administrator dan pengguna yang dapat menginstal dan mengelola add-in untuk Outlook](https://docs.microsoft.com/exchange/clients-and-mobile-in-exchange-online/add-ins-for-outlook/specify-who-can-install-and-manage-add-ins).
