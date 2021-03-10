---
title: Contoh kebijakan Microsoft Defender untuk Office 365 Safe attachment
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
ms.openlocfilehash: 077762dd37a2974b4e519c1f242fa753623cb49a
ms.sourcegitcommit: 4883f1f89d4c6ca23161e9a43ff206ad21d4f09b
ms.translationtype: MT
ms.contentlocale: id-ID
ms.lasthandoff: 03/08/2021
ms.locfileid: "50693828"
---
# <a name="example-microsoft-defender-for-office-365-safe-attachment-policy"></a>Contoh kebijakan Microsoft Defender untuk Office 365 Safe attachment

Pengaturan ini mengaktifkan kebijakan yang *tidak disebut keterlambatan* yang akan mengirimkan pesan dengan segera lalu melepaskan kembali lampiran setelah dipindai:

- **Nama**: tidak ada keterlambatan
- **Deskripsi**: mengirimkan pesan dengan segera dan melampirkan kembali lampiran setelah pemindaian.
- **Respons**: Pilih opsi **pengiriman dinamis** . Untuk informasi selengkapnya, lihat [pengiriman dinamis dalam kebijakan lampiran aman](https://go.microsoft.com/fwlink/?linkid=2092328).
- Bagian **lampiran pengalihan** : Pilih opsi untuk **mengaktifkan pengalihan**, lalu masukkan alamat email administrator global Microsoft 365, administrator keamanan, atau analis keamanan yang akan menyelidiki lampiran berbahaya.
- **Diterapkan ke** bagian: Pilih **domain Penerima**, lalu pilih domain Anda. Pilih **Tambahkan**, lalu pilih **OK**. Setelah selesai, pilih **Simpan**.

Untuk mempelajari selengkapnya, lihat [lampiran aman di Microsoft Defender untuk Office 365](https://go.microsoft.com/fwlink/?linkid=2092213).
