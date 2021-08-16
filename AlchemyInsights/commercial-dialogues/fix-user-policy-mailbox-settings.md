---
title: Memperbaiki pengaturan kebijakan/kotak surat pengguna
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
ms.openlocfilehash: fecc52bea66e0aed709a8995d2509f4432c09482459aa575d29e4c7551375211
ms.sourcegitcommit: b5f7da89a650d2915dc652449623c78be6247175
ms.translationtype: MT
ms.contentlocale: id-ID
ms.lasthandoff: 08/05/2021
ms.locfileid: "54034721"
---
# <a name="fix-user-policymailbox-settings"></a>Memperbaiki pengaturan kebijakan/kotak surat pengguna

Pengaturan email sampah pada kotak surat memengaruhi pesan ini. Untuk meninjau pengaturan, lakukan hal berikut:

1. Luncurkan Exchange Shell Manajemen. Untuk informasi selengkapnya, [lihat Membuka Exchange Management Shell](https://go.microsoft.com/fwlink/?linkid=2101432).
2. Jalankan perintah ini (menggunakan alamat email pengguna):  **get-mailboxjunkmailconfiguration -identity "user@domain.com"**
3. Periksa apakah alamat email pengirim merupakan bagian dari **TrustedSendersAndDomains** atau **BlockedSendersAndDomains**. Jika alamat email berada di salah satu daftar, Anda mungkin harus menghapusnya. Untuk mempelajari selengkapnya, lihat [Set-MailboxJunkEmailConfiguration](https://go.microsoft.com/fwlink/?linkid=2101047).
