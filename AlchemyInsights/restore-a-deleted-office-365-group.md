---
title: Memulihkan grup Microsoft 365 yang dihapus
ms.author: pebaum
author: pebaum
manager: scotv
ms.date: 04/21/2020
ms.audience: Admin
ms.topic: article
ms.service: o365-administration
ROBOTS: NOINDEX, NOFOLLOW
localization_priority: Normal
ms.collection: Adm_O365
ms.custom:
- "98"
- "1200024"
ms.assetid: bc0396ea-c426-4d1d-bb89-ced602d06fb6
ms.openlocfilehash: 6262ca04335c355fb4de41a9e1d854b666f47e10321a843717d6eb951c46cafd
ms.sourcegitcommit: b5f7da89a650d2915dc652449623c78be6247175
ms.translationtype: MT
ms.contentlocale: id-ID
ms.lasthandoff: 08/05/2021
ms.locfileid: "53959029"
---
# <a name="restore-a-deleted-microsoft-365-group"></a>Memulihkan grup Microsoft 365 yang dihapus

Anda dapat memulihkan grup Microsoft 365 yang Microsoft Teams dalam 30 hari dari penghapusan.

1. Masuk ke [pusat admin Microsoft 365](https://aka.ms/RestoreDeletedGroup) untuk masuk ke daftar anda adalah grup dan tim yang dihapus.

    **Catatan:** Masuk menggunakan akun yang ditetapkan untuk administrator penyewa atau peran admin grup.

1. Pilih grup Microsoft 365 yang Teams akan dipulihkan dan klik **pulihkan grup.**

    Jika grup tidak bisa dipulihkan karena alamat SMTP yang berkonflik, gunakan perintah berikut untuk menemukan objek yang menyebabkan konflik dan menghapus alamat SMTP:

    `Get-Recipient -Filter "EmailAddresses -eq '<conflictingsmtpaddress>'"`

    **Catatan:** Dalam beberapa kasus, mungkin akan memakan waktu hingga 24 jam agar grup dan semua datanya dipulihkan.

    Untuk informasi selengkapnya, atau untuk mempelajari cara memulihkan grup menggunakan PowerShell, [lihat Memulihkan Microsoft 365 yang dihapus](https://go.microsoft.com/fwlink/?linkid=867802).