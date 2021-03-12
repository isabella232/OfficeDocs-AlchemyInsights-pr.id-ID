---
title: Memecahkan masalah grup
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
- "7814"
- "9004358"
ms.openlocfilehash: 7e2957a27305e8fb0bfd10e21189cef9870c5aaa
ms.sourcegitcommit: 6d02eb533fd74199af6b20f714b3720991da2c4a
ms.translationtype: MT
ms.contentlocale: id-ID
ms.lasthandoff: 01/18/2021
ms.locfileid: "50714054"
---
# <a name="troubleshoot-group-issues"></a>Memecahkan masalah grup

**Saya perlu menetapkan grup ke peran Azure AD**

Untuk menetapkan grup Azure Active Directory (AD) ke peran Azure AD, lakukan langkah-langkah berikut:

1. Membuat grup baru-untuk membuat grup baru:

    untuk. Masuk ke Pusat admin Azure AD dengan administrator peran istimewa atau izin administrator global. 
    b. Pilih grup > direktori aktif Azure > semua grup > grup baru. 
    's. Buat grup.

2. Tetapkan peran ke grup selama pembuatan grup atau setelah grup dibuat.

    untuk. Untuk menetapkan peran ke grup pada saat pembuatan grup, Aktifkan tombol Alihkan Azure AD bisa ditetapkan ke grup dan Buat grup.
    b. Untuk menetapkan peran ke grup setelah dibuat, navigasikan ke tab peran yang ditetapkan untuk grup yang baru dibuat, dan tetapkan peran ke grup.

**Saya perlu mengelola keanggotaan grup yang ditetapkan pada peran Azure AD**

