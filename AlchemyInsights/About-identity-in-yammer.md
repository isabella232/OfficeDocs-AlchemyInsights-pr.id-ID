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
ms.openlocfilehash: 57e7e6328747fc05b89799d631b2c6d7e0056547253aa3d75cdecb38cea3ad7e
ms.sourcegitcommit: b5f7da89a650d2915dc652449623c78be6247175
ms.translationtype: MT
ms.contentlocale: id-ID
ms.lasthandoff: 08/05/2021
ms.locfileid: "53918940"
---
# <a name="about-identity-in-yammer"></a>Tentang identitas di Yammer

Disarankan agar semua jaringan melakukan langkah-langkah berikut ini untuk menghindari masalah yang terkait dengan identitas:

1. Terapkan Office 365 identitas setelah penyediaan Microsoft 365 pengguna di Azure AD untuk memastikan bahwa semua pengguna masuk dengan menggunakan akun utama Microsoft 365 mereka. Untuk informasi selengkapnya, lihat [Menerapkan Office 365 identitas bagi Yammer pengguna.](https://docs.microsoft.com/yammer/configure-your-yammer-network/enforce-office-365-identity)
2. Mengonsolidasi beberapa Yammer jaringan. Konfigurasi Yammer warisan mengizinkan beberapa Yammer jaringan tersambung ke satu penyewa. Untuk informasi selengkapnya, lihat [Migrasi jaringan - Menggabungkan beberapa Yammer jaringan](https://docs.microsoft.com/yammer/configure-your-yammer-network/consolidate-multiple-yammer-networks).
3. Secara opsional, terapkan lisensi Yammer untuk memblokir Yammer pengguna dari komputer jika mereka tidak memiliki lisensi. Untuk informasi selengkapnya, [lihat Mengelola Yammer pengguna di Office 365](https://docs.microsoft.com/yammer/manage-yammer-users/manage-yammer-licenses-in-office-365).
4. Terakhir, audit daftar pengguna untuk jaringan Yammer lama dan tangguhkan pengguna warisan. Disarankan agar Anda menangguhkan (menonaktifkan) pengguna dan bukan menghapusnya, karena penghapusan tidak dapat dibatalkan. Untuk informasi selengkapnya, lihat [Audit Yammer pengguna di jaringan yang tersambung ke Office 365](https://docs.microsoft.com/yammer/manage-yammer-users/audit-users-connected-to-office-365) dan Hapus [pengguna.](https://docs.microsoft.com/yammer/manage-yammer-users/add-block-or-remove-users#remove-users)

Dengan mengonfigurasi Yammer langkah-langkah ini, Anda juga akan siap untuk mengonfigurasikan jaringan Yammer Anda untuk Mode Asli untuk Microsoft 365. Untuk informasi selengkapnya, lihat [Mengonfigurasi jaringan Yammer Anda untuk Mode Asli untuk Microsoft 365](https://docs.microsoft.com/yammer/configure-your-yammer-network/native-mode).