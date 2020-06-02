---
title: Pemecahan masalah Akses ditolak pesan ke OneDrive untuk situs bisnis
ms.author: pebaum
author: pebaum
manager: pamgreen
ms.audience: Admin
ms.topic: article
ROBOTS: NOINDEX, NOFOLLOW
localization_priority: Normal
ms.collection: Adm_O365
ms.assetid: cebb7a4a-33e1-474e-a5d0-dbd02a80b1e9
ms.openlocfilehash: 95bd46e8b7a6006f3735612d9a5602fb2b2a283b
ms.sourcegitcommit: bc7d6f4f3c9f7060d073f5130e1ec856e248d020
ms.translationtype: MT
ms.contentlocale: id-ID
ms.lasthandoff: 06/02/2020
ms.locfileid: "44511187"
---
# <a name="troubleshooting-access-denied-messages-to-onedrive-for-business-sites"></a>Pemecahan masalah Akses ditolak pesan ke OneDrive untuk situs bisnis

Masalah ini paling sering terjadi ketika pengguna dihapus dan dibuat ulang dengan nama prinsip pengguna (UPN) yang sama. Akun baru dibuat dengan menggunakan nilai yang berbeda PUID (paspor unik ID). Saat pengguna berusaha mengakses koleksi situs atau OneDrive mereka, pengguna memiliki PUID salah. Skenario kedua melibatkan sinkronisasi direktori dengan direktori aktif unit organisasi (OU). Jika pengguna telah masuk ke SharePoint, dan kemudian dipindahkan ke OU berbeda dan resynced dengan SharePoint, mereka mungkin mengalami masalah ini.

1. Untuk mengatasi masalah ini, Anda harus memulihkan UPN asli dengan langkah dalam artikel, [memulihkan pengguna di Microsoft 365](https://docs.microsoft.com/microsoft-365/admin/add-users/restore-user).
2. Jika Anda tidak dapat memulihkan pengguna asli, Anda harus menghapus pengguna lama dari situs OneDrive menggunakan langkah ini, [Hapus pengguna dari daftar Info pengguna](). 
3. Setelah ini dilakukan, Anda dapat memverifikasi bahwa pengguna memiliki hak admin untuk situs OneDrive dengan mengikuti langkah untuk [menambahkan admin untuk onedrive pengguna](https://docs.microsoft.com/sharepoint/manage-user-profiles)

Untuk informasi lebih lanjut tentang tingkat izin, lihat artikel, [memahami tingkat izin di SharePoint](https://docs.microsoft.com/sharepoint/understanding-permission-levels).
