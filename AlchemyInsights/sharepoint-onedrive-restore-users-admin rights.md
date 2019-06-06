---
title: Memberikan akses kepada pengguna ke SharePoint dan OneDrive
ms.author: kirks
author: Techwriter40
manager: pamgreen
ms.date: 11/14/2018
ms.audience: Admin
ms.topic: article
ROBOTS: NOINDEX, NOFOLLOW
localization_priority: Normal
ms.collection: Adm_O365
ms.custom: ''
ms.assetid: cebb7a4a-33e1-474e-a5d0-dbd02a80b1e9
ms.openlocfilehash: 9326932e93970edc96396a141c9b36b14e7b4d4d
ms.sourcegitcommit: 241e21b6da226563bf70bdb1f5bad3d91c38cd2c
ms.translationtype: MT
ms.contentlocale: id-ID
ms.lasthandoff: 06/05/2019
ms.locfileid: "34736651"
---
# <a name="give-users-access-to-sharepoint-and-onedrive"></a>Memberikan akses kepada pengguna ke SharePoint dan OneDrive

Masalah ini paling sering terjadi ketika pengguna dihapus dan kembali dibuat dengan sama pengguna (UPN nama dasar). Account yang baru dibuat dengan menggunakan PUID (paspor unik ID) nilai yang berbeda. Ketika pengguna mencoba untuk mengakses situs koleksi atau OneDrive mereka, pengguna memiliki PUID salah. Skenario yang kedua melibatkan sinkronisasi direktori dengan unit organisasi Active Directory (OU). Jika pengguna telah sudah masuk ke SharePoint, dan kemudian pindah ke OU berbeda dan resynced dengan SharePoint, mereka mungkin mengalami masalah ini.

Untuk mengatasi masalah ini, Anda harus mengembalikan UPN asli dengan langkah-langkah dalam artikel,[mengembalikan pengguna di Office 365](https://docs.microsoft.com/en-us/office365/admin/add-users/restore-user?view=o365-worldwide).

Setelah ini selesai, Anda dapat memverifikasi pengguna memiliki hak admin situs OneDrive dengan mengikuti langkah-langkah untuk [menambahkan admin's untuk pengguna OneDrive](https://docs.microsoft.com/en-us/sharepoint/manage-user-profiles?redirectSourcePath=%252fen-us%252farticle%252fmanage-user-profiles-in-the-sharepoint-admin-center-494bec9c-6654-41f0-920f-f7f937ea9723#add-and-remove-admins-for-a-users-onedrive)

Untuk informasi lebih lanjut tentang tingkat izin, lihat artikel, [pemahaman tingkat izin di SharePoint](https://docs.microsoft.com/en-us/sharepoint/understanding-permission-levels).
