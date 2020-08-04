---
title: Pembersihan otomatis perangkat kedaluwarsa di Intune
ms.author: pebaum
author: pebaum
manager: scotv
ms.date: 07/28/2020
ms.audience: Admin
ms.topic: article
ROBOTS: NOINDEX, NOFOLLOW
localization_priority: Priority
ms.collection: Adm_O365
ms.custom:
- "1285"
- "6700008"
ms.openlocfilehash: 874ee290c59df3b5de1421369484a1a5a0ff7be4
ms.sourcegitcommit: 0e50dfcdb3f6aa72368279e23b83efecb9dc9c3f
ms.translationtype: MT
ms.contentlocale: id-ID
ms.lasthandoff: 07/28/2020
ms.locfileid: "46555222"
---
# <a name="automatic-cleanup-of-stale-devices-in-intune"></a>Pembersihan otomatis perangkat kedaluwarsa di Intune

Intune memungkinkan admin untuk mengkonfigurasi interval waktu antara 90 dan 270 hari, setelah perangkat kedaluwarsa dihapus dari layanan. Pengaturan ini adalah organisasi luas dan sekali diaktifkan berlaku segera. Perangkat apa pun yang tidak diperiksa ke server Intune untuk jangka waktu yang melebihi pengaturan akan dihapus secara permanen.

**Catatan** Hanya objek perangkat MDM yang memenuhi syarat untuk tindakan pembersihan ini. EA hanya objek perangkat dikecualikan.

Untuk informasi tambahan saat perangkat menjadi memenuhi syarat untuk penghapusan berdasarkan pengaturan pembersihan perangkat dan "keadaan":

Pengaturan: **Hapus perangkat setelah tanggal Check-In terakhir: Ya (beberapa nilai (N) di hari yang ditentukan)**

- Berdasarkan nilai (N) dikonfigurasi dalam pengaturan, Layanan Intune menghapus perangkat dalam beberapa hari setelah terakhir berhasil Check-in.

Pengaturan: **Hapus perangkat setelah tanggal Check-In terakhir: tidak**

- 180 hari setelah sertifikat perangkat kedaluwarsa dan tidak diperbarui, perangkat akan dihapus.

**Catatan** Dalam kedua kasus, perangkat harus terdaftar berhasil di Intune. Pendaftaran terjadi selama checkin perangkat pertama dengan layanan Intune.

Jika perangkat mendaftar berhasil untuk Intune tetapi tidak menjadi Intune terdaftar, perangkat dihapus 270 hari setelah pendaftaran. (90 hari untuk menandai perangkat sebagai dicabut, dan kemudian 180 hari lagi untuk menghapus catatan.)

Mekanisme tidak ada saat ini di konsol Intune untuk menetapkan tanggal kedaluwarsa sertifikasi perangkat untuk setiap perangkat tertentu.