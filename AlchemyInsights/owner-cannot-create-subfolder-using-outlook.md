---
title: Pemilik tidak dapat membuat sub-folder menggunakan Outlook
ms.author: pebaum
author: pebaum
manager: mnirkhe
ms.date: 04/21/2020
ms.audience: Admin
ms.topic: article
ROBOTS: NOINDEX, NOFOLLOW
localization_priority: Priority
ms.collection: Adm_O365
ms.custom:
- "5884"
- "3500007"
ms.openlocfilehash: 2116bb837e4378ea29d7882df1d3010b3a4e0b1c
ms.sourcegitcommit: 936330b11fec49f6174eadea6c765bdf9e6ba784
ms.translationtype: MT
ms.contentlocale: id-ID
ms.lasthandoff: 06/12/2020
ms.locfileid: "44749148"
---
# <a name="owner-cannot-create-sub-folder-using-outlook"></a>Pemilik tidak dapat membuat sub-folder menggunakan Outlook

**Ada masalah yang sedang berlangsung dengan pemilik folder publik yang membuat subfolder menggunakan Outlook. Masalah akan segera diperbaiki.**

Sementara itu, gunakan salah satu dari penyelesaian berikut:

1. Menggunakan Outlook untuk MAC untuk membuat subfolder sebagai masalah dampak hanya Outlook untuk Windows Desktop (semua versi)
2. Memiliki admin membuat subfolder menggunakan EXO shell atau EAC
3. Mengubah DefaultPublicFolderMailbox/EffectivePublicFolderMailbox di pengguna ke kotak surat lainnya dari kotak surat konten untuk folder yang menyebabkan masalah  
    - *Set-kotak surat User1 DefaultPublicFolderMailbox PubMBX3*
4. Tunggu selama satu jam, mulai ulang klien Outlook