---
title: Memecahkan masalah akses masuk tunggal (SSO) berbasis kata sandi
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
ms.openlocfilehash: 4a9163f199a505df9b2de4f02b7c37a5f5677022
ms.sourcegitcommit: 0eb4f9bde53395b5fd4b5cd4ffc56ca96db91298
ms.translationtype: MT
ms.contentlocale: id-ID
ms.lasthandoff: 03/10/2021
ms.locfileid: "50714771"
---
# <a name="troubleshoot-password-based-seamless-single-sign-on-sso-issues"></a>Memecahkan masalah akses masuk tunggal (SSO) berbasis kata sandi

Untuk mempelajari dasar-dasar SSO berbasis kata sandi, lihat [autentikasi berbasis kata sandi dengan Azure Active Directory](https://docs.microsoft.com/azure/active-directory/fundamentals/auth-password-based-sso).

**Mengonfigurasi SSO berbasis kata sandi**

1. [Konfigurasi akses masuk tunggal berbasis kata sandi](https://docs.microsoft.com/azure/active-directory/manage-apps/configure-password-single-sign-on-non-gallery-applications) -artikel ini MEMBAHAS opsi SSO berbasis kata sandi. Jika aplikasi yang Anda tambahkan memerlukan konfigurasi kustom dan Anda perlu menggunakan SSO berbasis kata sandi, maka artikel ini ditujukan untuk Anda.
2. [Konfigurasi single sign-on berbasis kata sandi untuk aplikasi di prem](https://docs.microsoft.com/azure/active-directory/manage-apps/application-proxy-configure-single-sign-on-password-vaulting) -proksi aplikasi mendukung beberapa mode masuk tunggal. Masuk berbasis kata sandi ditujukan untuk aplikasi yang menggunakan kombinasi nama pengguna/kata sandi untuk autentikasi. Saat Anda mengonfigurasi masuk berbasis kata sandi untuk aplikasi Anda, pengguna Anda harus masuk ke aplikasi di tempat satu kali. Setelah itu, Azure Active Directory menyimpan informasi masuk dan secara otomatis menyediakannya ke aplikasi saat pengguna Anda mengaksesnya dari jarak jauh.
    - Anda harus sudah menerbitkan dan menguji aplikasi Anda dengan proksi aplikasi. Jika tidak, ikuti langkah-langkah dalam [menerbitkan aplikasi menggunakan proksi aplikasi AZURE AD](https://docs.microsoft.com/azure/active-directory/manage-apps/application-proxy-add-on-premises-application) lalu Lanjutkan konfigurasi SSO berbasis kata sandi untuk aplikasi di prem.

Untuk memecahkan masalah SSO berbasis kata sandi, lihat [memecahkan masalah masuk tunggal berbasis kata sandi di AZURE AD](https://docs.microsoft.com/azure/active-directory/manage-apps/troubleshoot-password-based-sso)
