---
title: Pengaturan kebijakan Rapat
ms.author: pebaum
author: pebaum
manager: mnirkhe
ms.audience: Admin
ms.topic: article
ms.service: o365-administration
ROBOTS: NOINDEX, NOFOLLOW
localization_priority: Normal
ms.collection: Adm_O365
ms.custom:
- "9000734"
- "2657"
ms.openlocfilehash: 24a55417df0f89063fbdd9ade6d104be4f8ab49c
ms.sourcegitcommit: 0eb4f9bde53395b5fd4b5cd4ffc56ca96db91298
ms.translationtype: MT
ms.contentlocale: id-ID
ms.lasthandoff: 03/10/2021
ms.locfileid: "50704609"
---
# <a name="manage-meeting-policies-in-microsoft-teams"></a>Mengelola Kebijakan Rapat di Microsoft teams

**Catatan: perlu waktu hingga 24 jam agar perubahan kebijakan diterapkan untuk pengguna.** Anda mungkin tidak dapat membuat perubahan pada kebijakan yang baru dibuat segera; Tunggu 4 jam dan coba Ubah kembali kebijakan yang baru dibuat.

Kebijakan Rapat digunakan untuk mengontrol fitur yang tersedia bagi peserta rapat untuk Rapat yang dijadwalkan oleh pengguna di organisasi Anda. Beberapa fitur kebijakan Rapat mungkin tidak diterapkan di pusat admin teams (yang disebut "segera hadir" di dokumentasi). Dalam kasus ini, atau jika Anda mendapatkan kesalahan seperti "kami tidak dapat memperbarui kebijakan sekarang tapi mencobanya lagi nanti" di pusat admin Microsoft teams, kami menyarankan agar Anda menggunakan PowerShell untuk membuat atau mengubah kebijakan Rapat teams. 

Untuk informasi selengkapnya tentang kebijakan Rapat, lihat sumber daya berikut ini:

- Untuk mempelajari tentang membuat kebijakan, membuat perubahan, dan menetapkan pengguna ke kebijakan, lihat [mengelola kebijakan Rapat di teams](https://docs.microsoft.com/microsoftteams/meeting-policies-in-teams).

- Untuk membuat perubahan kebijakan menggunakan cmdlet PowerShell, lihat [gambaran umum PowerShell teams](https://docs.microsoft.com/microsoftteams/teams-powershell-overview). 
    - Anda perlu menggunakan [modul PowerShell untuk Rapat Skype for Business](https://docs.microsoft.com/skypeforbusiness/set-up-your-computer-for-windows-powershell/download-and-install-the-skype-for-business-online-connector) . 
    - Tinjau [dokumentasi cmdlet *-csteamsmeetingpolicy](https://docs.microsoft.com/search/?search=CsTeamsMeetingPolicy&view=skype-ps) untuk informasi selengkapnya.

