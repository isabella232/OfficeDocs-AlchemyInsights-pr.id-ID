---
title: Masalah masuk pengguna SSO yang mulus
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
- "9004357"
- "7811"
ms.openlocfilehash: 347ef8f8176583f2a7c15fa82435eeb118b58c39
ms.sourcegitcommit: 67c873fa6e23ec39a826d60ac830969073bf79e1
ms.translationtype: MT
ms.contentlocale: id-ID
ms.lasthandoff: 01/21/2021
ms.locfileid: "49935172"
---
# <a name="seamless-sso-user-sign-in-issues"></a>Masalah masuk pengguna SSO yang mulus

Setelah pengguna diautentikasi, browser akan menyimpan kredensial pengguna, sehingga di browser yang sama, aplikasi akan masuk secara otomatis dengan akun yang sama. Ini mungkin menyulitkan pengguna lain atau satu pengguna untuk masuk ke beberapa akun di satu perangkat. Untuk mengatasi masalah ini: 1. Coba masuk di browser lain. 2. Kosongkan tembolok dan/atau cookie browser dan coba masuk lagi.

Jika Anda masih mengalami masalah masuk, kami merekomendasikan hal berikut ini untuk mendiagnosis dan mengotomatisasi langkah-langkah pemecahan masalah:

1. Instal [ekstensi browser aman aplikasi saya](https://docs.microsoft.com/azure/active-directory/manage-apps/access-panel-extension-problem-installing) untuk membantu Azure Active Directory (Azure AD) untuk menyediakan diagnosis dan resolusi yang lebih baik ketika menggunakan pengalaman uji coba di portal Azure.
2. Mereproduksi kesalahan menggunakan pengalaman uji dalam halaman konfigurasi aplikasi di Azure portal. Untuk mempelajari selengkapnya, lihat [debug aplikasi masuk tunggal berbasis SAML](https://docs.microsoft.com/azure/active-directory/azuread-dev/howto-v1-debug-saml-sso-issues).
3. Jika Anda menggunakan pengalaman uji coba di portal Azure dengan ekstensi browser aman aplikasi saya, Anda bisa **melewati langkah 4**.
4. Untuk membuka halaman konfigurasi masuk tunggal berbasis SAML:
    - Buka [portal Azure](https://portal.azure.com/) dan masuk sebagai **administrator global** atau **coadmin**.
    - Buka **ekstensi direktori aktif Azure** dengan memilih **semua layanan** di bagian atas menu navigasi sisi kiri utama.
    - Ketikkan "Azure Active Directory" dalam kotak pencarian filter dan pilih item **Azure Active Directory** .
    - Pilih **aplikasi Enterprise** dari menu navigasi kiri Azure Active Directory.
    - Pilih **semua aplikasi** untuk menampilkan daftar semua aplikasi Anda. Jika Anda tidak melihat aplikasi yang Anda inginkan muncul di sini, Gunakan kontrol **filter** di bagian atas **Daftar semua aplikasi** dan atur opsi **Perlihatkan** ke **semua aplikasi**.
    - Pilih aplikasi yang ingin Anda konfigurasi untuk masuk tunggal.
    - Setelah aplikasi dimuat, pilih **masuk tunggal** dari menu navigasi sebelah kiri aplikasi.
    - Pilih **SSO berbasis SAML**.
5. Berdasarkan kesalahan tersebut, untuk mempelajari selengkapnya tentang langkah-langkah yang dianjurkan untuk diikuti, lihat [masalah masuk ke aplikasi yang dikonfigurasi tunggal berbasis SAML](https://docs.microsoft.com/azure/active-directory/manage-apps/application-sign-in-problem-federated-sso-gallery#application-not-found-in-directory).
6. Untuk memecahkan masalah masuk pengguna lainnya rujuk ke panduan berikut ini:
    - [Protokol SAML Sign-On tunggal](https://docs.microsoft.com/azure/active-directory/develop/single-sign-on-saml-protocol)
    - [Cara: memecahkan masalah kesalahan masuk menggunakan laporan direktori aktif Azure](https://docs.microsoft.com/azure/active-directory/reports-monitoring/howto-troubleshoot-sign-in-errors)
    - [Perintah persetujuan yang tidak diharapkan](https://docs.microsoft.com/azure/active-directory/manage-apps/application-sign-in-unexpected-user-consent-prompt)
    - [Kesalahan persetujuan pengguna](https://docs.microsoft.com/azure/active-directory/manage-apps/application-sign-in-unexpected-user-consent-error)
    - [Masalah masuk dari aplikasi saya](https://docs.microsoft.com/azure/active-directory/manage-apps/application-sign-in-other-problem-access-panel)
    - [Kesalahan pada halaman masuk aplikasi](https://docs.microsoft.com/azure/active-directory/manage-apps/application-sign-in-problem-application-error)
    - [Masalah masuk ke aplikasi Microsoft](https://docs.microsoft.com/azure/active-directory/manage-apps/application-sign-in-problem-first-party-microsoft)
