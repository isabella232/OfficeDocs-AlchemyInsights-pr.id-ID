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
ms.openlocfilehash: 5c7081f8991716a8ac72f462c6c7ef88e800ab9c
ms.sourcegitcommit: 6f1af4aed507d4c074c36d77666cf00100efe168
ms.translationtype: MT
ms.contentlocale: id-ID
ms.lasthandoff: 01/25/2021
ms.locfileid: "49974406"
---
# <a name="your-archive-mailbox-is-almost-full"></a>Kotak surat arsip Anda hampir penuh

Jika pengguna menerima peringatan; **Kotak surat arsip Anda hampir penuh**, atau Anda perlu memperbesar ukuran kotak surat arsip, berikut ini beberapa tips:

1. Jika pengguna ditetapkan ke lisensi Exchange Online paket 1, Mutakhirkan ke **Exchange Online paket 2** untuk menambah ukuran dari 50 GB ke 100gb.
1. Jika pengguna sudah ditetapkan salah satu hal berikut ini: **Exchange Online paket 2** atau Exchange Online paket 1 dengan add-on pengarsipan Exchange Online, gunakan langkah-langkah di bawah ini untuk mengaktifkan pengarsipan otomatis:.
 
    1. [Menyambungkan ke Exchange Online PowerShell](https://docs.microsoft.com/powershell/exchange/connect-to-exchange-online-powershell?view=exchange-ps&preserve-view=true).
    2. Jalankan unifiedgroup berikut ini untuk pengguna:  `Enable-Mailbox <user mailbox> -AutoExpandingArchive`
    1. Jalankan unifiedgroup berikut ini untuk mengonfirmasinya diaktifkan untuk pengguna:  `Get-Mailbox <user mailbox> | FL AutoExpandingArchiveEnabled`

Untuk informasi selengkapnya, lihat:

- [ Mengaktifkan pengarsipan tak terbatas-bantuan admin-kepatuhan Microsoft 365 | Dokumen Microsoft](https://docs.microsoft.com/microsoft-365/compliance/enable-unlimited-archiving?view=o365-worldwide&preserve-view=true)

- [Batas-Deskripsi Layanan Exchange Online | Dokumen Microsoft](https://docs.microsoft.com/office365/servicedescriptions/exchange-online-service-description/exchange-online-limits?redirectedfrom=MSDN#storage-limits-across-standalone-plans)

- [Memutakhirkan ke paket bisnis yang berbeda | Dokumen Microsoft](https://docs.microsoft.com/microsoft-365/commerce/subscriptions/upgrade-to-different-plan?view=o365-worldwide&preserve-view=true)

