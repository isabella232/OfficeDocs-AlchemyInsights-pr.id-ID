---
title: Memecahkan masalah pesan Access Denied
ms.author: pebaum
author: pebaum
ms.date: 04/21/2020
ms.audience: ITPro
ms.topic: article
ms.service: o365-administration
ROBOTS: NOINDEX, NOFOLLOW
localization_priority: Normal
ms.assetid: d678b57a-53ad-4414-9423-d8726a0c532f
ms.openlocfilehash: 9acde72f82a27c9f2faa2cf4d0417374aa5a294234da96080dc0498d07639248
ms.sourcegitcommit: b5f7da89a650d2915dc652449623c78be6247175
ms.translationtype: MT
ms.contentlocale: id-ID
ms.lasthandoff: 08/05/2021
ms.locfileid: "54085231"
---
# <a name="troubleshoot-access-denied-messages-in-sharepointonedrive-admin-center"></a>Memecahkan masalah Akses Pesan yang Ditolak di Pusat Admin Sharepoint/OneDrive

Jika Menerima pesan yang menolak akses saat mencoba menelusuri Pusat Admin Sharepoint/OneDrive, pastikan untuk menetapkan lisensi kepada [pengguna.](https://docs.microsoft.com/microsoft-365/admin/add-users/add-users) Jika pengguna mempunyai lisensi, Anda juga harus memastikan mereka [diberi peran administrator yang](https://docs.microsoft.com/microsoft-365/admin/add-users/about-admin-roles) bisa mengakses pusat admin.

Masalah ini juga dapat terjadi ketika pengguna dihapus dan dibuat ulang dengan nama prinsipal pengguna (UPN) yang sama. Akun baru dibuat dengan menggunakan nilai PUID (ID Unik Paspor) yang berbeda. Saat pengguna berusaha mengakses kumpulan situs atau situs OneDrive, pengguna memiliki PUID yang tidak benar. Skenario kedua melibatkan sinkronisasi direktori dengan Unit organisasi Direktori Aktif (OU). Jika pengguna sudah masuk ke SharePoint lalu dipindahkan ke OU lain dan disinkronkan kembali dengan SharePoint, mereka mungkin mengalami masalah ini.

Untuk mengatasi masalah ini, Anda harus memulihkan UPN asli dengan langkah-langkah dalam artikel, [Memulihkan pengguna di Microsoft 365](https://docs.microsoft.com/microsoft-365/admin/add-users/restore-user).

Catatan: Jika Pusat OneDrive atau SharePoint Admin tidak tersedia bagi beberapa pengguna yang sebelumnya memiliki akses, mungkin terdapat masalah layanan sementara.  [Periksa dasbor kesehatan layanan](https://portal.office.com/adminportal/home#/servicehealth).


