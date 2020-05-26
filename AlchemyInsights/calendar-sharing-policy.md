---
title: 618 kebijakan berbagi kalender
ms.author: chrisda
author: chrisda
manager: scotv
ms.date: 04/21/2020
ms.audience: Admin
ms.topic: article
ROBOTS: NOINDEX, NOFOLLOW
localization_priority: Normal
ms.collection: Adm_O365
ms.custom:
- "618"
- "899"
- "3800014"
ms.assetid: bc3db17b-87f8-4e50-b3ee-8b105b70d67a
ms.openlocfilehash: cc5827975eff10a119281541622224d0e37f08a7
ms.sourcegitcommit: 2afad0b107d03cd8c4de0b85b5bee38a13a7960d
ms.translationtype: MT
ms.contentlocale: id-ID
ms.lasthandoff: 05/26/2020
ms.locfileid: "44373002"
---
# <a name="policy-error-when-sharing-a-calendar"></a>Galat kebijakan saat berbagi kalender

1. Lakukan salah satu dari berikut ini, yang sesuai untuk situasi Anda:
    - Menyambung ke Exchange Online menggunakan PowerShell jarak jauh. Untuk informasi selengkapnya, lihat [tersambung ke Exchange Online menggunakan PowerShell jarak jauh](https://technet.microsoft.com/library/jj984289%28v=exchg.160%29.aspx).
    - Di server lokal, buka Exchange Management Shell.
2. Menentukan kebijakan berbagi yang ditetapkan untuk pengguna. Untuk melakukannya, jalankan perintah berikut ini dan catat kebijakan yang dikembalikan:

    `
    Get-Mailbox User1 | fl *sharing*
    `

3. Memperbarui kebijakan berbagi untuk pengguna. Untuk melakukan ini, ikuti langkah berikut:
    - Buka Pusat admin Exchange.
    - Klik **organisasi**, dan kemudian klik dua kali kebijakan yang ditetapkan untuk pengguna di bawah masing- **masing berbagi**. Ini adalah kebijakan yang dikembalikan di langkah 2.
    - Pada halaman aturan berbagi, pilih tingkat berbagi kalender yang ingin Anda Izinkan di bawah **menentukan informasi apa yang Anda ingin berbagi**; Klik **Simpan**.

Untuk informasi selengkapnya, lihat: ["kebijakan tidak mengizinkan memberikan izin pada tingkat ini ke satu atau lebih Penerima" galat saat pengguna berusaha berbagi kalender](https://docs.microsoft.com/exchange/troubleshoot/calendar-sharing/policy-permissions-issue).
