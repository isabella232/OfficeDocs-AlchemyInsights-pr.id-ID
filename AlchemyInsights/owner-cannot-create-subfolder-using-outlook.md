---
title: Pemilik tidak dapat membuat sub-folder menggunakan Outlook
ms.author: pebaum
author: pebaum
manager: scotv
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
ms.openlocfilehash: b2ab7b60bc521fd28d68333bb963528f7b9e05f2
ms.sourcegitcommit: 8bc60ec34bc1e40685e3976576e04a2623f63a7c
ms.translationtype: MT
ms.contentlocale: id-ID
ms.lasthandoff: 04/15/2021
ms.locfileid: "51836138"
---
# <a name="owner-cannot-create-sub-folder-using-outlook"></a>Pemilik tidak dapat membuat sub-folder menggunakan Outlook

**Masih terdapat masalah dengan pemilik folder publik yang membuat subfolder menggunakan Outlook. Masalah akan segera diperbaiki.**

Sementara itu, gunakan salah satu solusi berikut:

1. Menggunakan Outlook untuk MAC untuk membuat subfolder karena masalah hanya memengaruhi Outlook untuk jendela desktop (semua versi)
2. Buat admin membuat subfolder menggunakan EXO Shell atau EAC
3. Mengubah DefaultPublicFolderMailbox/EffectivePublicFolderMailbox pada pengguna ke kotak surat lain dari Kotak Surat Konten untuk folder yang menyebabkan masalah  
    - *Set-Mailbox User1 DefaultPublicFolderMailbox PubMBX3*
4. Tunggu satu jam, mulai ulang klien outlook