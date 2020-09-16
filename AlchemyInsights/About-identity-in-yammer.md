---
title: Tentang identitas di Yammer
ms.author: pebaum
author: pebaum
manager: scotv
ms.date: 07/15/2020
ms.audience: Admin
ms.topic: article
ms.service: o365-administration
ROBOTS: NOINDEX, NOFOLLOW
localization_priority: Priority
ms.collection: Adm_O365
ms.custom:
- "6039"
- "9003111"
ms.openlocfilehash: f417117acac4c3040932fc0a35e5d0b1c3709cd5
ms.sourcegitcommit: c6692ce0fa1358ec3529e59ca0ecdfdea4cdc759
ms.translationtype: MT
ms.contentlocale: id-ID
ms.lasthandoff: 09/14/2020
ms.locfileid: "47664173"
---
# <a name="about-identity-in-yammer"></a>Tentang identitas di Yammer

Disarankan agar semua jaringan melakukan langkah-langkah berikut untuk menghindari masalah terkait identitas:

1. Terapkan identitas 365 Office setelah menetapkan akun Microsoft 365 untuk pengguna di Azure AD guna memastikan bahwa semua pengguna masuk menggunakan akun 365 Microsoft utama Microsoft. Untuk informasi selengkapnya, lihat [memaksakan identitas Office 365 untuk pengguna Yammer](https://docs.microsoft.com/yammer/configure-your-yammer-network/enforce-office-365-identity).
2. Menggabungkan beberapa jaringan Yammer. Warisan konfigurasi Yammer mengizinkan beberapa jaringan Yammer untuk tersambung ke satu penyewa. Untuk informasi selengkapnya, lihat [migrasi jaringan-menggabungkan beberapa jaringan Yammer](https://docs.microsoft.com/yammer/configure-your-yammer-network/consolidate-multiple-yammer-networks).
3. Secara opsional, Terapkan lisensi untuk Yammer untuk memblokir pengguna dari Yammer jika mereka tidak memiliki lisensi. Untuk informasi selengkapnya, lihat [mengelola lisensi pengguna Yammer di Office 365](https://docs.microsoft.com/yammer/manage-yammer-users/manage-yammer-licenses-in-office-365).
4. Terakhir, audit daftar pengguna untuk jaringan Yammer yang lebih lama dan tangguhkan pengguna pewaris. Disarankan agar Anda menangguhkan (menonaktifkan) pengguna dan bukan menghapusnya, karena penghapusan tidak dapat dibatalkan. Untuk informasi selengkapnya, lihat [mengaudit pengguna Yammer di jaringan yang tersambung ke Office 365](https://docs.microsoft.com/yammer/manage-yammer-users/audit-users-connected-to-office-365) dan [menghapus pengguna](https://docs.microsoft.com/yammer/manage-yammer-users/add-block-or-remove-users#remove-users).

Dengan mengonfigurasi Yammer menggunakan langkah-langkah ini, Anda juga akan siap mengonfigurasi jaringan Yammer Anda untuk mode asli untuk Microsoft 365. Untuk informasi selengkapnya, lihat [mengonfigurasi jaringan Yammer Anda untuk Microsoft 365](https://docs.microsoft.com/yammer/configure-your-yammer-network/native-mode).