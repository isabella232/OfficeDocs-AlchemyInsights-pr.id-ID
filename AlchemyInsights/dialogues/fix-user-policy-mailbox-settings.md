---
title: Memperbaiki pengaturan kebijakan pengguna/kotak surat
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
ms.openlocfilehash: ca998c453fcb0905b122436f0eea384a9b8a9992
ms.sourcegitcommit: bd6a9cb5d357baee5134c0dea430afc2a035c810
ms.translationtype: MT
ms.contentlocale: id-ID
ms.lasthandoff: 03/09/2021
ms.locfileid: "50694173"
---
# <a name="fix-user-policymailbox-settings"></a>Memperbaiki pengaturan kebijakan pengguna/kotak surat

Pengaturan email sampah pada kotak surat terpengaruh pesan ini. Untuk meninjau pengaturan, lakukan hal berikut:

1. Luncurkan Exchange Management Shell. Untuk informasi selengkapnya, lihat [membuka Exchange Management Shell](https://go.microsoft.com/fwlink/?linkid=2101432).
2. Jalankan perintah ini (menggunakan alamat email pengguna):  **Get-mailboxjunkmailconfiguration-Identity "user@domain.com"**
3. Periksa apakah alamat email pengirim adalah bagian dari **Trustedsendersanddomains** atau **blockedsendersanddomains**. Jika alamat email berada dalam salah satu daftar, Anda mungkin harus menghapusnya. Untuk mempelajari selengkapnya, lihat [set-MailboxJunkEmailConfiguration](https://go.microsoft.com/fwlink/?linkid=2101047).
