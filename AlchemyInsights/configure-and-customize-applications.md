---
title: Mengonfigurasi dan mengustomisasi aplikasi
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
ms.openlocfilehash: 30127beda85dd9824f7e3a7a4744d109e7ea874b
ms.sourcegitcommit: aeb15e206865f61ff61a1e55c407e34eaa89b6d1
ms.translationtype: MT
ms.contentlocale: id-ID
ms.lasthandoff: 01/29/2021
ms.locfileid: "50063656"
---
# <a name="configure-and-customize-applications"></a>Mengonfigurasi dan mengustomisasi aplikasi

**Mengonfigurasi aplikasi**

1. [Mulai cepat: mengonfigurasi properti untuk aplikasi di penyewa Azure Active Directory (AZURE AD) Anda](https://docs.microsoft.com/azure/active-directory/manage-apps/add-application-portal-configure) memperlihatkan cara mengonfigurasi beberapa properti untuk aplikasi.
2. Untuk membantu mengintegrasikan aplikasi Anda dengan Azure Active Directory, kami telah mengembangkan [kumpulan tutorial](https://docs.microsoft.com/azure/active-directory/saas-apps/tutorial-list) yang memandu Anda melalui konfigurasi.
3. [Cara mengonfigurasi aplikasi proksi aplikasi](https://docs.microsoft.com/azure/active-directory/manage-apps/application-proxy-config-how-to) membantu Anda memahami cara mengonfigurasi aplikasi proksi aplikasi dalam Azure AD untuk mengekspos aplikasi lokal Anda ke awan.
4. [Unduh pingaccess dan konfigurasikan aplikasi Anda](https://docs.microsoft.com/azure/active-directory/manage-apps/application-proxy-ping-access-publishing-guide#download-pingaccess-and-configure-your-application): Ikuti instruksi di *mengonfigurasi Pingaccess untuk Azure AD untuk memproteksi aplikasi* yang diterbitkan menggunakan PROKSI aplikasi Microsoft Azure AD di situs web ping Identity dan mengunduh versi terbaru pingaccess.

**Kesalahan aplikasi misconfigured (AADSTS650056)**

1. Pastikan Anda mengakses aplikasi dari alamat masuk yang disediakan oleh pemilik aplikasi. Jika artinya, masuk ke aplikasi melalui proses normalnya. Dalam kebanyakan kasus ini akan secara otomatis mengatasi secara alami. Jika tidak, maka postingan ini bisa membantu memecahkan masalah dan mengatasinya.
2. **Jika organisasi Anda memiliki aplikasi** (yang berarti pendaftaran aplikasi ada di organisasi Anda):
    - Minimal, kami merekomendasikan `User.Read` `openid` izin atau delegasi dari **Microsoft graph** .
    - Pastikan aplikasi dan semua izinnya telah disetujui. Anda dapat memverifikasi ini dengan melihat kolom **status** dari pendaftaran aplikasi dalam **izin api**.
    - Dalam beberapa skenario, aplikasi mungkin merupakan pihak ketiga namun mungkin didaftarkan di organisasi Anda. Konfirmasi jika aplikasi ini tercantum dalam pendaftaran aplikasi Anda (bukan aplikasi perusahaan).
    - Jika Anda masih melihat pesan kesalahan ini. Maka Anda mungkin perlu menyusun URL persetujuan yang diuraikan di **langkah 4**.
3. **Jika organisasi Anda bukan pemilik aplikasi dan menggunakannya sebagai aplikasi pihak ketiga**:
    - Jika Anda adalah administrator global/perusahaan, Anda akan melihat layar persetujuan. Pastikan Anda mencentang kotak **"persetujuan atas nama organisasi Anda"**.
    - Jika Anda tidak melihat layar persetujuan, Hapus aplikasi perusahaan, dan coba lagi.
    - Jika Anda masih melihat pesan kesalahan ini. Maka Anda mungkin perlu menyusun URL persetujuan yang diuraikan di **langkah 4**.
4. Secara **manual buat URL persetujuan yang akan digunakan**: jika aplikasi dirancang untuk mengakses sumber daya tertentu, Anda mungkin tidak dapat menggunakan tombol persetujuan dari portal Azure, Anda harus membuat URL persetujuan Anda sendiri secara manual dan menggunakannya.
    - Anda akan perlu mendapatkan `{App-Id}` dan `{App-Uri-Id}` dari pemilik aplikasi. `{Tenant-Id}` akan menjadi pengidentifikasi penyewa Anda. Ini akan berupa `yourdomain.onmicrosoft.com` atau id direktori Anda.
    - Jika aplikasi mengakses sendiri untuk sumber daya, maka `{App-Id}` dan `{App-Uri-Id}` akan sama.
5. Untuk informasi selengkapnya, lihat [masalah masuk ke SAML-based single sign-on aplikasi yang dikonfigurasi](https://docs.microsoft.com/azure/active-directory/manage-apps/application-sign-in-problem-federated-sso-gallery#misconfigured-application).

**Mengkustomisasi aplikasi**

- [Menambahkan pencitraan merek ke halaman masuk direktori Azure Active Directory Anda](https://docs.microsoft.com/azure/active-directory/fundamentals/customize-branding) -Gunakan logo dan skema warna kustom organisasi Anda untuk menyediakan tampilan dan nuansa yang konsisten ke halaman masuk Azure Active Directory (Azure AD) Anda.
- [Tambahkan nama domain kustom Anda menggunakan portal Azure Active Directory](https://docs.microsoft.com/azure/active-directory/fundamentals/add-custom-domain) -setiap penyewa Azure AD baru hadir dengan nama domain awal. Anda tidak bisa mengubah atau menghapus nama domain awal, tapi Anda bisa menambahkan nama organisasi Anda. Menambahkan nama domain kustom membantu Anda membuat nama pengguna yang sudah familiar untuk pengguna Anda.
