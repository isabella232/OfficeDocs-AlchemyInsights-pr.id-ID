---
title: Mengatur balasan otomatis untuk kotak surat
ms.author: pebaum
author: pebaum
manager: scotv
ms.audience: Admin
ms.topic: article
ms.service: o365-administration
ROBOTS: NOINDEX, NOFOLLOW
localization_priority: Priority
ms.collection: Adm_O365
ms.custom:
- "9000761"
- "3514"
ms.openlocfilehash: 85b7e969032607216c948532dcdf83ba09022c7cdfaebce8671c6d2e8fef183d
ms.sourcegitcommit: b5f7da89a650d2915dc652449623c78be6247175
ms.translationtype: MT
ms.contentlocale: id-ID
ms.lasthandoff: 08/05/2021
ms.locfileid: "54046611"
---
# <a name="set-auto-replies-for-a-users-mailbox"></a>Mengatur balasan otomatis untuk kotak surat pengguna

**Metode 1**

1. Masuk ke portal Microsoft 365.

2. Masuk ke **Pengguna > Pengguna aktif** (atau **Grup > Kotak surat bersama** jika Anda menetapkannya di kotak surat bersama).

3. Pilih pengguna yang memiliki kotak surat Microsoft Exchange.

4. Pada menu fly-out di sebelah kanan, masuk ke **Pengaturan email > Balasan otomatis** (jika ini adalah kotak surat bersama, cukup klik **Balasan otomatis** pada fly-out).

**Metode 2**

1. Masuk ke portal admin Microsoft 365 menggunakan kredensial administrator.

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
