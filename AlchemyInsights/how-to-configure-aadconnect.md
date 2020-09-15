---
title: 646 cara mengonfigurasi AADConnect
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
ms.openlocfilehash: 6327e42b74283d732247c9a847c68db72082c56a
ms.sourcegitcommit: c6692ce0fa1358ec3529e59ca0ecdfdea4cdc759
ms.translationtype: MT
ms.contentlocale: id-ID
ms.lasthandoff: 09/14/2020
ms.locfileid: "47704492"
---
# <a name="configure-sync-features"></a>Mengonfigurasi fitur sinkronisasi

Azure AD Connect menyertakan beberapa fitur yang diaktifkan secara default, atau yang dapat Anda Aktifkan nanti. Beberapa fitur memerlukan konfigurasi tambahan dalam lingkungan tertentu.

- [Pemfilteran](https://docs.microsoft.com/azure/active-directory/connect/active-directory-aadconnectsync-configure-filtering) membatasi objek disinkronkan ke Azure AD. Secara default, semua pengguna, kontak, grup, dan akun komputer Windows 10 disinkronisasi. Anda bisa menyertakan atau mengecualikan objek berdasarkan domain, ou, atau atribut lainnya.

- [Sinkronisasi hash kata](https://docs.microsoft.com/azure/active-directory/connect/active-directory-aadconnectsync-implement-password-hash-synchronization) sandi menyinkronkan hash kata sandi dari direktori aktif lokal ke Azure AD. Ini memungkinkan manajemen kata sandi dalam satu lokasi, tetapi penggunaan kata sandi yang sama di lingkungan lokal dan awan. Karena direktori aktif adalah sumber otoritatif, Anda dapat menggunakan kebijakan kata sandi Anda sendiri.

- [Reset kata sandi layanan mandiri (SSPR)](https://docs.microsoft.com/azure/active-directory/authentication/quickstart-sspr) memungkinkan pengguna untuk mengatur ulang kata sandi mereka sendiri di awan saat masih menerapkan kebijakan kata sandi lokal Anda.

- [Alat tulis balik perangkat](https://docs.microsoft.com/azure/active-directory/connect/active-directory-aadconnect-feature-device-writeback) memungkinkan perangkat terdaftar di Azure AD untuk ditulis kembali ke direktori aktif di tempat sehingga dapat digunakan untuk akses bersyarat.

- [Mencegah penghapusan disengaja](https://docs.microsoft.com/azure/active-directory/connect/active-directory-aadconnectsync-feature-prevent-accidental-deletes) diaktifkan secara default untuk membantu mencegah terlalu banyak penghapusan objek bersamaan (lebih dari 500 objek per sinkronisasi). Anda dapat mengubah pengaturan ini untuk memenuhi kebutuhan organisasi Anda.

- [Pemutakhiran otomatis](https://docs.microsoft.com/azure/active-directory/connect/active-directory-aadconnect-feature-automatic-upgrade) diaktifkan secara default untuk penginstalan kilat dan membantu memastikan versi Azure AD Connect selalu terkini.
