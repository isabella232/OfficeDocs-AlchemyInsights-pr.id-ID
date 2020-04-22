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
ms.openlocfilehash: 82e11458529b8a49e583b1a6963a51e2a466bfd6
ms.sourcegitcommit: 631cbb5f03e5371f0995e976536d24e9d13746c3
ms.translationtype: MT
ms.contentlocale: id-ID
ms.lasthandoff: 04/22/2020
ms.locfileid: "43758449"
---
# <a name="troubleshoot-access-denied-messages-in-sharepointonedrive-admin-center"></a>Memecahkan masalah Akses ditolak pesan di pusat admin SharePoint/OneDrive

Jika Anda menerima pesan Akses ditolak saat berusaha menjelajah ke Pusat admin SharePoint/OneDrive, pastikan bahwa Anda [menetapkan lisensi untuk pengguna](https://docs.microsoft.com/office365/admin/subscriptions-and-billing/assign-licenses-to-users?view=o365-worldwide&amp;tabs=One). Jika pengguna memiliki lisensi, Anda juga harus memastikan bahwa mereka [ditetapkan peran administrator](https://docs.microsoft.com/office365/admin/add-users/about-admin-roles?view=o365-worldwide) yang dapat mengakses pusat admin.

Masalah ini juga dapat terjadi ketika pengguna dihapus dan dibuat ulang dengan nama prinsip pengguna (UPN) yang sama. Akun baru dibuat dengan menggunakan nilai yang berbeda PUID (paspor unik ID). Saat pengguna berusaha mengakses koleksi situs atau OneDrive mereka, pengguna memiliki PUID salah. Skenario kedua melibatkan sinkronisasi direktori dengan direktori aktif unit organisasi (OU). Jika pengguna telah masuk ke SharePoint, dan kemudian dipindahkan ke OU berbeda dan resynced dengan SharePoint, mereka mungkin mengalami masalah ini.

Untuk mengatasi masalah ini, Anda harus memulihkan UPN asli dengan langkah dalam artikel, [memulihkan pengguna di Microsoft 365](https://docs.microsoft.com/office365/admin/add-users/restore-user?view=o365-worldwide).

Catatan: jika Pusat admin OneDrive atau SharePoint tidak tersedia untuk beberapa pengguna yang sebelumnya memiliki akses, mungkin ada masalah layanan sementara.  [Periksa dasbor Kesehatan Layanan](https://portal.office.com/adminportal/home#/servicehealth).


