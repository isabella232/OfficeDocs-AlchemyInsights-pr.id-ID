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
ms.openlocfilehash: 0dee7e44a8701e1df924b9657cce6cf9d90160e58277d667f6069a4cbcf87ce5
ms.sourcegitcommit: b5f7da89a650d2915dc652449623c78be6247175
ms.translationtype: MT
ms.contentlocale: id-ID
ms.lasthandoff: 08/05/2021
ms.locfileid: "54057105"
---
# <a name="find-missing-applications-on-app-registration-blade"></a>Temukan aplikasi yang hilang di App Registration blade

1. Tidak dapat menemukan aplikasi di portal Registrasi Aplikasi.

    Jika aplikasi merupakan aplikasi multi-penyewa dan telah didaftarkan di penyewa lain, aplikasi tidak akan ditampilkan di bawah blade Registrasi Aplikasi. Namun, Anda dapat menemukannya di bawah Aplikasi Enterprise blade setelah dapat diakses (setelah disetujui) dan prinsipal layanan telah dibuat di penyewa Anda. Untuk informasi selengkapnya, lihat [Prinsipal & aplikasi di Azure AD - platform identitas Microsoft](https://docs.microsoft.com/azure/active-directory/develop/app-objects-and-service-principals).
2. Tidak dapat menampilkan aplikasi di App Registration blade meskipun Anda adalah admin.

    Pastikan Anda berada dalam direktori yang tepat di portal Azure.
3. Aplikasi saya tidak tercantum di bawah blade Aplikasi Perusahaan namun muncul ketika saya membuat kueri perintah PowerShell.

    Terkadang, setelah Anda menghapus aplikasi dari portal Azure, aplikasi tidak muncul di portal tetapi mungkin belum dihapus sepenuhnya. Untuk informasi selengkapnya, lihat:
    - Anda dapat mengambil daftar aplikasi yang dihapus sebelumnya dan melihat apakah aplikasi tersebut muncul dalam daftar menggunakan perintah Powershell: **Get-AzureADDeletedApplication**. Untuk mempelajari selengkapnya, lihat [Get-AzureADDeletedApplication (AzureAD).](https://docs.microsoft.com/powershell/module/azuread/get-azureaddeletedapplication)
    - Jika ingin menghapus aplikasi sepenuhnya, Anda dapat mencoba hal berikut ini di PowerShell: **Remove-AzureADApplication -ObjectId**. Untuk mempelajari selengkapnya, lihat [Remove-AzureADApplication (AzureAD).](https://docs.microsoft.com/powershell/module/azuread/remove-azureadapplication)
    - Atau, Anda dapat mencoba memulihkan aplikasi yang dihapus menggunakan perintah Powershell berikut ini: **Pulihkan AzureADDeletedApplication -ObjectId**. Untuk mempelajari selengkapnya, lihat [Restore-AzureADDeletedApplication (AzureAD).](https://docs.microsoft.com/powershell/module/azuread/restore-azureaddeletedapplication)
4. Tidak dapat menemukan daftar semua aplikasi perusahaan yang telah terinstal sebelumnya di penyewa Azure baru saya.

    Tidak ada aplikasi perusahaan yang terinstal sebelumnya di Azure AD secara default. Anda perlu menambahkannya secara manual dari opsi 'Aplikasi baru' dengan menelusurinya dari galeri Azure AD atau menambahkan aplikasi non-galeri. Untuk mempelajari selengkapnya, [lihat Mulai cepat: Menambahkan aplikasi ke penyewa Azure Active Directory (Azure AD) Anda.](https://docs.microsoft.com/azure/active-directory/manage-apps/add-application-portal)
    Jika Anda administrator global, Anda bisa dengan mudah mengakses aplikasi Anda menggunakan [Microsoft 365 App Launcher](https://docs.microsoft.com/microsoft-365/admin/manage/customize-the-app-launcher).
5. Tidak dapat menemukan aplikasi dari portal Aplikasi Saya.

    Pastikan bahwa aplikasi tidak tersembunyi di halaman kumpulan Aplikasi Saya. Untuk mempelajari selengkapnya, lihat [Koleksi (pratinjau) di portal Aplikasi Saya - Azure AD](https://docs.microsoft.com/azure/active-directory/user-help/my-apps-portal-user-collections).
6. Untuk memulai aplikasi dari portal Aplikasi Saya, lihat [Temukan & menggunakan aplikasi di portal Aplikasi Saya - Azure AD](https://docs.microsoft.com/azure/active-directory/user-help/my-apps-portal-end-user-access).
7. Office 365 Aplikasi Mover tidak muncul di blade Aplikasi Enterprise setelah penginstalan.

    Aplikasi "Office 365 Pindahkan Gambar" merupakan aplikasi multi-fungsi yang tidak perlu ditambahkan ke AAD menggunakan bagian Aplikasi Galeri di bawah Registrasi Aplikasi Perusahaan. Untuk mengakses Office 365 Mover Anda, cukup masuk ke aplikasi dan aplikasi akan meminta persetujuan pengguna atas izin tersebut. Setelah pengguna memberikan izin, aplikasi ini akan secara otomatis ditambahkan ke penyewa dengan id email yang telah Anda masuki.

    Setelah masuk ke aplikasi, Anda akan dapat menemukan entri aplikasi ini di bawah blade Enterprise Applications di AAD. Anda perlu mencari aplikasi tersebut dengan mengetikkan nama lengkap, seperti "Office 365 Mover" atau cukup cari "office" dan aplikasi harus mencantumkannya. Untuk mempelajari selengkapnya, lihat Office 365 Mover mengatakan aplikasi telah terinstal tetapi [tidak tercantum di galeri Aplikasi Perusahaan.](https://docs.microsoft.com/answers/questions/30186/office-365-mover-says-its-already-installed-but-it.html)
8. Mulai Cepat: Tampilkan daftar aplikasi yang menggunakan penyewa [Azure Active Directory (Azure AD)](https://docs.microsoft.com/azure/active-directory/manage-apps/view-applications-portal) untuk manajemen identitas untuk manajemen identitas memperlihatkan cara menampilkan aplikasi, yang juga dikenal sebagai aplikasi, yang telah disiapkan untuk menggunakan penyewa Azure AD sebagai Penyedia Identitas (IdP, Identity Provider).
9. [Pecahkan masalah umum saat menambahkan atau menghapus aplikasi untuk Azure Active Directory](https://docs.microsoft.com/azure/active-directory/manage-apps/troubleshoot-adding-apps) Anda memahami masalah umum yang sering terjadi saat menampilkan aplikasi Azure Active Directory.
