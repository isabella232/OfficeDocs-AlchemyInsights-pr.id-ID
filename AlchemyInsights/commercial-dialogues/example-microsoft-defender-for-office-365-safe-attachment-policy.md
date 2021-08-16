---
title: Contoh Pertahanan Microsoft untuk Office 365 Brankas Attachment
ms.author: v-jmathew
author: v-jmathew
manager: dansimp
audience: Admin
ms.topic: article
ms.service: o365-administration
ROBOTS: NOINDEX, NOFOLLOW
localization_priority: Normal
ms.collection: Adm_O365
ms.custom:
- "9000760"
- "7391"
ms.openlocfilehash: 7294be81a24fa61a92367bae304798a333cb916c8718e28b1a87314c15ef6c8c
ms.sourcegitcommit: b5f7da89a650d2915dc652449623c78be6247175
ms.translationtype: MT
ms.contentlocale: id-ID
ms.lasthandoff: 08/05/2021
ms.locfileid: "53988298"
---
# <a name="example-microsoft-defender-for-office-365-safe-attachment-policy"></a>Contoh Pertahanan Microsoft untuk Office 365 Brankas Attachment

Pengaturan ini mengaktifkan kebijakan *yang disebut Tidak ada* penundaan yang mengirimkan pesan dengan segera lalu menghapus kembali lampiran setelah dipindai:

- **Nama**: Tidak ada penundaan
- **Deskripsi**: Mengirimkan pesan dengan segera dan menyerang kembali lampiran setelah memindai.
- **Respons**: Pilih **opsi Pengiriman** Dinamis. Untuk informasi selengkapnya, lihat [Pengiriman Dinamis Brankas Kebijakan Lampiran](https://go.microsoft.com/fwlink/?linkid=2092328).
- **Mengalihkan bagian** lampiran: Pilih opsi untuk Mengaktifkan pengalihan **,** lalu masukkan alamat email administrator global Microsoft 365, administrator keamanan, atau analis keamanan yang akan menyelidiki lampiran berbahaya.
- **Bagian Diterapkan** Ke: **Pilih Domain penerima adalah**, lalu pilih domain Anda. Pilih **tambahkan**, lalu pilih **OK.** Setelah Anda selesai, pilih **Simpan**.

Untuk mempelajari selengkapnya, [lihat Brankas Lampiran di Pertahanan Microsoft untuk Office 365](https://go.microsoft.com/fwlink/?linkid=2092213).
