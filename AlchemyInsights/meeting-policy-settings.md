---
title: Pengaturan kebijakan Rapat
ms.author: pebaum
author: pebaum
manager: mnirkhe
ms.audience: Admin
ms.topic: article
ROBOTS: NOINDEX, NOFOLLOW
localization_priority: Normal
ms.collection: Adm_O365
ms.custom:
- "2657"
- "9000734"
ms.openlocfilehash: dac06690b51459ca166c15a5ef0f4c7e7a6d36f0
ms.sourcegitcommit: 0495112ad4fd0e695140ec66d190e62f03030584
ms.translationtype: MT
ms.contentlocale: id-ID
ms.lasthandoff: 10/02/2019
ms.locfileid: "37376688"
---
# <a name="manage-meeting-policies-in-microsoft-teams"></a>Mengelola Kebijakan Rapat di Microsoft teams

Kebijakan Rapat digunakan untuk mengontrol fitur yang tersedia untuk Rapat peserta pertemuan yang dijadwalkan oleh pengguna di organisasi Anda. Beberapa fitur kebijakan Rapat mungkin tidak diimplementasikan di pusat admin teams (ini diberi label "segera hadir" dalam dokumentasi). Dalam hal ini, atau jika Anda menerima pesan kesalahan seperti "kami tidak dapat memperbarui kebijakan sekarang, namun coba lagi nanti" di pusat admin Microsoft teams, sebaiknya gunakan PowerShell untuk membuat atau memodifikasi Kebijakan Rapat tim. 

Untuk informasi selengkapnya tentang kebijakan Rapat, lihat sumber daya berikut ini:

- Untuk mempelajari tentang membuat kebijakan, membuat perubahan, dan menetapkan pengguna ke kebijakan, lihat [mengelola kebijakan Rapat di teams](https://docs.microsoft.com/en-us/microsoftteams/meeting-policies-in-teams).

- Untuk membuat perubahan kebijakan menggunakan cmdlet PowerShell, lihat [ringkasan tim PowerShell](https://docs.microsoft.com/microsoftteams/teams-powershell-overview). 
    - Anda harus menggunakan [modul Skype for Business PowerShell](https://www.microsoft.com/download/details.aspx?id=39366) untuk kebijakan Rapat tim. 
    - Meninjau [*-csteamsmeetingpolicy cmdlet dokumentasi](https://docs.microsoft.com/search/?search=CsTeamsMeetingPolicy&view=skype-ps) untuk informasi lebih lanjut.

**Catatan:** Diperlukan waktu hingga 24 jam agar perubahan kebijakan diterapkan bagi pengguna. Anda mungkin tidak dapat membuat perubahan pada kebijakan yang baru dibuat dengan segera; menunggu 4 jam dan mencoba untuk mengubah kebijakan baru dibuat lagi. Jika Anda masih mengalami masalah, coba PowerShell.  