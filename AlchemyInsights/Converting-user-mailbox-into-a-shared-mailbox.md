---
title: Mengkonversi kotak pesan pengguna ke kotak pesan bersama?
ms.author: pebaum
author: pebaum
manager: mnirkhe
ms.audience: Admin
ms.topic: reference
ms.service: o365-administration
localization_priority: Normal
ROBOTS: NOINDEX, NOFOLLOW
description: ''
ms.openlocfilehash: ab34b8939b95b29bedb797f640dd744bc783adef
ms.sourcegitcommit: 1d98db8acb9959aba3b5e308a567ade6b62da56c
ms.translationtype: MT
ms.contentlocale: id-ID
ms.lasthandoff: 08/22/2019
ms.locfileid: "36496402"
---
# <a name="convert-a-user-mail-box-into-a-shared-mailbox"></a>Mengkonversi kotak pesan pengguna ke kotak pesan bersama

Anda hanya dapat mengkonversi kotak pesan pengguna ke kotak pesan bersama jika pengguna memiliki lisensi asing. Setelah kotak pesan yang diubah, itu akan terus muncul di daftar pengguna aktif karena daftar itu mencakup kotak pesan bersama. Namun, kotak pesan yang dikonversi akan juga muncul dalam daftar kotak pesan bersama. 
  
Jika Anda mencoba untuk mengkonversi kotak pesan di Exchange Admin Console dan konversi gagal, membersihkan tembolok peramban dan kuki dan coba lagi. Jika itu masih tidak bekerja, coba mengkonversi kotak pesan di Exchange Management Shell dengan menjalankan perintah berikut:
  
```
Set-Mailbox -Type Shared
```

Selengkapnya konversi kotak pesan ini tersedia dalam [mengkonversi pesan pengguna ke kotak pesan bersama](https://docs.microsoft.com/office365/admin/email/convert-user-mailbox-to-shared-mailbox).
  
