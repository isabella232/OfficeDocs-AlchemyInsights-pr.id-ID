---
title: Mengatasi masalah Akses ditolak pesan
ms.author: kirks
author: Techwriter40
ms.date: 6/29/2018
ms.audience: ITPro
ms.topic: article
ROBOTS: NOINDEX, NOFOLLOW
localization_priority: Normal
ms.assetid: d678b57a-53ad-4414-9423-d8726a0c532f
ms.openlocfilehash: c204f1889e03886fdfd3d1c760a4a2beb82b0836
ms.sourcegitcommit: 4b7e478ce700c0b781efec3857ac4dce5bdf00c6
ms.translationtype: MT
ms.contentlocale: id-ID
ms.lasthandoff: 06/07/2019
ms.locfileid: "34760344"
---
# <a name="troubleshoot-access-denied-messages-in-sharepointonedrive-admin-center"></a>Mengatasi masalah Akses ditolak pesan di Sharepoint OneDrive Admin Center

Jika Anda menerima Akses ditolak pesan ketika mencoba untuk menelusuri Sharepoint OneDrive Admin Center, pastikan bahwa Anda [menetapkan lisensi ke pengguna](https://docs.microsoft.com/office365/admin/subscriptions-and-billing/assign-licenses-to-users?view=o365-worldwide&amp;tabs=One). Jika pengguna memiliki lisensi, Anda juga harus memastikan mereka adalah [menetapkan peran administrator](https://docs.microsoft.com/office365/admin/add-users/about-admin-roles?view=o365-worldwide) yang dapat mengakses pusat admin.

Masalah ini juga dapat terjadi ketika pengguna dihapus dan kembali dibuat dengan sama pengguna (UPN nama dasar). Account yang baru dibuat dengan menggunakan PUID (paspor unik ID) nilai yang berbeda. Ketika pengguna mencoba untuk mengakses situs koleksi atau OneDrive mereka, pengguna memiliki PUID salah. Skenario yang kedua melibatkan sinkronisasi direktori dengan unit organisasi Active Directory (OU). Jika pengguna telah sudah masuk ke SharePoint, dan kemudian pindah ke OU berbeda dan resynced dengan SharePoint, mereka mungkin mengalami masalah ini.

Untuk mengatasi masalah ini, Anda harus mengembalikan UPN asli dengan langkah-langkah dalam artikel, [mengembalikan pengguna di Office 365](https://docs.microsoft.com/office365/admin/add-users/restore-user?view=o365-worldwide).

Catatan: Jika pusat OneDrive atau SharePoint Admin tidak tersedia untuk beberapa pengguna yang sebelumnya mempunyai akses, mungkin ada masalah sementara layanan.  [Periksa layanan kesehatan dashboard](https://portal.office.com/adminportal/home#/servicehealth).


