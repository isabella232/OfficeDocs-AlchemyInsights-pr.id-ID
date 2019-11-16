---
title: Pemecahan masalah Akses ditolak pesan ke OneDrive untuk situs bisnis
ms.author: efrene
author: efrene
manager: pamgreen
ms.audience: Admin
ms.topic: article
ROBOTS: NOINDEX, NOFOLLOW
localization_priority: Normal
ms.collection: Adm_O365
ms.assetid: cebb7a4a-33e1-474e-a5d0-dbd02a80b1e9
ms.openlocfilehash: 3c40ad76a8961a3d0b4963483291c2a1364c51d3
ms.sourcegitcommit: b43f77221f47b50c41197a448a9c26c423ce1ad5
ms.translationtype: MT
ms.contentlocale: id-ID
ms.lasthandoff: 11/15/2019
ms.locfileid: "37766714"
---
# <a name="troubleshooting-access-denied-messages-to-onedrive-for-business-sites"></a>Pemecahan masalah Akses ditolak pesan ke OneDrive untuk situs bisnis

Masalah ini paling sering terjadi ketika pengguna dihapus dan dibuat ulang dengan nama prinsip pengguna (UPN) yang sama. Akun baru dibuat dengan menggunakan nilai yang berbeda PUID (paspor unik ID). Saat pengguna berusaha mengakses koleksi situs atau OneDrive mereka, pengguna memiliki PUID salah. Skenario kedua melibatkan sinkronisasi direktori dengan direktori aktif unit organisasi (OU). Jika pengguna telah masuk ke SharePoint, dan kemudian dipindahkan ke OU berbeda dan resynced dengan SharePoint, mereka mungkin mengalami masalah ini.

1. Untuk mengatasi masalah ini, Anda harus memulihkan UPN asli dengan langkah dalam artikel, [memulihkan pengguna di Office 365](https://docs.microsoft.com/office365/admin/add-users/restore-user?view=o365-worldwide).
2. Jika Anda tidak dapat memulihkan pengguna asli, Anda harus menghapus pengguna lama dari situs OneDrive menggunakan langkah ini, [Hapus pengguna dari daftar Info pengguna](). 
3. Setelah ini dilakukan, Anda dapat memverifikasi bahwa pengguna memiliki hak admin untuk situs OneDrive dengan mengikuti langkah untuk [menambahkan admin untuk onedrive pengguna](https://docs.microsoft.com/sharepoint/manage-user-profiles?redirectSourcePath=%252fen-us%252farticle%252fmanage-user-profiles-in-the-sharepoint-admin-center-494bec9c-6654-41f0-920f-f7f937ea9723#add-and-remove-admins-for-a-users-onedrive)

Untuk informasi lebih lanjut tentang tingkat izin, lihat artikel, [memahami tingkat izin di SharePoint](https://docs.microsoft.com/sharepoint/understanding-permission-levels).
