---
title: Pemecahan masalah pesan access ditolak OneDrive for Business situs
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
ms.openlocfilehash: fc4a2bd7dcc74f5f05e8b709e4bc3eac6ed445d6e2ea9ede698abbc8667723ce
ms.sourcegitcommit: b5f7da89a650d2915dc652449623c78be6247175
ms.translationtype: MT
ms.contentlocale: id-ID
ms.lasthandoff: 08/05/2021
ms.locfileid: "53957796"
---
# <a name="troubleshooting-access-denied-messages-to-onedrive-for-business-sites"></a>Pemecahan masalah pesan access ditolak OneDrive for Business situs

Masalah ini paling sering terjadi ketika pengguna dihapus dan dibuat ulang dengan nama prinsipal pengguna (UPN) yang sama. Akun baru dibuat dengan menggunakan nilai PUID (ID Unik Paspor) yang berbeda. Saat pengguna berusaha mengakses kumpulan situs atau situs OneDrive, pengguna memiliki PUID yang tidak benar. Skenario kedua melibatkan sinkronisasi direktori dengan Unit organisasi Direktori Aktif (OU). Jika pengguna sudah masuk ke SharePoint lalu dipindahkan ke OU lain dan disinkronkan kembali dengan SharePoint, mereka mungkin mengalami masalah ini.

1. Untuk mengatasi masalah ini Anda harus memulihkan UPN asli dengan langkah-langkah dalam artikel, [Memulihkan pengguna di Microsoft 365](https://docs.microsoft.com/microsoft-365/admin/add-users/restore-user).
2. If you cannot restore the original user you should remove the old user from the OneDrive site using these steps, [Remove a user from the user info list](). 
3. Setelah ini selesai, Anda bisa memverifikasi bahwa pengguna mempunyai hak admin ke situs OneDrive dengan mengikuti langkah-langkah untuk Menambahkan [admin untuk](https://docs.microsoft.com/sharepoint/manage-user-profiles) akun OneDrive

Untuk informasi selengkapnya tentang tingkat izin, lihat artikel Memahami [tingkat izin dalam SharePoint](https://docs.microsoft.com/sharepoint/understanding-permission-levels).
