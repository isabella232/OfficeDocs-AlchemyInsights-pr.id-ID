---
title: Peran manajemen identitas istimewa
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
ms.openlocfilehash: 726511d016462f56c48a4272b57abc3e9f0cbc3d
ms.sourcegitcommit: 35e2c122d8a838d98d1f0851c29b16282261580f
ms.translationtype: MT
ms.contentlocale: id-ID
ms.lasthandoff: 11/17/2020
ms.locfileid: "49088881"
---
# <a name="privileged-identity-managementpim-role"></a>Peran manajemen identitas istimewa (PIM)

**Izin tidak diberikan setelah mengaktifkan peran**

Saat Anda mengaktifkan peran di Azure AD Privileged Management (PIM), aktivasi mungkin tidak langsung dialihkan ke semua portal yang memerlukan peran istimewa. Terkadang, meskipun perubahan disebarkan, caching web di portal mungkin mengakibatkan perubahan tidak berpengaruh dengan segera.

Jika aktivasi tertunda, ikuti langkah-langkah berikut:

1. Keluar dari Azure portal lalu masuk kembali. Saat Anda mengaktifkan peran Azure AD atau peran sumber daya Azure, Anda akan melihat tahapan aktivasi Anda. Setelah semua tahapan selesai, Anda akan melihat link ' keluar '. Anda dapat menggunakan tautan ini untuk keluar. Ini akan menyelesaikan sebagian besar kasus untuk penundaan aktivasi.
2. Di PIM, verifikasi bahwa Anda tercantum sebagai anggota peran.
3. Jika Anda mengaktifkan peran administrator Exchange, pastikan Anda keluar dan masuk kembali. Jika masalah masih terjadi, buka tiket dukungan dan Naikkan ini sebagai masalah. Jika Anda menggunakan peran administrator Exchange Anda untuk mengakses pusat keamanan dan kepatuhan, lihat langkah berikutnya.
4. Jika Anda mengaktifkan peran untuk mengakses pusat keamanan dan kepatuhan atau jika Anda mengaktifkan peran administrator SharePoint, Anda akan mengalami beberapa penundaan aktivasi dari beberapa menit hingga beberapa jam. Ini adalah masalah umum dan kami sedang bekerja sama dengan tim ini untuk mengatasi masalah ini sesegera mungkin.

Untuk informasi selengkapnya, lihat:

- [Mengaktifkan peran Azure AD di PIM](https://docs.microsoft.com/azure/active-directory/privileged-identity-management/pim-how-to-activate-role?WT.mc_id=Portal-Microsoft_Azure_Support "https://docs.microsoft.com/azure/active-directory/privileged-identity-management/pim-how-to-activate-role?wt.mc_id=portal-microsoft_azure_support")
- [Mengaktifkan peran sumber daya Azure saya di PIM](https://docs.microsoft.com/azure/active-directory/privileged-identity-management/pim-resource-roles-activate-your-roles?WT.mc_id=Portal-Microsoft_Azure_Support "https://docs.microsoft.com/azure/active-directory/privileged-identity-management/pim-resource-roles-activate-your-roles?wt.mc_id=portal-microsoft_azure_support")

**Izin tidak dihapus setelah menonaktifkan peran atau aktivasi peran kedaluwarsa**

Saat Anda menonaktifkan peran dalam manajemen identitas Azure AD Privilege atau ketika periode aktivasi peran berakhir, mungkin ada penundaan ketika Anda masih memiliki akses.

Jika penonaktifan ditunda, ikuti langkah-langkah berikut:

1. Jika Anda menonaktifkan peran administrator Exchange atau periode aktivasi peran kedaluwarsa, dan Anda melihat penundaan yang signifikan sebelum izin dihapus, buka tiket dukungan dan beri tahu teknisi dukungan Anda untuk membantu Anda mengirimkan tiket dengan tim manajemen akses istimewa (PAM) di dalam kantor tentang masalah ini.
2. Jika periode aktivasi telah kedaluwarsa, tapi Anda masih memiliki sesi browser terbuka, tutup browser Anda. Anda dapat terus menggunakan peran hingga Anda menutup sesi tersebut. Ini adalah masalah umum dan kami melihat potensi perbaikan untuk secara aktif mencabut setiap sesi setelah aktivasi kedaluwarsa.

Jika delay berbeda dengan dua skenario ini, silakan buka tiket dukungan.
