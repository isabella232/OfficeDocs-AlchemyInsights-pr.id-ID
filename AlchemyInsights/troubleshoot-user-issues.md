---
title: Memecahkan masalah pengguna
ms.author: v-smandalika
author: v-smandalika
manager: dansimp
ms.date: 01/15/2021
ms.audience: Admin
ms.topic: article
ms.service: o365-administration
ROBOTS: NOINDEX, NOFOLLOW
localization_priority: Priority
ms.collection: Adm_O365
ms.custom:
- "7813"
- "9004358"
ms.openlocfilehash: d9964e50bdea0c41ac14ab3783b579034b5f2c8c
ms.sourcegitcommit: 6d02eb533fd74199af6b20f714b3720991da2c4a
ms.translationtype: MT
ms.contentlocale: id-ID
ms.lasthandoff: 01/18/2021
ms.locfileid: "49901040"
---
# <a name="announcements"></a>Penawaran

Ikuti panduan Google tentang menguji kompatibilitas untuk menguji apakah aplikasi Anda terpengaruh. Panduan Google tersedia di https://docs.microsoft.com/azure/active-directory/external-identities/google-federation#deprecation-of-webview-sign-in-support .

Pastikan Anda menggunakan browser sistem WebView atau sistem saat masuk ke pengguna Anda dengan akun Google konsumen. Untuk informasi selengkapnya, lihat [masalah masuk ke aplikasi menggunakan browser Chrome saja](https://docs.microsoft.com/office365/troubleshoot/miscellaneous/chrome-behavior-affects-applications).


**Saya tidak dapat membuat pengguna baru di direktori Azure AD saya**

Untuk memecahkan masalah tidak dapat membuat pengguna baru di Azure AD, lakukan langkah-langkah berikut:

1. Pastikan bahwa Anda memiliki wewenang untuk membuat pengguna standar baru. Hanya peran administrator global atau administrator pengguna di Azure Active Directory (AD) yang dapat membuat pengguna standar baru. Jika Anda tidak berada di salah satu peran ini, mintalah administrator untuk menambahkan Anda ke salah satu peran ini atau untuk membuat akun pengguna baru untuk Anda.
2. Pastikan bahwa nama pengguna berada di domain yang diverifikasi di Azure AD Anda. Jika Anda tidak memiliki nama domain kustom yang diverifikasi di Azure AD Anda, Anda bisa menggunakan domain awal Azure AD, yang diakhiri dengan *. onmicrosoft.com.
3. Pastikan bahwa nama pengguna berada di domain yang tidak digabungkan ke Azure AD dari iklan lokal Anda. Pengguna tidak dapat ditambahkan di awan dengan nama domain yang digabungkan dari lokal.
4. Pastikan bahwa tidak ada pengguna atau kontak lain yang sudah memiliki nama pengguna yang ingin Anda tetapkan ke pengguna baru. Nama pengguna harus unik di seluruh Azure AD.
5. Lihat [AZURE AD peran dan administrator](https://ms.portal.azure.com/#blade/Microsoft_AAD_IAM/ActiveDirectoryMenuBlade/RolesAndAdministrators) untuk Azure AD Anda.
6. Lihat [nama domain](https://ms.portal.azure.com/#blade/Microsoft_AAD_IAM/ActiveDirectoryMenuBlade/Domains) untuk Azure AD Anda.
7. Tinjau [log audit](https://ms.portal.azure.com/#blade/Microsoft_AAD_IAM/ActiveDirectoryMenuBlade/Audit) untuk melihat informasi mendetail selengkapnya tentang pengguna yang baru dibuat atau dihapus seperti siapa yang melakukan tindakan dan kapan.
8. Untuk informasi selengkapnya tentang menambahkan pengguna baru, lihat [menggunakan Azure portal untuk membuat pengguna baru di AZURE AD Anda](https://docs.microsoft.com/azure/active-directory/fundamentals/add-users-azure-active-directory) .
9. Untuk informasi selengkapnya tentang izin peran administrator di Azure AD, lihat [peran administratif AZURE AD](https://docs.microsoft.com/azure/active-directory/roles/permissions-reference).
10. Untuk detail tentang membuat pengguna menggunakan PowerShell Azure AD, lihat [AZURE AD PowerShell untuk membuat pengguna baru](https://docs.microsoft.com/powershell/module/azuread/new-azureaduser).

**Masalah dengan pendaftaran layanan mandiri**

Untuk memecahkan masalah terkait pendaftaran layanan mandiri, lakukan langkah-langkah berikut:

1. Untuk menggunakan pendaftaran layanan mandiri dengan aplikasi Anda, pertama-tama aktifkan pendaftaran layanan mandiri untuk penyewa Anda. 
2. Untuk mengaktifkan aplikasi untuk mendukung pendaftaran layanan mandiri, tambahkan ke alur pengguna Anda. Saat berikutnya Anda masuk ke halaman masuk untuk aplikasi tersebut, Anda akan melihat opsi **_tanpa akun? Buat satu!_* _. Ini memulai proses pendaftaran layanan mandiri.
3. Untuk informasi tentang cara menggunakan daftar layanan mandiri untuk mengisi organisasi di Azure AD, lihat [mendaftar layanan mandiri untuk AZURE AD](https://docs.microsoft.com/azure/active-directory/enterprise-users/directory-self-service-signup).
4. Setelah mengaitkan alur pengguna dengan satu atau beberapa aplikasi, pengguna yang mengunjungi aplikasi tersebut akan bisa mendaftar dan mendapatkan akun tamu menggunakan opsi yang dikonfigurasi dalam alur pengguna. Untuk informasi selengkapnya tentang mendaftar dan mendapatkan akun tamu, pengguna bisa melihat [pendaftaran layanan mandiri untuk pengguna tamu](https://docs.microsoft.com/azure/active-directory/external-identities/self-service-sign-up-user-flow).

_ *Problem mengundang pengguna eksternal**

Untuk memecahkan masalah terkait mengundang pengguna eksternal, lakukan langkah berikut:

Pastikan Anda mengirim undangan pengguna ke alamat email yang cocok dengan nama pengguna yang masuk. Jika Anda mengirimkan undangan ke alamat email proksi pengguna, pengguna tidak dapat menukarkannya. Untuk informasi selengkapnya, lihat [dokumentasi AZURE AD B2B](https://docs.microsoft.com/azure/active-directory/external-identities/).

**Saya tidak dapat menetapkan lisensi untuk pengguna**

Untuk memecahkan masalah terkait penetapan lisensi kepada pengguna, lakukan langkah-langkah berikut:

1. Untuk mengelola lisensi pengguna, pastikan bahwa Anda menggunakan akun dengan salah satu peran administrator yang diperlukan: administrator global, administrator lisensi, atau administrator pengguna. Anda dapat memeriksa peran pengguna dalam tab **peran direktori** pada bilah pengguna.
2. Jika Anda menggunakan Azure portal dan penetapan lisensi gagal, klik pemberitahuan di sudut kanan atas. Ini akan membuka pisau dengan detail tentang apa yang salah. Dalam kebanyakan kasus yang cukup untuk memahami dan mengatasi masalah tersebut.
3. Sebelum lisensi dapat ditetapkan ke pengguna, pastikan bahwa properti **lokasi penggunaan** diatur untuk pengguna. Verifikasi bahwa pengguna memiliki kumpulan properti tersebut dengan menampilkan tab **profil** pada bilah pengguna.
4. Pastikan ada cukup lisensi yang tersedia untuk produk yang ingin Anda tetapkan. Anda dapat melihat jumlah lisensi yang tersedia di Azure portal, di [Azure Active Directory-> lisensi-> semua produk](https://ms.portal.azure.com/#blade/Microsoft_AAD_IAM/LicensesMenuBlade/Products).
5. Pengguna mungkin sudah memiliki lisensi lain yang berkonflik dengan layanannya dalam lisensi baru yang ingin Anda tetapkan. Misalnya, jika pengguna memiliki layanan Exchange Online (paket 1) yang diaktifkan, Anda tidak akan bisa menetapkan lisensi dengan Exchange Online (paket 2). Nonaktifkan salah satu layanan untuk memperbolehkan penetapan lisensi baru. Jika Anda menggunakan cmdlet Azure portal atau PowerShell, halaman **detail masalah** mencantumkan layanan tertentu yang menyebabkan konflik.
6. Jika Anda mencoba menghapus lisensi dan yang gagal, pengguna mungkin memiliki lisensi lain dengan layanan yang bergantung pada layanan yang coba Anda hapus. Jika Anda menggunakan cmdlet Azure portal atau PowerShell, pesan kesalahan akan mencantumkan layanan tertentu yang memiliki dependensi.
7. Jika Anda ingin memahami mengapa lisensi ditambahkan/dihapus dari pengguna (misalnya, siapa saja di organisasi Anda yang mungkin telah membuat perubahan), periksa log audit. Setel filter ke **aktivitas lisensi** untuk memperlihatkan semua modifikasi, termasuk "aktor" yang menampilkannya.
8. Jika Anda menggunakan Exchange Online, beberapa pengguna di penyewa Anda mungkin salah dikonfigurasikan dengan nilai alamat proksi yang sama. Dalam kasus tersebut, Anda mungkin melihat pesan kesalahan generik ketika operasi lisensi gagal. [Artikel ini](https://docs.microsoft.com/exchange/troubleshoot/administration/proxy-address-being-used) berisi informasi selengkapnya tentang masalah ini, termasuk informasi tentang [cara menyambungkan ke Exchange Online menggunakan PowerShell jarak jauh](https://docs.microsoft.com/powershell/exchange/connect-to-exchange-online-powershell). Untuk mengidentifikasi pengguna mana di penyewa Anda, berisi alamat proksi yang sama, Jalankan cmdlet Exchange Online ini:

Menjalankan

Get-Recipient | di mana {$ _. EmailAddresses-Match <user principal name> } | Nama fL, RecipientType, EmailAddresses





