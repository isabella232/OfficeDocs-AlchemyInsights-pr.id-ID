---
title: Pemecahan masalah akses pesan yang ditolak ke OneDrive untuk situs bisnis
ms.author: pebaum
author: pebaum
manager: pamgreen
ms.audience: Admin
ms.topic: article
ms.service: o365-administration
ROBOTS: NOINDEX, NOFOLLOW
localization_priority: Normal
ms.collection: Adm_O365
ms.assetid: cebb7a4a-33e1-474e-a5d0-dbd02a80b1e9
ms.openlocfilehash: 9001cf0b7d9f1f05a2ecedca2c3137dd1b8a1c38
ms.sourcegitcommit: c6692ce0fa1358ec3529e59ca0ecdfdea4cdc759
ms.translationtype: MT
ms.contentlocale: id-ID
ms.lasthandoff: 09/14/2020
ms.locfileid: "47670619"
---
# <a name="troubleshooting-access-denied-messages-to-onedrive-for-business-sites"></a>Pemecahan masalah akses pesan yang ditolak ke OneDrive untuk situs bisnis

Masalah ini paling sering terjadi ketika pengguna dihapus dan dibuat ulang dengan nama prinsip pengguna (UPN) yang sama. Akun baru dibuat menggunakan nilai PUID (ID unik paspor) yang berbeda. Saat pengguna mencoba mengakses kumpulan situs atau OneDrive mereka, pengguna tersebut memiliki PUID yang salah. Skenario kedua melibatkan sinkronisasi direktori dengan unit organisasi direktori aktif (OU). Jika pengguna sudah masuk ke SharePoint, lalu dipindahkan ke OU berbeda dan resynced dengan SharePoint, mereka mungkin mengalami masalah ini.

1. Untuk mengatasi masalah ini, Anda harus memulihkan UPN asli dengan langkah-langkah dalam artikel, [memulihkan pengguna di Microsoft 365](https://docs.microsoft.com/microsoft-365/admin/add-users/restore-user).
2. Jika Anda tidak bisa memulihkan pengguna asli, Anda harus menghapus pengguna lama dari situs OneDrive menggunakan langkah-langkah ini, [menghapus pengguna dari daftar Info pengguna](). 
3. Setelah ini selesai, Anda dapat memverifikasi bahwa pengguna memiliki hak admin ke situs OneDrive dengan mengikuti langkah-langkah untuk [menambahkan admin untuk onedrive pengguna](https://docs.microsoft.com/sharepoint/manage-user-profiles)

Untuk informasi selengkapnya tentang tingkat izin, lihat artikel, [memahami tingkat izin di SharePoint](https://docs.microsoft.com/sharepoint/understanding-permission-levels).
