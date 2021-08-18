---
title: Aktifkan tulis balik kata sandi di Azure AD Connect
ms.author: pebaum
author: pebaum
manager: scotv
ms.audience: Admin
ms.topic: article
ms.service: o365-administration
ROBOTS: NOINDEX, NOFOLLOW
localization_priority: Priority
ms.collection: Adm_O365
ms.custom:
- "9002933"
- "5615"
ms.openlocfilehash: 63304667cce67c48fd8bbeee52ff6d61d033ea38fd8d4c4d96c240847dab2cab
ms.sourcegitcommit: b5f7da89a650d2915dc652449623c78be6247175
ms.translationtype: MT
ms.contentlocale: id-ID
ms.lasthandoff: 08/05/2021
ms.locfileid: "54118207"
---
# <a name="enable-password-writeback-in-azure-ad-connect"></a>Aktifkan tulis balik kata sandi di Azure AD Connect

Untuk mengaktifkan tulis balik pengaturan ulang kata sandi mandiri, aktifkan terlebih dahulu opsi tulis balik di Azure AD Connect. Dari server Azure AD Connect Anda, lakukan langkah berikut:

1. Masuk ke server Azure AD Connect Anda dan mulai panduan konfigurasi **Azure AD Connect**.
2. Pada halaman **Selamat Datang**, klik **Konfigurasi**.
3. Pada halaman **Tugas tambahan**, pilih **Kustomisasi opsi sinkronisasi**, lalu klik **Lanjut**.
4. Pada halaman **Sambungkan ke Azure AD**, masukkan kredensial administrator global untuk penyewa Azure Anda, lalu klik **Lanjut**.
5. Pada halaman **Sambungkan direktori** dan pemfilteran **Domain/OU**, klik **Lanjut**.
6. Pada halaman **Fitur opsional**, pilih kotak di sebelah **Tulis balik kata sandi** dan klik **Lanjut**.
7. Pada halaman **Siap untuk mengonfigurasi**, klik **Konfigurasi** dan tunggu prosesnya selesai.
8. Saat Anda melihat konfigurasi selesai, klik **Keluar**.

Dengan tulis balik kata sandi diaktifkan di Azure AD Connect, konfigurasikan SSPR Azure AD untuk tulis balik.  Untuk mengaktifkan tulis balik kata sandi di SSPR, lakukan langkah berikut:

1. Masuk ke portal Microsoft Azure dengan menggunakan akun administrator global.
2. Cari dan pilih **Azure Active Directory**, klik **Reset kata sandi**, lalu klik **Integrasi lokal**.
3. Atur opsi untuk **Tulis ulang kata sandi ke direktori lokal Anda?** ke **Ya**.
4. Atur opsi untuk **Izinkan pengguna untuk membuka kunci akun tanpa mereset kata sandi?** ke **Ya**.
5. Jika sudah siap, klik **Simpan**.

Untuk informasi selengkapnya, lihat [Mengaktifkan tulis balik pengaturan ulang kata sandi mandiri Azure Active Directory ke lingkungan lokal](https://docs.microsoft.com/azure/active-directory/authentication/tutorial-enable-sspr-writeback).

> [!NOTE]
>  Saat administrator mereset kata sandi pengguna di Portal Microsoft Azure, jika pengguna tersebut gabungan atau hash kata sandi disinkronkan, kata sandi tersebut akan ditulis ulang ke lokal. Fungsionalitas ini memerlukan Lisensi Azure Premium (P1 atau P2) dan saat ini tidak didukung di portal Admin Office.
