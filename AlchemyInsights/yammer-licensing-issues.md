---
title: Yammer lisensi
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
ms.openlocfilehash: 3ec764ece9cb7be933e9e2cd002379898522790528b0fa586ab501424b00cd7b
ms.sourcegitcommit: b5f7da89a650d2915dc652449623c78be6247175
ms.translationtype: MT
ms.contentlocale: id-ID
ms.lasthandoff: 08/05/2021
ms.locfileid: "53989732"
---
# <a name="yammer-licensing-issues"></a>Yammer lisensi

Semua pengguna harus memiliki lisensi untuk menggunakan layanan Yammer Enterprise, tapi secara default Yammer tidak mengharuskan pengguna tersebut memiliki lisensi untuk mengakses layanan. Saat administrator mengubah pengaturan untuk memblokir Microsoft 365 pengguna tanpa lisensi Yammer, pengguna yang tidak diberi lisensi Yammer Enterprise tidak bisa mengakses layanan Yammer. Untuk informasi selengkapnya, [lihat Mengelola Yammer pengguna di Office 365](https://docs.microsoft.com/yammer/manage-yammer-users/manage-yammer-licenses-in-office-365) 

Saat lisensi dihapus dari pengguna, petak Yammer tidak lagi ditampilkan, dan layanan lain dapat menggunakan penghapusan lisensi untuk menyembunyikan fitur. Dalam kasus lain, fitur masih dapat muncul tetapi memerlukan penetapan lisensi untuk beroperasi.  

**Lisensi tidak diperbarui untuk pengguna**  

Terkadang, pengguna diberikan lisensi tapi masih tidak bisa mengakses Yammer. Penundaan lebih mungkin terjadi saat penetapan lisensi massal sedang berlangsung. Yammer pengguna mungkin tidak diperbarui dalam urutan yang sama seperti lisensi diubah di Azure AD karena sistem berjalan asinkron. Tunggu hingga 24 jam sebelum membuka kasus dukungan untuk melaporkan masalah sinkronisasi lisensi.  

**Penetapan lisensi massal**  

Lisensi dapat ditetapkan melalui pusat admin atau pembuatan skrip PowerShell. Untuk informasi selengkapnya, [lihat Menetapkan lisensi kepada pengguna](https://docs.microsoft.com/microsoft-365/admin/manage/assign-licenses-to-users) dan Menetapkan lisensi ke akun pengguna dengan Office 365 [PowerShell](https://docs.microsoft.com/office365/enterprise/powershell/assign-licenses-to-user-accounts-with-office-365-powershell). 

Dukungan Microsoft tidak menyediakan bantuan pembuatan skrip, tetapi dokumentasi tentang penetapan Yammer lisensi tersedia. Untuk informasi selengkapnya, [lihat Yammer lisensi dengan menggunakan Windows PowerShell](https://docs.microsoft.com/yammer/manage-yammer-users/manage-yammer-licenses-in-office-365#manage-yammer-licenses-by-using-windows-powershell).