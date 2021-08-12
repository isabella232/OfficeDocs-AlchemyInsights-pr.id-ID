---
title: 646 Cara mengonfigurasi AADConnect
ms.author: chrisda
author: chrisda
manager: dansimp
ms.date: 04/21/2020
ms.audience: ITPro
ms.topic: article
ms.service: o365-administration
ROBOTS: NOINDEX, NOFOLLOW
localization_priority: Normal
ms.custom:
- "646"
- "1300023"
ms.assetid: 599698ac-6709-477a-a66f-169b3165064e
ms.openlocfilehash: c5fa5fd7586f999698fe43554fb9a2b205be3e25740c20763254a38d41297e0c
ms.sourcegitcommit: b5f7da89a650d2915dc652449623c78be6247175
ms.translationtype: MT
ms.contentlocale: id-ID
ms.lasthandoff: 08/05/2021
ms.locfileid: "53963646"
---
# <a name="configure-sync-features"></a>Mengonfigurasi fitur sinkronisasi

Azure AD Koneksi menyertakan beberapa fitur yang diaktifkan secara default, atau yang dapat Anda aktifkan nanti. Beberapa fitur memerlukan konfigurasi tambahan di lingkungan tertentu.

- [Pembatasan pemfilteran](https://docs.microsoft.com/azure/active-directory/connect/active-directory-aadconnectsync-configure-filtering) objek disinkronkan ke Azure AD. Secara default, semua pengguna, kontak, grup, Windows 10 akun komputer disinkronkan. Anda bisa menyertakan atau mengecualikan objek berdasarkan domain, OUs, atau atribut lain.

- [Sinkronisasi hash kata](https://docs.microsoft.com/azure/active-directory/connect/active-directory-aadconnectsync-implement-password-hash-synchronization) sandi menyinkronkan hash kata sandi dari Direktori Aktif lokal ke Azure AD. Ini memungkinkan manajemen kata sandi di satu lokasi, tapi penggunaan kata sandi yang sama di lingkungan lokal dan awan. Karena Direktori Aktif adalah sumber otoritatif, Anda bisa menggunakan kebijakan kata sandi Anda sendiri.

- [Reset kata sandi layanan mandiri (SSPR)](https://docs.microsoft.com/azure/active-directory/authentication/quickstart-sspr) memungkinkan pengguna untuk mereset kata sandi mereka sendiri di awan saat masih menerapkan kebijakan kata sandi lokal Anda.

- [Menulis kembali](https://docs.microsoft.com/azure/active-directory/connect/active-directory-aadconnect-feature-device-writeback) perangkat memungkinkan perangkat yang terdaftar di Azure AD untuk ditulis kembali ke Direktori Aktif lokal sehingga dapat digunakan untuk akses bersyarat.

- [Cegah penghapusan tidak](https://docs.microsoft.com/azure/active-directory/connect/active-directory-aadconnectsync-feature-prevent-accidental-deletes) disengaja diaktifkan secara default untuk membantu mencegah terlalu banyak penghapusan objek secara bersamaan (lebih dari 500 objek per sinkronisasi). Anda bisa mengubah pengaturan ini untuk memenuhi kebutuhan organisasi Anda.

- [Pemutakhiran otomatis](https://docs.microsoft.com/azure/active-directory/connect/active-directory-aadconnect-feature-automatic-upgrade) diaktifkan secara default untuk penginstalan ekspres dan membantu memastikan versi Azure AD Koneksi selalu terbaru.
