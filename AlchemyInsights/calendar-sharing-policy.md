---
title: Kebijakan berbagi kalender 618
ms.author: chrisda
author: chrisda
manager: scotv
ms.date: 04/21/2020
ms.audience: Admin
ms.topic: article
ms.service: o365-administration
ROBOTS: NOINDEX, NOFOLLOW
localization_priority: Normal
ms.collection: Adm_O365
ms.custom:
- "618"
- "899"
- "3800014"
ms.assetid: bc3db17b-87f8-4e50-b3ee-8b105b70d67a
ms.openlocfilehash: d2511183d068330cdcfb4e08b08df4f18625c822
ms.sourcegitcommit: c6692ce0fa1358ec3529e59ca0ecdfdea4cdc759
ms.translationtype: MT
ms.contentlocale: id-ID
ms.lasthandoff: 09/14/2020
ms.locfileid: "47684233"
---
# <a name="policy-error-when-sharing-a-calendar"></a>Kesalahan kebijakan saat berbagi kalender

1. Lakukan salah satu hal berikut ini, yang sesuai untuk situasi Anda:
    - Menyambungkan ke Exchange Online menggunakan PowerShell jarak jauh. Untuk informasi selengkapnya, lihat [menyambungkan ke Exchange Online menggunakan PowerShell jarak jauh](https://technet.microsoft.com/library/jj984289%28v=exchg.160%29.aspx).
    - Di server lokal, buka Exchange Management Shell.
2. Menentukan kebijakan berbagi yang ditetapkan untuk pengguna. Untuk melakukan ini, jalankan perintah berikut ini dan catat kebijakan yang dikembalikan:

    `
    Get-Mailbox User1 | fl *sharing*
    `

3. Memperbarui kebijakan berbagi untuk pengguna. Untuk melakukan ini, ikuti langkah berikut:
    - Buka Pusat admin Exchange.
    - Klik **organisasi**, lalu klik dua kali kebijakan yang ditetapkan untuk pengguna di bawah **masing-masing berbagi**. Ini adalah kebijakan yang dikembalikan di langkah 2.
    - Pada halaman aturan berbagi, pilih tingkat berbagi kalender yang ingin Anda Izinkan di bawah **tentukan informasi apa yang ingin Anda bagikan**; Klik **Simpan**.

Untuk informasi selengkapnya, lihat: ["kebijakan tidak memperbolehkan pemberian izin pada tingkat ini ke satu atau beberapa penerima pesan kesalahan" ketika pengguna mencoba berbagi kalender](https://docs.microsoft.com/exchange/troubleshoot/calendar-sharing/policy-permissions-issue).
