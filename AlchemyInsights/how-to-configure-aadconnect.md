---
title: 646 cara mengkonfigurasi AADConnect
ms.author: chrisda
author: chrisda
manager: dansimp
ms.date: 6/8/2018
ms.audience: ITPro
ms.topic: article
ROBOTS: NOINDEX, NOFOLLOW
localization_priority: Normal
ms.custom: 646
ms.assetid: 599698ac-6709-477a-a66f-169b3165064e
ms.openlocfilehash: 2dc4ae7d6809c24ce599ac128570e9354c9f2b30
ms.sourcegitcommit: 4b7e478ce700c0b781efec3857ac4dce5bdf00c6
ms.translationtype: MT
ms.contentlocale: id-ID
ms.lasthandoff: 06/07/2019
ms.locfileid: "34752564"
---
# <a name="configure-sync-features"></a>Mengkonfigurasi fitur sinkronisasi

Azure iklan Connect mencakup beberapa fitur yang diaktifkan secara default, atau bahwa Anda dapat mengaktifkan kemudian. Beberapa fitur yang memerlukan konfigurasi tambahan di lingkungan tertentu.

- Batas [menyaring](https://docs.microsoft.com/azure/active-directory/connect/active-directory-aadconnectsync-configure-filtering) objek disinkronisasi Azure iklan. Secara default, semua pengguna, kontak, grup, dan Windows 10 komputer account disinkronisasi. Anda dapat menyertakan atau mengecualikan benda-benda yang didasarkan pada domain, OUs, atau atribut lainnya.

- [Password hash syncronization](https://docs.microsoft.com/azure/active-directory/connect/active-directory-aadconnectsync-implement-password-hash-synchronization) sinkronisasi password hash dari Active Directory lokal Azure iklan. Hal ini memungkinkan manajemen password di satu lokasi, tetapi menggunakan sandi yang sama di kedua lokal dan awan lingkungan. Karena Active Directory sumber otoritatif, Anda dapat menggunakan kebijakan sandi Anda sendiri.

- [Reset password swalayan (SSPR)](https://docs.microsoft.com/azure/active-directory/authentication/quickstart-sspr) memungkinkan pengguna untuk membuat ulang sandi sendiri di Internet sementara masih menerapkan kebijakan sandi lokal Anda.

- [Perangkat writeback](https://docs.microsoft.com/azure/active-directory/connect/active-directory-aadconnect-feature-device-writeback) memungkinkan perangkat terdaftar di Azure iklan ditulis kembali ke Active Directory lokal sehingga mereka dapat digunakan untuk akses bersyarat.

- [Mencegah disengaja menghapus](https://docs.microsoft.com/azure/active-directory/connect/active-directory-aadconnectsync-feature-prevent-accidental-deletes) diaktifkan secara default untuk membantu mencegah penghapusan simultan objek terlalu banyak (lebih dari 500 obyek per sinkronisasi). Anda dapat mengubah pengaturan ini untuk memenuhi kebutuhan organisasi Anda.

- [Upgrade otomatis](https://docs.microsoft.com/azure/active-directory/connect/active-directory-aadconnect-feature-automatic-upgrade) diaktifkan secara default untuk instalasi Check dan membantu memastikan Anda versi Azure iklan Connect selalu saat ini.
