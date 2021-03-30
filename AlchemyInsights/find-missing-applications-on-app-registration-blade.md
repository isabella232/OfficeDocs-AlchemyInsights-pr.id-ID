---
title: Temukan aplikasi yang hilang di App Registration blade
ms.author: v-jmathew
author: v-jmathew
manager: scotv
audience: Admin
ms.topic: article
ms.service: o365-administration
ROBOTS: NOINDEX, NOFOLLOW
localization_priority: Normal
ms.collection: Adm_O365
ms.custom:
- "9004352"
- "9654"
ms.openlocfilehash: 00b5821e2edad8b60ff60b1f85264d81c72277e4
ms.sourcegitcommit: 1f43598a726cdb9904aa501eb8db87f143020d9e
ms.translationtype: MT
ms.contentlocale: id-ID
ms.lasthandoff: 03/23/2021
ms.locfileid: "51404696"
---
# <a name="find-missing-applications-on-app-registration-blade"></a>Temukan aplikasi yang hilang di App Registration blade

1. Tidak dapat menemukan aplikasi di portal Registrasi Aplikasi.

    Jika aplikasi merupakan aplikasi multi-penyewa dan telah didaftarkan di penyewa lain, aplikasi tidak akan ditampilkan di bawah blade Registrasi Aplikasi. Namun, Anda dapat menemukannya di bawah Aplikasi Enterprise blade setelah dapat diakses (setelah disetujui) dan prinsipal layanan telah dibuat di penyewa Anda. Untuk informasi selengkapnya, lihat [Dukungan & prinsipal layanan di Azure AD - platform identitas Microsoft.](https://docs.microsoft.com/azure/active-directory/develop/app-objects-and-service-principals)
2. Tidak dapat menampilkan aplikasi di App Registration blade meskipun Anda adalah admin.

    Pastikan Anda berada dalam direktori yang tepat di portal Azure.
3. Aplikasi saya tidak tercantum di bawah blade Aplikasi Perusahaan namun muncul ketika saya membuat kueri perintah PowerShell.

    Terkadang, setelah Anda menghapus aplikasi dari portal Azure, aplikasi tidak muncul di portal tetapi mungkin belum dihapus sepenuhnya. Untuk informasi selengkapnya, lihat:
    - Anda dapat mengambil daftar aplikasi yang dihapus sebelumnya dan melihat apakah aplikasi tersebut muncul dalam daftar menggunakan perintah Powershell: **Get-AzureADDeletedApplication**. Untuk mempelajari selengkapnya, lihat [Get-AzureADDeletedApplication (AzureAD).](https://docs.microsoft.com/powershell/module/azuread/get-azureaddeletedapplication)
    - Jika ingin menghapus aplikasi sepenuhnya, Anda dapat mencoba hal berikut ini di PowerShell: **Remove-AzureADApplication -ObjectId**. Untuk mempelajari selengkapnya, lihat [Remove-AzureADApplication (AzureAD).](https://docs.microsoft.com/powershell/module/azuread/remove-azureadapplication)
    - Atau, Anda dapat mencoba memulihkan aplikasi yang dihapus menggunakan perintah Powershell berikut ini: **Pulihkan AzureADDeletedApplication -ObjectId**. Untuk mempelajari selengkapnya, lihat [Restore-AzureADDeletedApplication (AzureAD).](https://docs.microsoft.com/powershell/module/azuread/restore-azureaddeletedapplication)
4. Tidak dapat menemukan daftar semua aplikasi perusahaan yang telah terinstal sebelumnya di penyewa Azure baru saya.

    Tidak ada aplikasi perusahaan yang terinstal sebelumnya di Azure AD secara default. Anda perlu menambahkannya secara manual dari opsi 'Aplikasi baru' dengan menelusurinya dari galeri Azure AD atau menambahkan aplikasi non-galeri. Untuk mempelajari selengkapnya, [lihat Mulai cepat: Menambahkan aplikasi ke penyewa Azure Active Directory (Azure AD) Anda.](https://docs.microsoft.com/azure/active-directory/manage-apps/add-application-portal)
    Jika Anda merupakan administrator global, Anda dapat dengan mudah mengakses aplikasi menggunakan [Peluncur Aplikasi Microsoft 365.](https://docs.microsoft.com/microsoft-365/admin/manage/customize-the-app-launcher)
5. Tidak dapat menemukan aplikasi dari portal Aplikasi Saya.

    Pastikan bahwa aplikasi tidak tersembunyi di halaman kumpulan Aplikasi Saya. Untuk mempelajari selengkapnya, lihat [Koleksi (pratinjau) di portal Aplikasi Saya - Azure AD](https://docs.microsoft.com/azure/active-directory/user-help/my-apps-portal-user-collections).
6. Untuk memulai aplikasi dari portal Aplikasi Saya, lihat [Temukan & menggunakan aplikasi di portal Aplikasi Saya - Azure AD](https://docs.microsoft.com/azure/active-directory/user-help/my-apps-portal-end-user-access).
7. Aplikasi Office 365 Mover tidak muncul di blade Enterprise Applications setelah penginstalan.

    Aplikasi "Pemindahan Office 365" merupakan aplikasi multi-fungsi yang tidak perlu ditambahkan ke AAD menggunakan bagian Aplikasi Galeri di bawah Registrasi Aplikasi Perusahaan. Untuk mengakses aplikasi Office 365 Mover, cukup masuk ke aplikasi dan aplikasi akan meminta persetujuan pengguna atas izin tersebut. Setelah pengguna memberikan izin, aplikasi ini akan secara otomatis ditambahkan ke penyewa dengan id email yang telah Anda masuki.

    Setelah masuk ke aplikasi, Anda akan dapat menemukan entri aplikasi ini di bawah blade Enterprise Applications di AAD. Anda perlu mencari aplikasi tersebut dengan mengetikkan nama lengkap, misalnya, "Office 365 Mover" atau cukup cari "office" dan aplikasi harus mencantumkannya. Untuk mempelajari selengkapnya, lihat [Office 365 Mover](https://docs.microsoft.com/answers/questions/30186/office-365-mover-says-its-already-installed-but-it.html)mengatakan program telah terinstal tetapi tidak tercantum di galeri Aplikasi Perusahaan.
8. Mulai Cepat: Tampilkan daftar aplikasi yang menggunakan penyewa [Azure Active Directory (Azure AD)](https://docs.microsoft.com/azure/active-directory/manage-apps/view-applications-portal) untuk manajemen identitas memperlihatkan cara menampilkan aplikasi, yang juga dikenal sebagai aplikasi, yang telah disiapkan untuk menggunakan penyewa Azure AD sebagai Penyedia Identitas (IdP) mereka.
9. [Pecahkan masalah umum menambahkan atau menghapus aplikasi ke Azure Active Directory](https://docs.microsoft.com/azure/active-directory/manage-apps/troubleshoot-adding-apps) membantu Anda memahami masalah umum yang dihadapi orang-orang yang menampilkan aplikasi di Azure Active Directory.
