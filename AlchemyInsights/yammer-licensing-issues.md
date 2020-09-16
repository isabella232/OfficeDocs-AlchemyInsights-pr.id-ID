---
title: Masalah lisensi Yammer
ms.author: pebaum
author: pebaum
manager: scotv
ms.date: 07/14/2020
ms.audience: Admin
ms.topic: article
ms.service: o365-administration
ROBOTS: NOINDEX, NOFOLLOW
localization_priority: Priority
ms.collection: Adm_O365
ms.custom:
- "5900"
- "9003071"
ms.openlocfilehash: f0a7625c7b77860e5ba0e29f2df47101749aace3
ms.sourcegitcommit: c6692ce0fa1358ec3529e59ca0ecdfdea4cdc759
ms.translationtype: MT
ms.contentlocale: id-ID
ms.lasthandoff: 09/14/2020
ms.locfileid: "47657279"
---
# <a name="yammer-licensing-issues"></a>Masalah lisensi Yammer

Semua pengguna harus memiliki lisensi untuk menggunakan layanan Yammer Enterprise, namun secara default Yammer tidak mengharuskan pengguna memiliki lisensi untuk mengakses layanan. Saat administrator mengubah pengaturan untuk memblokir pengguna Microsoft 365 tanpa lisensi Yammer, pengguna tidak diberi lisensi Yammer Enterprise tidak bisa mengakses layanan Yammer. Untuk informasi selengkapnya, lihat [mengelola lisensi pengguna Yammer di Office 365](https://docs.microsoft.com/yammer/manage-yammer-users/manage-yammer-licenses-in-office-365) 

Saat lisensi dihapus dari pengguna, petak Yammer tidak lagi ditampilkan, dan layanan lainnya bisa menggunakan penghapusan lisensi untuk menyembunyikan fitur. Dalam kasus lain, fitur masih bisa muncul tapi memerlukan penugasan lisensi untuk beroperasi.  

**Lisensi tidak diperbarui untuk pengguna**  

Terkadang, pengguna diberi lisensi tetapi masih tidak dapat mengakses Yammer. Penundaan lebih mungkin terjadi ketika tugas lisensi massal sedang dalam proses. Pengguna Yammer mungkin tidak diperbarui dalam urutan yang sama seperti lisensi yang diubah di Azure AD karena sistem berjalan asinkron. Tunggu hingga 24 jam sebelum membuka kasus dukungan untuk melaporkan masalah sinkronisasi lisensi.  

**Penetapan lisensi massal**  

Lisensi bisa ditetapkan melalui Pusat admin atau scripting PowerShell. Untuk informasi selengkapnya, lihat [menetapkan lisensi kepada pengguna](https://docs.microsoft.com/microsoft-365/admin/manage/assign-licenses-to-users) dan [menetapkan lisensi ke akun pengguna dengan Office 365 PowerShell](https://docs.microsoft.com/office365/enterprise/powershell/assign-licenses-to-user-accounts-with-office-365-powershell). 

Dukungan Microsoft tidak menyediakan bantuan dengan membuat skrip, tapi dokumentasi tentang penetapan lisensi Yammer tersedia. Untuk informasi selengkapnya, lihat [mengelola lisensi Yammer menggunakan Windows PowerShell](https://docs.microsoft.com/yammer/manage-yammer-users/manage-yammer-licenses-in-office-365#manage-yammer-licenses-by-using-windows-powershell).