---
title: Masalah lisensi heboh
ms.author: pebaum
author: pebaum
manager: scotv
ms.date: 07/14/2020
ms.audience: Admin
ms.topic: article
ROBOTS: NOINDEX, NOFOLLOW
localization_priority: Priority
ms.collection: Adm_O365
ms.custom:
- "5900"
- "9003071"
ms.openlocfilehash: 6d9b2126dc1ed90968738ddb2e249dce9857f1db
ms.sourcegitcommit: b677b85395b7244b2bf2b753468b696b4cf27c8d
ms.translationtype: MT
ms.contentlocale: id-ID
ms.lasthandoff: 07/16/2020
ms.locfileid: "45148312"
---
# <a name="yammer-licensing-issues"></a>Masalah lisensi heboh

Semua pengguna harus memiliki izin untuk menggunakan layanan heboh perusahaan, tetapi secara default heboh tidak mengharuskan pengguna memiliki lisensi untuk mengakses layanan. Ketika administrator perubahan pengaturan untuk memblokir Microsoft 365 pengguna tanpa lisensi heboh, pengguna tidak ditetapkan lisensi heboh perusahaan tidak dapat mengakses layanan heboh. Untuk informasi lebih lanjut, lihat [mengelola heboh pengguna lisensi di Office 365](https://docs.microsoft.com/yammer/manage-yammer-users/manage-yammer-licenses-in-office-365) 

Ketika lisensi dihapus dari pengguna, ubin heboh tidak lagi ditampilkan, dan layanan lainnya dapat menggunakan penghapusan lisensi untuk menyembunyikan fitur. Dalam kasus lain, fitur masih dapat muncul tetapi memerlukan penetapan lisensi untuk beroperasi.  

**Lisensi tidak mendapatkan diperbarui untuk pengguna**  

Terkadang, pengguna ditetapkan lisensi tetapi masih tidak dapat mengakses heboh. Penundaan cenderung terjadi ketika penetapan lisensi massal sedang berlangsung. Heboh pengguna mungkin tidak diperbarui dalam urutan yang sama sebagai lisensi diubah di Azure AD karena sistem berjalan asinkron. Tunggu hingga 24 jam sebelum membuka kasus dukungan untuk melaporkan masalah sinkronisasi lisensi.  

**Tugas lisensi massal**  

Lisensi dapat ditetapkan melalui Pusat admin atau skrip PowerShell. Untuk informasi lebih lanjut, lihat [menetapkan lisensi untuk pengguna](https://docs.microsoft.com/microsoft-365/admin/manage/assign-licenses-to-users) dan [menetapkan lisensi untuk account pengguna dengan Office 365 PowerShell](https://docs.microsoft.com/office365/enterprise/powershell/assign-licenses-to-user-accounts-with-office-365-powershell). 

Dukungan Microsoft tidak memberikan bantuan dengan membuat skrip, namun dokumentasi tentang penetapan lisensi Yammer tersedia. Untuk informasi lebih lanjut, lihat [mengelola heboh lisensi dengan menggunakan Windows PowerShell](https://docs.microsoft.com/yammer/manage-yammer-users/manage-yammer-licenses-in-office-365#manage-yammer-licenses-by-using-windows-powershell).