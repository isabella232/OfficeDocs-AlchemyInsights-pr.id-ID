---
title: Konfigurasi Proksi Aplikasi
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
- "9004356"
- "7800"
ms.openlocfilehash: 835bfc59f77b31dc9a37c98db911505e2c7a758b37406dfc4da2d139afa61db5
ms.sourcegitcommit: b5f7da89a650d2915dc652449623c78be6247175
ms.translationtype: MT
ms.contentlocale: id-ID
ms.lasthandoff: 08/05/2021
ms.locfileid: "53951568"
---
# <a name="app-proxy-configuration"></a>Konfigurasi Proksi Aplikasi

1. Untuk memahami cara mengonfigurasi aplikasi Proksi Aplikasi dalam Azure AD untuk mengekspos aplikasi lokal ke awan, lihat Cara mengonfigurasi [aplikasi Proksi Aplikasi](https://docs.microsoft.com/azure/active-directory/application-proxy-config-how-to).
2. Masuk tunggal (SSO, Single sign-on) memungkinkan pengguna Anda mengakses aplikasi tanpa mengotentikan beberapa kali. Ini memungkinkan autentikasi tunggal terjadi di awan, terhadap Azure Active Directory, dan memungkinkan layanan atau Konektor meniru pengguna untuk menyelesaikan tantangan autentikasi tambahan apa pun dari aplikasi. Untuk mempelajari selengkapnya, [lihat Cara mengonfigurasi masuk tunggal ke aplikasi Proksi Aplikasi](https://docs.microsoft.com/azure/active-directory/application-proxy-config-sso-how-to).
3. Gunakan [artikel ini](https://docs.microsoft.com/azure/active-directory/application-proxy-config-problem) untuk memecahkan masalah umum yang dihadapi orang-orang saat membuat aplikasi proksi aplikasi baru.
4. Jika mengalami masalah dalam menyiapkan autentikasi ujung-belakang untuk aplikasi, Anda mungkin perlu Memecahkan masalah konfigurasi delegasi [Kerberos](https://docs.microsoft.com/azure/active-directory/application-proxy-back-end-kerberos-constrained-delegation-how-to) yang dibatasi untuk Proksi Aplikasi atau mengikuti panduan tentang mengonfigurasi aplikasi dengan [PingAccess](https://docs.microsoft.com/azure/active-directory/application-proxy-back-end-ping-access-how-to) untuk mengatasi masalah Anda.
