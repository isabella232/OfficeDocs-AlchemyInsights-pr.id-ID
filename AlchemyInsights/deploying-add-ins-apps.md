---
title: Menyebarkan add-in untuk Aplikasi Microsoft 365
ms.author: pebaum
author: pebaum
manager: scotv
ms.date: 04/30/2021
ms.audience: Admin
ms.topic: article
ms.service: o365-administration
ROBOTS: NOINDEX, NOFOLLOW
localization_priority: Normal
ms.collection: Adm_O365
ms.custom:
- "11107"
- "9005477"
ms.openlocfilehash: 3aacc3c6675f4102a5b34a435c862215dbfd0479b75549d608ed3c91021ed3d7
ms.sourcegitcommit: b5f7da89a650d2915dc652449623c78be6247175
ms.translationtype: MT
ms.contentlocale: id-ID
ms.lasthandoff: 08/05/2021
ms.locfileid: "54031409"
---
# <a name="deploying-add-ins-for-microsoft-365-apps"></a>Menyebarkan add-in untuk Aplikasi Microsoft 365

Penyebaran Terpusat adalah cara yang disarankan untuk menyebarkan add-in Office kepada pengguna dan grup dalam organisasi Anda. Untuk menyebarkan add-in, ikuti langkah-langkah di bawah ini:

**Catatan:** Untuk menginstal add-in bagi Office pengguna individu, lihat Menampilkan, mengelola, dan menginstal [add-in Office tertentu.](https://support.microsoft.com/topic/view-manage-and-install-add-ins-in-office-programs-16278816-1948-4028-91e5-76dca5380f8d) Selain itu, pastikan akuisisi individual Office add-in Bursa telah diaktifkan. Untuk detailnya, [lihat Mencegah pengunduhan add-in dengan](https://docs.microsoft.com/microsoft-365/admin/manage/manage-addins-in-the-admin-center?view=o365-worldwide#prevent-add-in-downloads-by-turning-off-the-office-store-across-all-clients-except-outlook)menonaktifkan Bursa Office di semua klien (Kecuali Outlook) .

1. Pastikan lingkungan Anda memenuhi persyaratan penyebaran add-in menggunakan Penyebaran Terpusat. Untuk detailnya, lihat [Persyaratan.](https://docs.microsoft.com/microsoft-365/admin/manage/centralized-deployment-of-add-ins?#requirements)
2. Masuk ke **Pengaturan**  >  **Dapatkan aplikasi**  >  **Terintegrasi** di pusat admin Microsoft 365 untuk menyebarkan add-in. 

Catatan: 

- Aplikasi Terintegrasi mengharuskan admin memiliki izin Admin Global Exchange Admin.

- Ketika menyebarkan add-in ke beberapa pengguna, kami menyarankan penetapan dilakukan menggunakan grup dan bukan pengguna individu. Untuk detailnya, [lihat Pertimbangan saat menetapkan add-in ke pengguna dan grup](https://docs.microsoft.com/microsoft-365/admin/manage/manage-deployment-of-add-ins?view=o365-worldwide#considerations-when-assigning-an-add-in-to-users-and-groups).

- Penyebaran Terpusat tidak mendukung pengguna dalam grup bertumpuk atau grup yang memiliki grup induk. Untuk detailnya, [lihat Penetapan pengguna dan grup](https://docs.microsoft.com/microsoft-365/admin/manage/centralized-deployment-of-add-ins?view=o365-worldwide#user-and-group-assignments).

- Pastikan bahwa Layanan Manajemen Aplikasi Microsoft 365 (GUID: '0517ffae-825d-4aff-999e-3f2336b8a20a') telah diaktifkan untuk masuk bagi pengguna. Untuk detailnya, [lihat Mengonfigurasi properti aplikasi](https://docs.microsoft.com/azure/active-directory/manage-apps/add-application-portal-configure#configure-app-properties).

- Jika Anda mengalami masalah dalam menyebarkan add-in menggunakan Aplikasi Terintegrasi, coba sebarkan menggunakan [Add-In.](https://admin.microsoft.com/AdminPortal/Home?#/Settings/AddIns)

Untuk informasi selengkapnya, lihat:

[Menyebarkan add-in di pusat admin](https://docs.microsoft.com/microsoft-365/admin/manage/manage-deployment-of-add-ins) 
 [Mengelola add-in di pusat admin](https://docs.microsoft.com/microsoft-365/admin/manage/manage-addins-in-the-admin-center) 
 [Menggunakan cmdlet PowerShell Penyebaran Terpusat untuk mengelola add-in](https://docs.microsoft.com/microsoft-365/enterprise/use-the-centralized-deployment-powershell-cmdlets-to-manage-add-ins) 
 [Menerbitkan Office Add-in menggunakan Penyebaran Terpusat melalui pusat admin Microsoft 365](https://docs.microsoft.com/office/dev/add-ins/publish/centralized-deployment#publish-an-office-add-in-via-centralized-deployment) 
 [Pemecahan masalah: Pengguna tidak melihat add-in](https://docs.microsoft.com/office365/troubleshoot/access-management/user-not-seeing-add-ins) 
 [Memecahkan masalah kesalahan pengguna Office Add-in](https://docs.microsoft.com/office/dev/add-ins/testing/testing-and-troubleshooting)