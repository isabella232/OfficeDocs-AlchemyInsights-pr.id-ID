---
title: Menghapus data dan menyeka perangkat dari Intune
ms.author: pebaum
author: pebaum
manager: scotv
ms.date: 07/27/2020
ms.audience: Admin
ms.topic: article
ROBOTS: NOINDEX, NOFOLLOW
localization_priority: Priority
ms.collection: Adm_O365
ms.custom:
- "1279"
- "6700008"
ms.openlocfilehash: efaf111f694ab57d0435b141a6d4baad58658ed2
ms.sourcegitcommit: e34bb95fb93250f1dc7aec6a13578bb3bb355935
ms.translationtype: MT
ms.contentlocale: id-ID
ms.lasthandoff: 07/28/2020
ms.locfileid: "45439647"
---
# <a name="removing-data-and-wiping-devices-from-intune"></a>Menghapus data dan menyeka perangkat dari Intune

Device pensiun dan penghapusan perangkat tindakan jarak jauh dapat digunakan untuk menghapus data perusahaan yang dikelola oleh Intune atau melakukan reset pabrik dan mengembalikan perangkat ke pengaturan default.

1. Masuk ke Microsoft 365 manajemen perangkat, dan pergi ke **perangkat**  >  **semua perangkat**.
2. Pilih perangkat yang akan dihapus.
3. Pilih jenis penghapusan jarak jauh yang ingin Anda lakukan. Pensiun hanya menghapus informasi organisasi, sementara tisu penuh mengembalikan perangkat ke pengaturan pabriknya.
4. Pilih **ya** untuk mengonfirmasi. Hingga penghapusan selesai, status tindakan perangkat akan ditampilkan sebagai pensiun tertunda.</br>
    Setelah tindakan selesai, Anda tidak akan lagi melihat perangkat seluler di Daftar perangkat yang dikelola.

**Catatan** Data perusahaan tidak dapat dihapus dari perangkat bergabung ke Azure AD.

Untuk rincian lengkap tentang efek dari tindakan pensiun dan wipe, termasuk apa yang dipertahankan dan apa yang dihapus, lihat [menghapus perangkat dengan menggunakan wipe, pensiun, atau secara manual unenrolling perangkat](https://docs.microsoft.com/intune/devices-wipe).

Untuk menghapus semua data dari perangkat macOS, lihat [menghapus semua data dari perangkat MacOS](https://docs.microsoft.com/intune/device-erase).