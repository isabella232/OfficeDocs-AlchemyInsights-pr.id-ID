---
title: Masalah dengan link dan URL
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
- "7720"
- "9004329"
ms.openlocfilehash: 24885d873d6471a72ae66581ad1ceb0a19b664f7
ms.sourcegitcommit: 029c4697b77ce996d41ca74c4fa86de1bb84bd99
ms.translationtype: MT
ms.contentlocale: id-ID
ms.lasthandoff: 01/25/2021
ms.locfileid: "49974467"
---
# <a name="issues-with-links-and-urls"></a>Masalah dengan link dan URL

Redirect URL URI/Reply (kedua ekspresi dapat dipertukarkan) adalah URL yang digunakan oleh platform Microsoft Identity untuk mengembalikan Token yang diminta aplikasi. Untuk informasi tentang URL ini, lihat artikel berikut ini:

- [Alur autentikasi dan skenario aplikasi](https://docs.microsoft.com/azure/active-directory/develop/authentication-flows-app-scenarios) -informasi tentang pengalihan pengalihan di halaman **pendaftaran aplikasi** untuk setiap skenario.
- [Mengarahkan ulang pembatasan URL URI/Balasan](https://docs.microsoft.com/azure/active-directory/develop/reply-url)

**Saya tidak tahu cara mendaftarkan URL Redirect URI/Reply yang tepat untuk aplikasi saya**

Saat Anda masuk dengan aplikasi yang sedang Anda kembangkan, jika dialog masuk menampilkan **AADSTS50011: URL balasan yang ditentukan dalam permintaan tidak cocok dengan URL balasan yang dikonfigurasi untuk aplikasi <your app ID>**, Anda harus menambahkan ke pendaftaran aplikasi Anda, pengalihan URI bahwa kode Anda digunakan dalam permintaan token ke platform Microsoft Identity.

Untuk menambahkan URL Balasan, masuk ke tab **autentikasi** di halaman **pendaftaran aplikasi** Anda di portal Azure dan tambahkan entri di bagian **Alihkan Uris** . Pengalihan URIs diketik (web atau ponsel/desktop). Nilai yang perlu Anda masukkan tergantung pada tipe aplikasi yang sedang Anda gunakan, seperti yang diuraikan di bawah ini:

- Untuk aplikasi Halaman tunggal dan aplikasi web, URL Balasan adalah URL dalam aplikasi Anda. Lihat [registrasi aplikasi satu halaman](https://docs.microsoft.com/azure/active-directory/develop/scenario-spa-app-registration#register-a-redirect-uri) atau [Daftarkan aplikasi aplikasi web menggunakan Azure portal](https://docs.microsoft.com/azure/active-directory/develop/scenario-web-app-sign-user-app-registration?tabs=aspnetcore#register-an-app-using-azure-portal)
- Untuk aplikasi desktop, nilai yang perlu Anda pilih bergantung pada:
    - platform (MacOS berbeda dari Windows atau Linux)
    - cara Anda mendapatkan token (interaktif, dengan alur kode perangkat, dengan autentikasi Windows terpadu [IWA] atau dengan nama pengguna/kata sandi).
    Untuk detailnya, lihat [aplikasi desktop-registrasi aplikasi-redirect URi](https://docs.microsoft.com/azure/active-directory/develop/scenario-desktop-app-registration#redirect-uris)
- Untuk aplikasi seluler, pengalihan URI bergantung pada:
    - platform (iOS/Android/UWP)
    - informasi yang digunakan untuk menyusun aplikasi Anda, seperti ID bundel di iOS, dan nama paket dan hash tanda tangan di aplikasi Azure portal App akan membantu Anda. Untuk detailnya, lihat [konfigurasi platform dan URI pengalihan](https://docs.microsoft.com/azure/active-directory/develop/scenario-mobile-app-registration#platform-configuration-and-redirect-uris).

> [!NOTE]
> Api web dan beberapa cara hening untuk mendapatkan token (IWA dan username/password) tidak memerlukan pengalihan URI.

**Saya telah menggunakan aplikasi web saya dan ketika saya menguji aplikasi yang dikerahkan, saya mendapatkan pesan URL balasan yang tidak cocok**

Tambahkan pengalihan pengalihan untuk semua lokasi di mana Anda menggunakan aplikasi web Anda. Untuk informasi selengkapnya, lihat [mendaftarkan aplikasi Web App menggunakan Azure portal](https://docs.microsoft.com/azure/active-directory/develop/scenario-web-app-sign-user-app-registration).

> [!NOTE]
> Tambahkan pengalihan URI untuk lokasi segera setelah Anda menyebarkan aplikasi di lokasi tersebut.

**Saya tidak dapat mendaftarkan cukup URL Balasan**

Anda adalah ISV dan memiliki satu atau beberapa pengalihan pengalihan untuk setiap pelanggan Anda. Anda ingin melakukan migrasi dari ADAL/Azure AD v 1.0 ke MSAL/platform identitas Microsoft dan Anda menekan [jumlah maksimum pengalihan URIs](https://docs.microsoft.com/azure/active-directory/develop/reply-url#maximum-number-of-redirect-uris). Untuk mengatasi masalah ini, [Tambahkan URI pengalihan ke prinsip Layanan](https://docs.microsoft.com/azure/active-directory/develop/reply-url#add-redirect-uris-to-service-principals) yang sesuai untuk masing-masing pelanggan Anda.
