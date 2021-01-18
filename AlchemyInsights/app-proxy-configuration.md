---
title: Konfigurasi proksi aplikasi
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
ms.openlocfilehash: 0b782705afa8eab338687590baff90de4e17ccb9
ms.sourcegitcommit: 83fe2a8d060794fdf58445b469b30a3294b7a9b6
ms.translationtype: MT
ms.contentlocale: id-ID
ms.lasthandoff: 01/15/2021
ms.locfileid: "49885135"
---
# <a name="app-proxy-configuration"></a>Konfigurasi proksi aplikasi

1. Untuk memahami cara mengonfigurasi aplikasi proksi aplikasi dalam Azure AD untuk mengekspos aplikasi lokal Anda ke awan, lihat [cara mengonfigurasi aplikasi proksi aplikasi](https://docs.microsoft.com/azure/active-directory/application-proxy-config-how-to).
2. Masuk tunggal (SSO) memungkinkan pengguna mengakses aplikasi tanpa mengautentikasi beberapa kali. Ini memungkinkan autentikasi tunggal terjadi di awan, berlawanan dengan Azure Active Directory, dan memungkinkan layanan atau konektor untuk meniru pengguna untuk menyelesaikan setiap tantangan autentikasi tambahan dari aplikasi. Untuk mempelajari selengkapnya, lihat [cara mengonfigurasi masuk tunggal ke aplikasi proksi aplikasi](https://docs.microsoft.com/azure/active-directory/application-proxy-config-sso-how-to).
3. Gunakan [artikel ini](https://docs.microsoft.com/azure/active-directory/application-proxy-config-problem) untuk memecahkan masalah umum yang dihadapi orang saat membuat aplikasi proksi aplikasi baru.
4. Jika Anda mengalami masalah saat menyiapkan autentikasi back-end ke aplikasi Anda, Anda mungkin perlu [memecahkan masalah konfigurasi delegasi Kerberos untuk proksi aplikasi](https://docs.microsoft.com/azure/active-directory/application-proxy-back-end-kerberos-constrained-delegation-how-to) atau mengikuti panduan tentang [mengonfigurasi aplikasi dengan pingaccess](https://docs.microsoft.com/azure/active-directory/application-proxy-back-end-ping-access-how-to) untuk mengatasi masalah Anda.
