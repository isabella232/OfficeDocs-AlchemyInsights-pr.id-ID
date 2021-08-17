---
title: 618 Kebijakan Berbagi Kalender
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
ms.openlocfilehash: 1f1bfb0273301c05f5fe5f8af5fb9039328390d16305e33897680dce1c1977e8
ms.sourcegitcommit: b5f7da89a650d2915dc652449623c78be6247175
ms.translationtype: MT
ms.contentlocale: id-ID
ms.lasthandoff: 08/05/2021
ms.locfileid: "54091606"
---
# <a name="policy-error-when-sharing-a-calendar"></a>Kesalahan kebijakan saat berbagi kalender

1. Lakukan salah satu hal berikut, yang sesuai dengan situasi Anda:
    - Koneksi ke Exchange Online dengan menggunakan Remote PowerShell. Untuk informasi selengkapnya, lihat [Koneksi cara Exchange Online menggunakan Remote PowerShell](https://technet.microsoft.com/library/jj984289%28v=exchg.160%29.aspx).
    - Di server lokal, buka Exchange Management Shell.
2. Menentukan kebijakan berbagi yang ditetapkan kepada pengguna. Untuk melakukan ini, jalankan perintah berikut ini dan perhatikan kebijakan yang dikembalikan:

    `
    Get-Mailbox User1 | fl *sharing*
    `

3. Memperbarui kebijakan berbagi untuk pengguna. Untuk melakukan ini, ikuti langkah berikut:
    - Buka Exchange admin baru.
    - Klik **Organisasi,** lalu klik ganda kebijakan yang ditetapkan kepada pengguna di bawah **Berbagi Individual.** Ini adalah kebijakan yang dikembalikan di langkah 2.
    - Di halaman Aturan Berbagi, pilih tingkat berbagi kalender yang ingin Anda perbolehkan di **bawah Tentukan informasi apa yang ingin Anda bagikan;** klik **Simpan.**

Untuk informasi selengkapnya, lihat: Kesalahan "Kebijakan tidak mengizinkan pemberian izin pada tingkat ini untuk satu atau beberapa penerima" ketika pengguna [mencoba untuk berbagi kalender.](https://docs.microsoft.com/exchange/troubleshoot/calendar-sharing/policy-permissions-issue)
