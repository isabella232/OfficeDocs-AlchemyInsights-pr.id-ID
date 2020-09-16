---
title: Pemilik tidak dapat membuat sub-folder menggunakan Outlook
ms.author: pebaum
author: pebaum
manager: mnirkhe
ms.date: 04/21/2020
ms.audience: Admin
ms.topic: article
ms.service: o365-administration
ROBOTS: NOINDEX, NOFOLLOW
localization_priority: Priority
ms.collection: Adm_O365
ms.custom:
- "5884"
- "3500007"
ms.openlocfilehash: 9590f780cffeaf644733752c763e04d748b1b39e
ms.sourcegitcommit: c6692ce0fa1358ec3529e59ca0ecdfdea4cdc759
ms.translationtype: MT
ms.contentlocale: id-ID
ms.lasthandoff: 09/14/2020
ms.locfileid: "47665721"
---
# <a name="owner-cannot-create-sub-folder-using-outlook"></a>Pemilik tidak dapat membuat sub-folder menggunakan Outlook

**Ada masalah yang sedang berlangsung dengan pemilik folder publik membuat subfolder menggunakan Outlook. Masalah akan segera diperbaiki.**

Sementara itu, gunakan salah satu solusi berikut:

1. Menggunakan Outlook untuk MAC untuk membuat subfolder karena masalah hanya memengaruhi Outlook untuk desktop Windows (semua versi)
2. Membuat admin membuat subfolder menggunakan EXO shell atau EAC
3. Mengubah DefaultPublicFolderMailbox/EffectivePublicFolderMailbox pada pengguna ke kotak surat lain dari kotak surat konten untuk masalah yang menyebabkan folder  
    - *Set-kotak surat User1 DefaultPublicFolderMailbox PubMBX3*
4. Menunggu satu jam, mulai ulang klien Outlook