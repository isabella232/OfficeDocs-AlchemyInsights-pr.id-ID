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
ms.openlocfilehash: b72b7c93ce9fe1b90d1608811b0eeabc8aec1363
ms.sourcegitcommit: a5edaaefdc56f8d5c8220a335f4e8228e2de4ee0
ms.translationtype: MT
ms.contentlocale: id-ID
ms.lasthandoff: 04/08/2021
ms.locfileid: "51645134"
---
# <a name="restore-a-deleted-microsoft-365-group"></a>Memulihkan grup Microsoft 365 yang dihapus

Anda dapat memulihkan grup Microsoft 365 yang dihapus atau Microsoft Teams dalam 30 hari dari penghapusan.

1. Masuk ke [pusat admin Microsoft 365](https://aka.ms/RestoreDeletedGroup) untuk masuk ke daftar tentang grup dan tim yang dihapus.

    **Catatan:** Masuk menggunakan akun yang ditetapkan untuk administrator penyewa atau peran admin grup.

1. Pilih grup/Teams Microsoft 365 yang dihapus untuk dipulihkan, lalu klik **pulihkan grup.**

    Jika grup tidak bisa dipulihkan karena alamat SMTP yang berkonflik, gunakan perintah berikut untuk menemukan objek yang menyebabkan konflik dan menghapus alamat SMTP:

    `Get-Recipient -Filter "EmailAddresses -eq '<conflictingsmtpaddress>'"`

    **Catatan:** Dalam beberapa kasus, mungkin akan memakan waktu hingga 24 jam agar grup dan semua datanya dipulihkan.

    Untuk informasi selengkapnya, atau untuk mempelajari cara memulihkan grup menggunakan PowerShell, [lihat Memulihkan grup Microsoft 365 yang dihapus.](https://go.microsoft.com/fwlink/?linkid=867802)