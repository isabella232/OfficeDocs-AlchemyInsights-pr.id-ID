---
title: Privileged Identity Management peran
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
- "9003230"
- "6825"
ms.openlocfilehash: 358e446192e6b58ace81afa06e0d65ae3a207282351ffc3ec9975a24779951fb
ms.sourcegitcommit: b5f7da89a650d2915dc652449623c78be6247175
ms.translationtype: MT
ms.contentlocale: id-ID
ms.lasthandoff: 08/05/2021
ms.locfileid: "53973232"
---
# <a name="privileged-identity-managementpim-role"></a>Privileged Identity Management(SLOW)

**Izin tidak diberikan setelah mengaktifkan peran**

Saat Anda mengaktifkan peran di Azure AD Privileged Identity Management (AZURE), aktivasi mungkin tidak langsung dis propagate ke semua portal yang memerlukan peran istimewa. Terkadang, meskipun perubahan disebarkan, caching web di portal mungkin mengakibatkan perubahan yang tidak langsung berpengaruh.

Jika aktivasi Anda tertunda, ikuti langkah-langkah berikut:

1. Keluar dari portal Azure, lalu masuk kembali. Ketika mengaktifkan peran Azure AD atau peran sumber daya Azure, Anda akan melihat tahapan aktivasi Anda. Setelah semua tahapan selesai, Anda akan melihat link 'Keluar'. Anda dapat menggunakan tautan ini untuk keluar. Hal ini akan mengatasi sebagian besar kasus penundaan aktivasi.
2. DiDAFTAR, verifikasi bahwa Anda terdaftar sebagai anggota peran.
3. Jika Anda mengaktifkan peran Exchange Administrator, pastikan Anda keluar dan masuk kembali. Jika masalah tetap ada, buka tiket dukungan dan naikkan hal ini sebagai masalah. Jika Anda menggunakan peran Exchange Administrator untuk mengakses Pusat Keamanan dan Kepatuhan, lihat langkah berikutnya.
4. Jika Anda mengaktifkan sebuah peran untuk mengakses Pusat Keamanan dan Kepatuhan atau jika Anda mengaktifkan peran Administrator SharePoint, Anda akan mengalami beberapa penundaan aktivasi dari beberapa menit hingga beberapa jam. Ini adalah masalah umum dan kami sedang bekerja sama dengan tim ini secara aktif untuk menyelesaikan masalah ini sesegera mungkin.

Untuk informasi selengkapnya, lihat:

- [Mengaktifkan peran Azure AD saya di AZURE](https://docs.microsoft.com/azure/active-directory/privileged-identity-management/pim-how-to-activate-role?WT.mc_id=Portal-Microsoft_Azure_Support "https://docs.microsoft.com/azure/active-directory/privileged-identity-management/pim-how-to-activate-role?wt.mc_id=portal-microsoft_azure_support")
- [Mengaktifkan peran sumber daya Azure saya di AZURE](https://docs.microsoft.com/azure/active-directory/privileged-identity-management/pim-resource-roles-activate-your-roles?WT.mc_id=Portal-Microsoft_Azure_Support "https://docs.microsoft.com/azure/active-directory/privileged-identity-management/pim-resource-roles-activate-your-roles?wt.mc_id=portal-microsoft_azure_support")

**Izin tidak dihapus setelah menonaktifkan peran atau aktivasi peran kedaluwarsa**

Saat Anda menonaktifkan peran di Azure AD Privileged Identity Management atau saat periode aktivasi peran kedaluwarsa, mungkin ada penundaan di mana Anda terus memiliki akses.

Jika penonaktifan Anda tertunda, ikuti langkah-langkah ini:

1. Jika Anda menonaktifkan peran Administrator Exchange atau periode aktivasi peran kedaluwarsa, dan melihat adanya penundaan yang signifikan sebelum izin dihapus, buka tiket dukungan dan beri tahu teknisi dukungan Anda untuk membantu Anda mengarmuterka tiket dengan tim Manajemen Akses Hak Istimewa (PAM) di Office tentang masalah ini.
2. Jika periode aktivasi telah kedaluwarsa, tapi Anda masih membuka sesi browser, tutup browser Anda. Anda dapat terus menggunakan peran hingga Anda menutup sesi itu. Ini adalah masalah yang telah diketahui dan kami sedang mencari kemungkinan perbaikan untuk mencabut setiap sesi secara aktif setelah aktivasi telah kedaluwarsa.

Jika penundaan Anda berbeda dari dua skenario ini, silakan buka tiket dukungan.
