---
title: 646 cara mengkonfigurasi AADConnect
ms.author: chrisda
author: chrisda
manager: dansimp
ms.date: 04/21/2020
ms.audience: ITPro
ms.topic: article
ROBOTS: NOINDEX, NOFOLLOW
localization_priority: Normal
ms.custom:
- "646"
- "1300023"
ms.assetid: 599698ac-6709-477a-a66f-169b3165064e
ms.openlocfilehash: 713cda26e55f07f0438cb9ebe5aa9da86c4ebb3a
ms.sourcegitcommit: 55eff703a17e500681d8fa6a87eb067019ade3cc
ms.translationtype: MT
ms.contentlocale: id-ID
ms.lasthandoff: 04/22/2020
ms.locfileid: "43722563"
---
# <a name="configure-sync-features"></a>Mengkonfigurasi fitur sinkronisasi

Azure AD menyambung mencakup beberapa fitur yang diaktifkan secara default, atau bahwa Anda dapat mengaktifkan kemudian. Beberapa fitur memerlukan konfigurasi tambahan di lingkungan tertentu.

- [Penyaringan](https://docs.microsoft.com/azure/active-directory/connect/active-directory-aadconnectsync-configure-filtering) membatasi objek disinkronkan ke Azure AD. Secara default, semua pengguna, kontak, grup, dan akun komputer Windows 10 disinkronkan. Anda dapat menyertakan atau mengecualikan objek berdasarkan domain, ou, atau atribut lainnya.

- [Sinkronisasi hash sandi](https://docs.microsoft.com/azure/active-directory/connect/active-directory-aadconnectsync-implement-password-hash-synchronization) menyinkronkan hash sandi dari Active Directory lokal ke Azure AD. Hal ini memungkinkan pengelolaan sandi di satu lokasi, namun menggunakan sandi yang sama di lingkungan lokal dan Cloud. Karena Active Directory adalah sumber otoritatif, Anda dapat menggunakan kebijakan sandi Anda sendiri.

- [Pengaturan ulang kata sandi layanan mandiri (SSPR)](https://docs.microsoft.com/azure/active-directory/authentication/quickstart-sspr) memungkinkan pengguna menyetel ulang sandi mereka di Cloud saat masih menerapkan kebijakan sandi lokal.

- [Perangkat tulis balik](https://docs.microsoft.com/azure/active-directory/connect/active-directory-aadconnect-feature-device-writeback) memungkinkan perangkat terdaftar di Azure AD untuk ditulis kembali ke direktori aktif di tempat sehingga mereka dapat digunakan untuk akses bersyarat.

- [Mencegah menghapus disengaja](https://docs.microsoft.com/azure/active-directory/connect/active-directory-aadconnectsync-feature-prevent-accidental-deletes) diaktifkan secara default untuk membantu mencegah terlalu banyak penghapusan objek simultan (lebih dari 500 objek per sinkronisasi). Anda dapat mengubah pengaturan ini untuk memenuhi kebutuhan organisasi Anda.

- [Peningkatan otomatis](https://docs.microsoft.com/azure/active-directory/connect/active-directory-aadconnect-feature-automatic-upgrade) diaktifkan secara default untuk instalasi Ekspres dan membantu memastikan bahwa versi Azure AD Connect selalu terkini.
