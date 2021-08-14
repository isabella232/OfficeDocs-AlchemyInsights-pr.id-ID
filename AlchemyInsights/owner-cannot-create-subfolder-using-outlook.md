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
ms.openlocfilehash: 60190727e75c120ad3915da8b563b7f6b1a3238b46bb6e14cbf956365e1a84e0
ms.sourcegitcommit: b5f7da89a650d2915dc652449623c78be6247175
ms.translationtype: MT
ms.contentlocale: id-ID
ms.lasthandoff: 08/05/2021
ms.locfileid: "54063127"
---
# <a name="owner-cannot-create-sub-folder-using-outlook"></a>Pemilik tidak dapat membuat sub-folder menggunakan Outlook

**Masih terdapat masalah dengan pemilik folder publik yang membuat subfolder menggunakan Outlook. Masalah akan segera diperbaiki.**

Sementara itu, gunakan salah satu solusi berikut:

1. Gunakan Outlook untuk MAC guna membuat subfolder sebagai masalah yang hanya memengaruhi Outlook desktop (semua versi)
2. Buat admin membuat subfolder menggunakan EXO Shell atau EAC
3. Mengubah DefaultPublicFolderMailbox/EffectivePublicFolderMailbox pada pengguna ke kotak surat lain dari Kotak Surat Konten untuk folder yang menyebabkan masalah  
    - *Set-Mailbox User1 DefaultPublicFolderMailbox PubMBX3*
4. Tunggu satu jam, mulai ulang klien outlook