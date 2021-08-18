---
title: Masalah pada tautan dan URL
ms.author: v-smandalika
author: v-smandalika
manager: dansimp
ms.date: 02/25/2021
ms.audience: Admin
ms.topic: article
ms.service: o365-administration
ROBOTS: NOINDEX, NOFOLLOW
localization_priority: Priority
ms.collection: Adm_O365
ms.custom:
- "7720"
- "9004329"
ms.openlocfilehash: d85069970fe6bc6cc7a8488c49c0e6236426d45b
ms.sourcegitcommit: ab75f66355116e995b3cb5505465b31989339e28
ms.translationtype: MT
ms.contentlocale: id-ID
ms.lasthandoff: 08/13/2021
ms.locfileid: "58321910"
---
# <a name="issues-with-links-and-urls"></a>Masalah pada tautan dan URL

URI pengalihan/URL balasan (kedua ekspresi dapat dipertukarkan) adalah URL yang digunakan oleh platform identitas Microsoft untuk menampilkan token yang diminta aplikasi. Untuk informasi tentang URL tersebut, lihat artikel berikut:

- [Aliran autentikasi dan skenario aplikasi](https://docs.microsoft.com/azure/active-directory/develop/authentication-flows-app-scenarios) - Informasi mengenai URI pengalihan di halaman **Pendaftaran aplikasi** untuk setiap skenario.
- [Pembatasan dan batasan URI pengalihan/URL balasan](https://docs.microsoft.com/azure/active-directory/develop/reply-url)

**Saya tidak tahu cara mendaftarkan URI pengalihan/URL balasan yang benar untuk aplikasi saya**

Saat masuk dengan aplikasi yang Anda kembangkan, jika dialog masuk menampilkan **AADSTS50011: URL balasan yang ditentukan dalam permintaan tidak cocok dengan URL balasan yang dikonfigurasi untuk aplikasi <your app ID>**, Anda perlu menambahkan URI pengalihan yang digunakan kode Anda dalam permintaan token ke platform identitas Microsoft ke pendaftaran aplikasi Anda.

Untuk menambahkan URL balasan, buka tab **Autentikasi** di halaman **pendaftaran aplikasi** Anda di portal Microsoft Azure, lalu tambahkan entri di bagian **URI Pengalihan**. Nilai yang perlu Anda masukkan bergantung pada tipe aplikasi yang Anda buat, seperti yang dijelaskan di bawah ini:

- Untuk aplikasi satu halaman dan aplikasi web, URL balasannya adalah URL di aplikasi Anda. Lihat [Pendaftaran aplikasi satu halaman](https://docs.microsoft.com/azure/active-directory/develop/scenario-spa-app-registration#register-a-redirect-uri) atau [Mendaftarkan aplikasi web menggunakan portal Microsoft Azure](https://docs.microsoft.com/azure/active-directory/develop/scenario-web-app-sign-user-app-registration?tabs=aspnetcore#register-an-app-using-azure-portal)
- Untuk aplikasi desktop, nilai yang perlu Anda pilih bergantung pada:
    - platform (MacOS berbeda dengan Windows atau Linux)
    - cara Anda memperoleh token (secara interaktif, dengan alur kode perangkat, dengan Autentikasi Windows Terpadu [IWA] atau dengan nama pengguna/kata sandi).
    Untuk detailnya, lihat [Aplikasi desktop - Pendaftaran aplikasi - URI Pengalihan](https://docs.microsoft.com/azure/active-directory/develop/scenario-desktop-app-registration#redirect-uris)
- Untuk aplikasi seluler, URI pengalihan bergantung pada:
    - platform (iOS/Android/UWP)
    - informasi yang digunakan untuk membangun aplikasi Anda, seperti ID bundel di iOS, dan nama paket serta hash tanda tangan di Android Pendaftaran aplikasi portal Microsoft Azure akan membantu Anda. Untuk detailnya, lihat [Konfigurasi platform dan URI pengalihan](https://docs.microsoft.com/azure/active-directory/develop/scenario-mobile-app-registration#platform-configuration-and-redirect-uris).

**Catatan**: API Web dan beberapa cara diam-diam mendapatkan token (IWA dan nama pengguna/kata sandi) tidak memerlukan URI pengalihan.

**Saya telah menyebarkan aplikasi web saya dan ketika saya mengujinya, saya mendapatkan pesan ketidakcocokan url balasan**

Tambahkan URI pengalihan untuk semua lokasi tempat Anda menyebarkan aplikasi web. Untuk informasi selengkapnya, lihat [Mendaftarkan aplikasi web menggunakan portal Microsoft Azure](https://docs.microsoft.com/azure/active-directory/develop/scenario-web-app-sign-user-app-registration).

**Catatan**: Menambahkan URI pengalihan untuk lokasi segera setelah Anda menggunakan aplikasi di lokasi tersebut.

**Saya tidak bisa mendaftarkan cukup URL balasan**

Anda merupakan ISV dan memiliki satu atau beberapa URI pengalihan untuk setiap pelanggan Anda. Anda ingin melakukan migrasi dari ADAL/Azure AD v1.0 ke MSAL/platform identitas Microsoft dan Anda menekan [jumlah maksimal URI pengalihan](https://docs.microsoft.com/azure/active-directory/develop/reply-url#maximum-number-of-redirect-uris). Untuk mengatasi ini, [tambahkan URI pengalihan ke layanan utama](https://docs.microsoft.com/azure/active-directory/develop/reply-url#add-redirect-uris-to-service-principals) yang sesuai dengan setiap pelanggan Anda.
