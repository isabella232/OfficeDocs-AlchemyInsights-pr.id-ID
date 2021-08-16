---
title: Mengonfigurasi dan mengkustomisasi aplikasi
ms.author: v-jmathew
author: v-jmathew
manager: scotv
ms.audience: Admin
ms.topic: article
ms.service: o365-administration
ROBOTS: NOINDEX, NOFOLLOW
localization_priority: Normal
ms.collection: Adm_O365
ms.custom:
- "9004334"
- "7733"
ms.openlocfilehash: 3ce5b04469eb655c9d682f5830d9f906529aa40f706ee594b670708426d48769
ms.sourcegitcommit: b5f7da89a650d2915dc652449623c78be6247175
ms.translationtype: MT
ms.contentlocale: id-ID
ms.lasthandoff: 08/05/2021
ms.locfileid: "54044991"
---
# <a name="configure-and-customize-applications"></a>Mengonfigurasi dan mengkustomisasi aplikasi

**Mengonfigurasi Aplikasi**

1. [Mulai cepat: Mengonfigurasi properti untuk aplikasi di penyewa Azure Active Directory (Azure AD)](https://docs.microsoft.com/azure/active-directory/manage-apps/add-application-portal-configure) memperlihatkan cara mengonfigurasi beberapa properti untuk aplikasi.
2. Untuk membantu mengintegrasikan aplikasi Azure Active Directory Anda, kami [telah mengembangkan kumpulan tutorial yang](https://docs.microsoft.com/azure/active-directory/saas-apps/tutorial-list) akan memandu Anda melalui konfigurasi.
3. [Cara mengonfigurasi aplikasi Proksi Aplikasi](https://docs.microsoft.com/azure/active-directory/manage-apps/application-proxy-config-how-to) membantu Memahami cara mengonfigurasi aplikasi Proksi Aplikasi dalam Azure AD untuk mengekspos aplikasi lokal ke awan.
4. [Unduh PingAccess dan konfigurasi](https://docs.microsoft.com/azure/active-directory/manage-apps/application-proxy-ping-access-publishing-guide#download-pingaccess-and-configure-your-application)aplikasi Anda : Ikuti instruksi dalam *Mengonfigurasi PingAccess* untuk Azure AD untuk memproteksi aplikasi yang diterbitkan menggunakan Microsoft Azure AD Application Proxy di situs web Identitas Ping dan mengunduh versi terbaru PingAccess.

**Kesalahan aplikasi yang dikonfigurasi dengan salah (AADSTS650056)**

1. Pastikan Anda mengakses aplikasi dari alamat masuk yang disediakan oleh pemilik aplikasi. Jika tidak, masuk ke aplikasi melalui proses normal. Dalam banyak kasus ini akan diatasi secara otomatis. Jika tidak, postingan ini dapat membantu memecahkan masalah dan mengatasinya.
2. **Jika organisasi Anda memiliki aplikasi (yang** berarti pendaftaran aplikasi ada di organisasi Anda):
    - Setidaknya, kami merekomendasikan izin `User.Read` `openid` atau izin yang didelegasikan **dari Microsoft Graph** ditambahkan.
    - Pastikan aplikasi dan semua izinnya telah setuju. Anda bisa memverifikasi ini dengan melihat **kolom Status** dari pendaftaran Aplikasi dalam **Izin API.**
    - Dalam beberapa skenario, aplikasi mungkin merupakan pihak ketiga, namun dapat didaftarkan di organisasi Anda. Konfirmasi apakah aplikasi ini tercantum dalam pendaftaran Aplikasi Anda (aplikasi Bukan Perusahaan).
    - Jika Anda terus melihat pesan kesalahan ini. Lalu Anda mungkin perlu menyusun URL persetujuan yang diuraikan di **langkah 4**.
3. **Jika organisasi Anda bukan pemilik aplikasi dan menggunakannya sebagai aplikasi pihak ketiga:**
    - Jika Anda adalah administrator Global/Perusahaan, Anda akan melihat layar persetujuan. Pastikan Anda mencentang kotak **"Persetujuan atas nama organisasi Anda"**.
    - Jika Anda tidak melihat layar persetujuan, hapus aplikasi Enterprise, dan coba lagi.
    - Jika Anda terus melihat pesan kesalahan ini. Lalu Anda mungkin perlu menyusun URL persetujuan yang diuraikan di **langkah 4**.
4. **Buat URL** persetujuan secara manual untuk digunakan: Jika aplikasi didesain untuk mengakses sumber daya tertentu, Anda mungkin tidak dapat menggunakan tombol Persetujuan dari portal Azure, Anda harus membuat URL persetujuan Anda sendiri secara manual dan menggunakan ini.
    - Anda perlu mendapatkan dan `{App-Id}` pemilik `{App-Uri-Id}` aplikasi. `{Tenant-Id}` akan menjadi pengidentifikasi penyewa Anda. Ini akan menjadi `yourdomain.onmicrosoft.com` ID direktori Anda.
    - Jika aplikasi mengakses sendiri untuk sumber daya, maka dan `{App-Id}` `{App-Uri-Id}` akan sama.
5. Untuk informasi selengkapnya, lihat Masalah masuk ke aplikasi tunggal yang dikonfigurasi berbasis [SAML.](https://docs.microsoft.com/azure/active-directory/manage-apps/application-sign-in-problem-federated-sso-gallery#misconfigured-application)

**Mengustomisasi Aplikasi**

- [Menambahkan pencitraan](https://docs.microsoft.com/azure/active-directory/fundamentals/customize-branding) ke halaman masuk Azure Active Directory organisasi Anda - Gunakan logo dan skema warna kustom organisasi Anda untuk memberikan tampilan dan nuansa yang konsisten untuk halaman masuk Azure Active Directory (Azure AD).
- [Menambahkan nama domain kustom Anda menggunakan portal Azure Active Directory](https://docs.microsoft.com/azure/active-directory/fundamentals/add-custom-domain) - Setiap penyewa Azure AD yang baru dilengkapi dengan nama domain awal. Anda tidak bisa mengubah atau menghapus nama domain awal, tapi Anda bisa menambahkan nama organisasi Anda. Menambahkan nama domain kustom membantu Anda membuat nama pengguna yang sudah tidak asing lagi bagi pengguna Anda.