1. Untuk mencegah elevasi hak istimewa, secara default, hanya administrator peran istimewa dan administrator global yang bisa mengubah keanggotaan grup yang ditetapkan untuk peran. Namun, mereka dapat memilih untuk menetapkan pemilik untuk grup tersebut dan mendelegasikan tugas ini. Untuk informasi selengkapnya, lihat, [menggunakan grup awan untuk mengelola penetapan peran di Azure Active Directory](https://docs.microsoft.com/azure/active-directory/roles/groups-concept).
2. Untuk pertanyaan Umum dan Tips pemecahan masalah untuk menetapkan peran ke grup di Azure AD, lihat [memecahkan masalah yang ditetapkan untuk grup awan](https://docs.microsoft.com/azure/active-directory/roles/groups-faq-troubleshooting).

**Grup dinamis**

1. Jika tidak dapat menemukan atribut pengguna bawaan, pastikan atribut tersebut ada dalam daftar properti yang didukung.
2. Jika Anda mencari atribut perangkat bawaan, pastikan bahwa atribut tersebut ada dalam daftar atribut perangkat 
3. Selain atribut pengguna dan perangkat bawaan, Anda juga dapat menggunakan [atribut ekstensi](https://docs.microsoft.com/azure/active-directory/enterprise-users/groups-dynamic-membership#extension-properties-and-custom-extension-properties). Setelah menyinkronkan atribut ekstensi dari AD Server Windows lokal atau dari aplikasi SaaS yang tersambung, atribut harus terlihat di daftar turun bawah penyusun aturan. Nama atribut kustom bisa ditemukan dalam direktori dengan menanyakan atribut pengguna menggunakan PowerShell dan mencari nama atribut. Ini juga bisa digunakan saat menyusun aturan dalam sintaks aturan.
4. Pastikan penyewa Anda memiliki lisensi yang sesuai. Grup dinamis mengharuskan penyewa memiliki lisensi Premium Azure AD P1. Daftar paket lisensi Azure AD dapat diakses [di sini](https://azure.microsoft.com/pricing/details/active-directory/). Paket Enterprise Mobility + lisensi keamanan dapat diakses [di sini](https://www.microsoft.com/microsoft-365/enterprise-mobility-security/compare-plans-and-pricing).
5. Pastikan bahwa peran pengguna yang membuat grup dinamis adalah administrator global, Intune administrator, administrator grup, atau administrator pengguna.
6. Berikan waktu untuk grup untuk mengisi. Tergantung pada ukuran penyewa Anda, grup mungkin memakan waktu hingga 24 jam untuk mengisi untuk pertama kalinya atau setelah perubahan aturan.
7. Untuk informasi selengkapnya, lihat [membuat aturan berbasis atribut untuk keanggotaan grup dinamis](https://docs.microsoft.com/azure/active-directory/enterprise-users/groups-dynamic-membership).

**Saya perlu menghapus Grup**

1. Grup dapat dihapus dari direktori menggunakan cmdlet Remove-AzureADGroup dalam modul Azure AD PowerShell.
2. Sebelum mencoba menghapus grup yang disinkronkan di Azure AD, pastikan Anda telah menghapus semua lisensi yang ditetapkan untuk menghindari kesalahan.
3. Untuk informasi selengkapnya tentang menghapus grup, lihat [menghapus grup dengan lisensi yang ditetapkan](https://docs.microsoft.com/azure/active-directory/enterprise-users/licensing-group-advanced#deleting-a-group-with-an-assigned-license).

**Saya perlu memulihkan grup yang dihapus**

1. Jika grup Office 365 dihapus, grup tersebut hanya bisa dipulihkan hingga 30 hari sebelum penghapusan permanen terjadi. Setelah dihapus secara permanen, grup tidak lagi dapat dipulihkan. Pelajari selengkapnya tentang memulihkan grup [di sini](https://docs.microsoft.com/azure/active-directory/enterprise-users/groups-restore-deleted).
2. Fungsi ini tidak didukung untuk grup keamanan dan grup distribusi.
3. Pastikan Anda memiliki wewenang untuk memulihkan grup Office 365. Administrator global, administrator grup, administrator akun pengguna, Intune administrator layanan, mitra Tier1 atau dukungan Tier2, dan pemilik grup bisa memulihkan grup.
4. Saat grup dinamis dihapus dan dipulihkan, grup terlihat sebagai grup baru dan diisi ulang sesuai dengan aturan. Proses ini mungkin memakan waktu hingga 24 jam.
5. Untuk informasi selengkapnya tentang memulihkan grup yang dihapus, lihat [memulihkan grup Office 365 yang dihapus di Azure Active Directory](https://docs.microsoft.com/azure/active-directory/enterprise-users/groups-restore-deleted).

**Konfigurasi kebijakan kedaluwarsa grup**

1. Fungsi ini hanya didukung untuk grup Office 365, dan bukan untuk grup keamanan dan grup distribusi tidak didukung.
2. Mengonfigurasi dan menggunakan kebijakan kedaluwarsa untuk grup Office 365 memerlukan lisensi Azure AD Premium.
3. Saat ini, hanya satu kebijakan kedaluwarsa yang dapat dikonfigurasikan untuk grup Office 365 pada penyewa.
4. Hanya administrator global, administrator grup, administrator pengguna, dan pemilik grup dapat memperpanjang grup.
5. Jika grup Office 365 telah kedaluwarsa, maka akan dihapus dan hanya bisa dipulihkan hingga 30 hari sebelum penghapusan permanen terjadi. Setelah dihapus secara permanen, grup tidak lagi dapat dipulihkan. Pelajari selengkapnya tentang memulihkan grup [di sini](https://docs.microsoft.com/azure/active-directory/enterprise-users/groups-restore-deleted).

**Pembaruan otomatis berbasis aktivitas**

Aktivitas pengguna dari SharePoint, Outlook, dan teams dapat memicu pembaruan otomatis grup. Aktivitas diperiksa pada 35 hari sebelum grup kedaluwarsa. Jika ada aktivitas selama siklus hidup grup saat ini, grup akan otomatis diperbarui dan pemberitahuan email tidak akan dikirim ke pemilik grup.

**Pengaturan waktu pemberitahuan untuk grup kedaluwarsa**

1. Pemberitahuan email dikirim ke pemilik grup Office 365 30 hari, 15 hari, dan 1 hari sebelum berakhirnya grup.
2. Saat Anda pertama kali menyetel kedaluwarsa, grup apa pun yang lebih lama dari interval kedaluwarsa diatur ke 35 hari hingga kedaluwarsa.
3. Tanggal kedaluwarsa grup dihitung berdasarkan tanggal pembaruan grup, bukan berdasarkan tanggal pembaruan kebijakan. Jika kebijakan kedaluwarsa diperbarui, tanggal kedaluwarsa tidak akan berubah.
4. Untuk informasi selengkapnya, lihat, [mengelompokkan kebijakan kedaluwarsa dan memperpanjang email](https://docs.microsoft.com/azure/active-directory/enterprise-users/groups-lifecycle) dan [memulihkan grup Office 365 yang dihapus di Azure Active Directory](https://docs.microsoft.com/azure/active-directory/enterprise-users/groups-restore-deleted).

**Izin untuk membuat grup**

Pastikan bahwa Anda memiliki wewenang untuk membuat grup baru. Administrator global dapat menonaktifkan pembuatan grup di portal Azure atau panel akses. Anda mungkin memerlukan administrator untuk membuat grup baru untuk Anda, atau untuk memberi izin yang sesuai.

1. [Membuat grup baru dan menambahkan anggota di portal Azure](https://docs.microsoft.com/azure/active-directory/fundamentals/active-directory-groups-create-azure-portal)
2. [Membuat grup di PowerShell MSOnline](https://docs.microsoft.com/azure/active-directory/enterprise-users/groups-settings-v2-cmdlets#create-groups)
3. [Menonaktifkan pembuatan grup di PowerShell](https://docs.microsoft.com/azure/active-directory/enterprise-users/groups-settings-v2-cmdlets#disable-group-creation-by-your-users) 
4. [Mengelola siapa yang bisa membuat grup di Office 365](https://docs.microsoft.com/microsoft-365/solutions/manage-creation-of-groups) 
5. [Menonaktifkan pemberitahuan Selamat datang Office 365 melalui PowerShell](https://docs.microsoft.com/powershell/module/exchange/set-unifiedgroup)
6. [Peran administratif Azure AD](https://docs.microsoft.com/azure/active-directory/roles/permissions-reference)

**Mengelola izin pembuatan grup**

1. Administrator global dapat mengelola izin pembuatan grup untuk grup keamanan atau Office 365 yang dibuat di portal Azure atau panel akses, dengan mengatur **pengguna bisa membuat grup keamanan di portal Azure** atau **pengguna bisa membuat grup Office 365 di pengaturan portal Azure** di **semua grup > Umum (pengaturan)**.
2. Anda juga bisa membatasi pembuatan grup untuk memilih grup pengguna jika Anda memiliki lisensi Premium Azure AD P1.

**Menonaktifkan pemberitahuan Selamat datang untuk anggota baru grup Office 365**

Pemberitahuan sambutan yang dikirimkan kepada pengguna yang ditambahkan ke grup Office 365 bisa dinonaktifkan dengan menyetel `UnifiedGroupWelcomeMessageEnabled` ke **false** di PowerShell. Pelajari tentang pengaturan ini [di sini](https://docs.microsoft.com/powershell/module/exchange/set-unifiedgroup).













