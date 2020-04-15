---
title: Mengatur balasan otomatis untuk kotak surat
ms.author: pebaum
author: pebaum
manager: mnirkhe
ms.audience: Admin
ms.topic: article
ROBOTS: NOINDEX, NOFOLLOW
localization_priority: Priority
ms.collection: Adm_O365
ms.custom:
- "9000761"
- "3514"
ms.openlocfilehash: aeeb2e1e76fe602d2767b422797452fd1155fdd5
ms.sourcegitcommit: fdfd41c2bfb2d45003b3906e6469377384a91cb5
ms.translationtype: HT
ms.contentlocale: id-ID
ms.lasthandoff: 04/15/2020
ms.locfileid: "43509505"
---
# <a name="set-auto-replies-for-a-users-mailbox"></a>Mengatur balasan otomatis untuk kotak surat pengguna

**Metode 1**

1. Masuk ke portal Office 365.

2. Masuk ke **Pengguna > Pengguna aktif** (atau **Grup > Kotak surat bersama** jika Anda menetapkannya di kotak surat bersama).

3. Pilih pengguna yang memiliki kotak surat Microsoft Exchange.

4. Pada menu fly-out di sebelah kanan, masuk ke **Pengaturan email > Balasan otomatis** (jika ini adalah kotak surat bersama, cukup klik **Balasan otomatis** pada fly-out).

**Metode 2**

1. Masuk ke portal admin Office 365 menggunakan kredensial administrator.

2. Perluas **Pusat Admin**, lalu klik **Exchange**.

3. Klik gambar di sudut kanan atas, klik **Pengguna Lain**, lalu pilih kotak surat pengguna yang ingin Anda ubah.

4. Di sisi kiri, pilih **Opsi**, klik **Atur Email**, lalu klik **Balasan otomatis.**

**Metode 3**

Jalankan cmdlet berikut ini di Exchange Online PowerShell:

PowerShellCopy

```
    Set-MailboxAutoReplyConfiguration
```

Untuk informasi selengkapnya tentang cmdlet ini, lihat [Set-MailboxAutoReplyConfiguration](https://docs.microsoft.com/powershell/module/exchange/mailboxes/set-mailboxautoreplyconfiguration).
