---
title: Memecahkan masalah Akses ditolak pesan
ms.author: pebaum
author: pebaum
ms.date: 04/21/2020
ms.audience: ITPro
ms.topic: article
ROBOTS: NOINDEX, NOFOLLOW
localization_priority: Normal
ms.assetid: d678b57a-53ad-4414-9423-d8726a0c532f
ms.openlocfilehash: 9430b9786b35dda9fb2604fb6ae3c39c8c258d6e
ms.sourcegitcommit: bc7d6f4f3c9f7060d073f5130e1ec856e248d020
ms.translationtype: MT
ms.contentlocale: id-ID
ms.lasthandoff: 06/02/2020
ms.locfileid: "44505382"
---
# <a name="troubleshoot-access-denied-messages-in-sharepointonedrive-admin-center"></a>Memecahkan masalah Akses ditolak pesan di pusat admin SharePoint/OneDrive

Jika Anda menerima pesan Akses ditolak saat berusaha menjelajah ke Pusat admin SharePoint/OneDrive, pastikan bahwa Anda [menetapkan lisensi untuk pengguna](https://docs.microsoft.com/microsoft-365/admin/add-users/add-users). Jika pengguna memiliki lisensi, Anda juga harus memastikan bahwa mereka [ditetapkan peran administrator](hhttps://docs.microsoft.com/microsoft-365/admin/add-users/about-admin-roles) yang dapat mengakses pusat admin.

Masalah ini juga dapat terjadi ketika pengguna dihapus dan dibuat ulang dengan nama prinsip pengguna (UPN) yang sama. Akun baru dibuat dengan menggunakan nilai yang berbeda PUID (paspor unik ID). Saat pengguna berusaha mengakses koleksi situs atau OneDrive mereka, pengguna memiliki PUID salah. Skenario kedua melibatkan sinkronisasi direktori dengan direktori aktif unit organisasi (OU). Jika pengguna telah masuk ke SharePoint, dan kemudian dipindahkan ke OU berbeda dan resynced dengan SharePoint, mereka mungkin mengalami masalah ini.

Untuk mengatasi masalah ini, Anda harus memulihkan UPN asli dengan langkah dalam artikel, [memulihkan pengguna di Microsoft 365](https://docs.microsoft.com/microsoft-365/admin/add-users/restore-user).

Catatan: jika Pusat admin OneDrive atau SharePoint tidak tersedia untuk beberapa pengguna yang sebelumnya memiliki akses, mungkin ada masalah layanan sementara.  [Periksa dasbor Kesehatan Layanan](https://portal.office.com/adminportal/home#/servicehealth).


