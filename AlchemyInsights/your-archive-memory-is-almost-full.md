---
title: Kotak surat arsip Anda hampir penuh
ms.author: v-aiyengar
author: AshaIyengar21
manager: dansimp
ms.date: 01/25/2021
ms.audience: Admin
ms.topic: article
ms.service: o365-administration
ROBOTS: NOINDEX, NOFOLLOW
localization_priority: Normal
ms.collection: Adm_O365
ms.custom:
- "3100006"
- "7960"
ms.openlocfilehash: 085d9b211d5a8e9a0e1eb12af14d87a4e59c844a3afa012095dfd60db316ad14
ms.sourcegitcommit: b5f7da89a650d2915dc652449623c78be6247175
ms.translationtype: MT
ms.contentlocale: id-ID
ms.lasthandoff: 08/05/2021
ms.locfileid: "54046755"
---
# <a name="your-archive-mailbox-is-almost-full"></a>Kotak surat arsip Anda hampir penuh

Jika pengguna menerima peringatan; **Kotak surat arsip Anda hampir penuh**, atau Anda perlu menambah ukuran kotak surat arsip mereka, berikut ini beberapa tips:

1. Jika pengguna menerima penetapan lisensi Exchange Online Paket 1, mutakhirkan ke **Exchange Online Lisensi Paket 2** untuk menambah ukuran dari 50 GB menjadi 100GB.
1. Jika pengguna telah diberi salah satu hal berikut ini: **Exchange Online Paket 2** atau Exchange Online Paket 1 dengan add-on Exchange Online Archiving, gunakan langkah-langkah di bawah ini untuk mengaktifkan Pengarsipan Diperluas Otomatis:.
 
    1. [Koneksi ke Exchange Online Powershell](https://docs.microsoft.com/powershell/exchange/connect-to-exchange-online-powershell?view=exchange-ps&preserve-view=true).
    2. Jalankan commandlet berikut untuk pengguna:  `Enable-Mailbox <user mailbox> -AutoExpandingArchive`
    1. Jalankan commandlet berikut untuk mengonfirmasi bahwa commandlet telah diaktifkan untuk pengguna:  `Get-Mailbox <user mailbox> | FL AutoExpandingArchiveEnabled`

Untuk informasi selengkapnya lihat:

- [Mengaktifkan pengarsipan tanpa batas - Bantuan Admin - Microsoft 365 Kepatuhan | Microsoft Docs](https://docs.microsoft.com/microsoft-365/compliance/enable-unlimited-archiving?view=o365-worldwide&preserve-view=true)

- [Exchange Online umum - Deskripsi Layanan | Microsoft Docs](https://docs.microsoft.com/office365/servicedescriptions/exchange-online-service-description/exchange-online-limits?redirectedfrom=MSDN#storage-limits-across-standalone-plans)

- [Memutakhirkan ke paket bisnis lain | Microsoft Docs](https://docs.microsoft.com/microsoft-365/commerce/subscriptions/upgrade-to-different-plan?view=o365-worldwide&preserve-view=true)

