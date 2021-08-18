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
ms.openlocfilehash: 607e27c883f83b4b29347e764b8f2273cf0f117e
ms.sourcegitcommit: ab75f66355116e995b3cb5505465b31989339e28
ms.translationtype: MT
ms.contentlocale: id-ID
ms.lasthandoff: 08/13/2021
ms.locfileid: "58325390"
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

**Catatan**: Ketika administrator mengatur ulang kata sandi pengguna di Portal Azure, jika pengguna tersebut disinkronkan, kata sandi akan ditulis kembali ke hash lokal. Fungsionalitas ini memerlukan Lisensi Azure Premium (P1 atau P2) dan saat ini tidak didukung di portal Admin Office.
