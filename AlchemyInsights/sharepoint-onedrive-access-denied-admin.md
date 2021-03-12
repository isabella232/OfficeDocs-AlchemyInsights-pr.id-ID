---
title: Memecahkan masalah pesan Akses ditolak
ms.author: pebaum
author: pebaum
ms.date: 04/21/2020
ms.audience: ITPro
ms.topic: article
ms.service: o365-administration
ROBOTS: NOINDEX, NOFOLLOW
localization_priority: Normal
ms.assetid: d678b57a-53ad-4414-9423-d8726a0c532f
ms.openlocfilehash: 3189fa61d28253569278024d4191ee63b917509f
ms.sourcegitcommit: 0eb4f9bde53395b5fd4b5cd4ffc56ca96db91298
ms.translationtype: MT
ms.contentlocale: id-ID
ms.lasthandoff: 03/10/2021
ms.locfileid: "50707957"
---
# <a name="troubleshoot-access-denied-messages-in-sharepointonedrive-admin-center"></a>Memecahkan masalah akses pesan yang ditolak di pusat admin SharePoint/OneDrive

Jika Anda menerima pesan Akses ditolak saat mencoba menelusuri ke Pusat admin SharePoint/OneDrive, pastikan bahwa Anda [menetapkan lisensi untuk pengguna tersebut](https://docs.microsoft.com/microsoft-365/admin/add-users/add-users). Jika pengguna memiliki lisensi, Anda juga harus memastikan bahwa mereka [diberi peran administrator](https://docs.microsoft.com/microsoft-365/admin/add-users/about-admin-roles) yang bisa mengakses pusat admin.

Masalah ini juga bisa terjadi ketika pengguna dihapus dan dibuat ulang dengan nama prinsip pengguna (UPN) yang sama. Akun baru dibuat menggunakan nilai PUID (ID unik paspor) yang berbeda. Saat pengguna mencoba mengakses kumpulan situs atau OneDrive mereka, pengguna tersebut memiliki PUID yang salah. Skenario kedua melibatkan sinkronisasi direktori dengan unit organisasi direktori aktif (OU). Jika pengguna sudah masuk ke SharePoint, lalu dipindahkan ke OU berbeda dan resynced dengan SharePoint, mereka mungkin mengalami masalah ini.

Untuk mengatasi masalah ini, Anda harus memulihkan UPN asli dengan langkah-langkah dalam artikel, [memulihkan pengguna di Microsoft 365](https://docs.microsoft.com/microsoft-365/admin/add-users/restore-user).

Catatan: jika OneDrive atau pusat admin SharePoint tidak tersedia untuk beberapa pengguna yang sebelumnya memiliki Access, mungkin ada masalah layanan sementara.  [Periksa dasbor Kesehatan Layanan](https://portal.office.com/adminportal/home#/servicehealth).


