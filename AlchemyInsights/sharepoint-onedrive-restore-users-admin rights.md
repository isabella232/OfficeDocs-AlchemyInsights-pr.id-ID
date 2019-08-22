---
title: Mengatasi masalah Akses ditolak pesan untuk OneDrive untuk situs bisnis
ms.author: efrene
author: efrene
manager: pamgreen
ms.date: 11/14/2018
ms.audience: Admin
ms.topic: article
ROBOTS: NOINDEX, NOFOLLOW
localization_priority: Normal
ms.collection: Adm_O365
ms.assetid: cebb7a4a-33e1-474e-a5d0-dbd02a80b1e9
ms.openlocfilehash: 39f9b9b1ca22f6e5959e2b431fb373b0002c0a92
ms.sourcegitcommit: 1d98db8acb9959aba3b5e308a567ade6b62da56c
ms.translationtype: MT
ms.contentlocale: id-ID
ms.lasthandoff: 08/22/2019
ms.locfileid: "36507814"
---
# <a name="troubleshooting-access-denied-messages-to-onedrive-for-business-sites"></a>Mengatasi masalah Akses ditolak pesan untuk OneDrive untuk situs bisnis

Masalah ini paling sering terjadi ketika pengguna dihapus dan kembali dibuat dengan sama pengguna (UPN nama dasar). Account yang baru dibuat dengan menggunakan PUID (paspor unik ID) nilai yang berbeda. Ketika pengguna mencoba untuk mengakses situs koleksi atau OneDrive mereka, pengguna memiliki PUID salah. Skenario yang kedua melibatkan sinkronisasi direktori dengan unit organisasi Active Directory (OU). Jika pengguna telah sudah masuk ke SharePoint, dan kemudian pindah ke OU berbeda dan resynced dengan SharePoint, mereka mungkin mengalami masalah ini.

1. Untuk mengatasi masalah ini, Anda harus mengembalikan UPN asli dengan langkah-langkah dalam artikel,[mengembalikan pengguna di Office 365](https://docs.microsoft.com/office365/admin/add-users/restore-user?view=o365-worldwide).
2. Jika Anda tidak dapat mengembalikan pengguna awal Anda harus menghapus pengguna lama dari situs OneDrive menggunakan langkah-langkah ini, [menghapus pengguna dari daftar info pengguna](). 
3. Setelah ini selesai, Anda dapat memverifikasi pengguna memiliki hak admin situs OneDrive dengan mengikuti langkah-langkah untuk [menambahkan admin's untuk pengguna OneDrive](https://docs.microsoft.com/sharepoint/manage-user-profiles?redirectSourcePath=%252fen-us%252farticle%252fmanage-user-profiles-in-the-sharepoint-admin-center-494bec9c-6654-41f0-920f-f7f937ea9723#add-and-remove-admins-for-a-users-onedrive)

Untuk informasi lebih lanjut tentang tingkat izin, lihat artikel, [pemahaman tingkat izin di SharePoint](https://docs.microsoft.com/sharepoint/understanding-permission-levels).
