---
title: Beberapa pengguna tidak melihat Add-in di Outlook
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
ms.openlocfilehash: 18d3fa535a88af18d8c4b02a5371d0a81c8d28c0
ms.sourcegitcommit: a05276bd623466ad211e1f8d9f0c616672dd3640
ms.translationtype: MT
ms.contentlocale: id-ID
ms.lasthandoff: 07/16/2020
ms.locfileid: "45197977"
---
# <a name="multiple-users-not-seeing-add-ins-in-outlook"></a>Beberapa pengguna tidak melihat Add-in di Outlook

Jika Anda menguji Add-in Outlook dan tidak muncul, sebagai langkah pemecahan masalah pertama, gunakan cmdlet **Get-OrganizationConfig** PowerShell untuk meminta _Appsforofficeenabled_ parameter. Jika permintaan mengembalikan nilai **false**, tetapkan parameter ini ke **True** dengan menggunakan cmdlet **set-OrganizationConfig** , sehingga Add-in muncul seperti yang diharapkan.

Kami tidak menyarankan bahwa _Appsforofficeenabled_ parameter diatur ke **false**. Nilai **salah** menimpa semua pengaturan peran administratif dan pengguna di atas dan mencegah aplikasi baru yang diaktifkan oleh pengguna di organisasi.

Untuk informasi selengkapnya, lihat [menentukan administrator dan pengguna yang dapat menginstal dan mengelola add-in untuk Outlook](https://docs.microsoft.com/exchange/clients-and-mobile-in-exchange-online/add-ins-for-outlook/specify-who-can-install-and-manage-add-ins#user-roles).