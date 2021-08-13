---
title: Menghapus data dan menghapus perangkat secara menyeluruh dari Intune
ms.author: pebaum
author: pebaum
manager: scotv
ms.date: 07/27/2020
ms.audience: Admin
ms.topic: article
ms.service: o365-administration
ROBOTS: NOINDEX, NOFOLLOW
localization_priority: Priority
ms.collection: Adm_O365
ms.custom:
- "1279"
- "6700008"
- "9004638"
- "8392"
ms.openlocfilehash: f3614a41c1bc92184d7f8a11bd224310fef6aa0cabc8e1db1288bde01ca1cb5a
ms.sourcegitcommit: b5f7da89a650d2915dc652449623c78be6247175
ms.translationtype: MT
ms.contentlocale: id-ID
ms.lasthandoff: 08/05/2021
ms.locfileid: "53922232"
---
# <a name="removing-data-and-wiping-devices-from-intune"></a>Menghapus data dan menghapus perangkat secara menyeluruh dari Intune

Tindakan jarak jauh Penghentian Perangkat dan Penghapusan Perangkat dapat digunakan untuk menghapus data perusahaan yang dikelola oleh Intune atau untuk melakukan reset pabrik dan mengembalikan perangkat ke pengaturan default-nya.

1. Masuk ke Manajemen Perangkat Microsoft 365, lalu buka **Perangkat** > **Semua Perangkat**.
2. Pilih perangkat yang ingin Anda hapus.
3. Pilih jenis penghapusan jarak jauh yang ingin Anda lakukan. Penghentian hanya menghapus informasi organisasi, sementara penghapusan menyeluruh mengembalikan perangkat ke pengaturan pabriknya.
4. Pilih **Ya** untuk mengonfirmasi. Hingga penghapusan selesai, status tindakan perangkat ditampilkan sebagai *Penghentian Tertunda*.
    Setelah tindakan selesai, Anda tidak akan melihat lagi perangkat seluler di daftar perangkat terkelola.

> [!NOTE]
> Data perusahaan tidak dapat dihapus dari perangkat yang BERGABUNG ke Microsoft Azure AD. 

Untuk detail lengkap tentang dampak dari tindakan Penghentian dan Penghapusan, termasuk apa yang dipertahankan dan apa yang dihapus, lihat dokumentasi berikut:

- [Hapus perangkat dengan menggunakan penghapusan menyeluruh, penghentian, atau pembatalan pendaftaran perangkat secara manual](https://docs.microsoft.com/mem/intune/remote-actions/devices-wipe).
- [Cara untuk hanya menghapus data perusahaan dari aplikasi yang dikelola Intune](https://docs.microsoft.com/mem/intune/apps/apps-selective-wipe)
- [Hapus semua data dari perangkat macOS](https://docs.microsoft.com/mem/intune/remote-actions/device-erase).