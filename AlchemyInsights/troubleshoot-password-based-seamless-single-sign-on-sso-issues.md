---
title: Memecahkan masalah Masuk Tunggal Tanpa Hambatan (SSO, Seamless Single Sign-on) berbasis kata sandi
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
- "9004357"
- "9374"
ms.openlocfilehash: 6b4d7335461c913a6b5f782756684c5526a96c58c44853ddf9154aa51607bd4a
ms.sourcegitcommit: b5f7da89a650d2915dc652449623c78be6247175
ms.translationtype: MT
ms.contentlocale: id-ID
ms.lasthandoff: 08/05/2021
ms.locfileid: "53972827"
---
# <a name="troubleshoot-password-based-seamless-single-sign-on-sso-issues"></a>Memecahkan masalah Masuk Tunggal Tanpa Hambatan (SSO, Seamless Single Sign-on) berbasis kata sandi

Untuk mempelajari [dasar-dasar](https://docs.microsoft.com/azure/active-directory/fundamentals/auth-password-based-sso)SSO berbasis kata sandi, lihat Autentikasi berbasis kata sandi dengan Azure Active Directory .

**Mengonfigurasi SSO berbasis kata sandi**

1. [Mengonfigurasi akses masuk tunggal berbasis kata sandi](https://docs.microsoft.com/azure/active-directory/manage-apps/configure-password-single-sign-on-non-gallery-applications) - Artikel ini menjelaskan opsi SSO berbasis kata sandi ke detail selengkapnya. Jika aplikasi yang Anda tambahkan memerlukan konfigurasi kustom dan Anda harus menggunakan SSO berbasis kata sandi, artikel ini tepat untuk Anda.
2. [Mengonfigurasi akses masuk tunggal berbasis kata sandi untuk aplikasi on-prem](https://docs.microsoft.com/azure/active-directory/manage-apps/application-proxy-configure-single-sign-on-password-vaulting) - Proksi Aplikasi mendukung beberapa mode masuk tunggal. Akses masuk berbasis kata sandi ditujukan untuk aplikasi yang menggunakan kombinasi nama pengguna/kata sandi untuk autentikasi. Saat mengonfigurasi masuk berbasis kata sandi untuk aplikasi, pengguna harus masuk sekali ke aplikasi lokal. Setelah itu, Azure Active Directory menyimpan informasi masuk dan secara otomatis menyediakannya ke aplikasi saat pengguna Anda mengaksesnya dari jarak jauh.
    - Seharusnya Anda sudah menerbitkan dan menguji aplikasi Anda dengan Proksi Aplikasi. Jika belum, ikuti langkah-langkah dalam Menerbitkan aplikasi menggunakan Proksi Aplikasi [Azure AD](https://docs.microsoft.com/azure/active-directory/manage-apps/application-proxy-add-on-premises-application) lalu lanjutkan konfigurasi SSO berbasis kata sandi untuk aplikasi sesuai kebutuhan.

Untuk memecahkan masalah SSO berbasis kata sandi, [lihat Memecahkan masalah masuk tunggal berbasis kata sandi di Azure AD](https://docs.microsoft.com/azure/active-directory/manage-apps/troubleshoot-password-based-sso)
