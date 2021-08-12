---
title: Pengaturan kebijakan rapat
ms.author: pebaum
author: pebaum
manager: scotv
ms.audience: Admin
ms.topic: article
ms.service: o365-administration
ROBOTS: NOINDEX, NOFOLLOW
localization_priority: Normal
ms.collection: Adm_O365
ms.custom:
- "9000734"
- "2657"
ms.openlocfilehash: 06395bcc1a631adeaa8abb5ad63b971639f226c19e48203078ba1097d43a50f8
ms.sourcegitcommit: b5f7da89a650d2915dc652449623c78be6247175
ms.translationtype: MT
ms.contentlocale: id-ID
ms.lasthandoff: 08/05/2021
ms.locfileid: "53925168"
---
# <a name="manage-meeting-policies-in-microsoft-teams"></a>Mengelola kebijakan rapat di Microsoft Teams

**Catatan: Perubahan kebijakan dapat memakan waktu hingga 24 jam agar dapat diterapkan bagi pengguna.** Anda mungkin tidak bisa membuat perubahan ke kebijakan yang baru dibuat dengan segera; tunggu 4 jam dan coba mengubah kebijakan yang baru dibuat lagi.

Kebijakan rapat digunakan untuk mengontrol fitur yang tersedia bagi peserta rapat untuk rapat yang dijadwalkan oleh pengguna di organisasi Anda. Beberapa fitur kebijakan rapat mungkin belum diterapkan di pusat admin Teams (dilabeli "segera hadir" dalam dokumentasi). Dalam kasus ini, atau jika Mendapatkan kesalahan seperti "Kami tidak dapat memperbarui kebijakan saat ini tetapi coba lagi nanti" di pusat admin Microsoft Teams, kami menyarankan agar Anda menggunakan PowerShell untuk membuat atau Teams kebijakan rapat. 

Untuk informasi selengkapnya tentang kebijakan rapat, lihat sumber daya berikut ini:

- Untuk mempelajari tentang membuat kebijakan, membuat perubahan, dan menetapkan pengguna ke kebijakan, lihat [Mengelola kebijakan rapat di Teams](https://docs.microsoft.com/microsoftteams/meeting-policies-in-teams).

- Untuk membuat perubahan kebijakan menggunakan cmdlet PowerShell, lihat [Teams Umum PowerShell](https://docs.microsoft.com/microsoftteams/teams-powershell-overview). 
    - Anda harus menggunakan modul [Skype for Business PowerShell](https://docs.microsoft.com/skypeforbusiness/set-up-your-computer-for-windows-powershell/download-and-install-the-skype-for-business-online-connector) untuk Teams rapat. 
    - Tinjau [dokumentasi cmdlet *-CsTeamsMeetingPolicy](https://docs.microsoft.com/search/?search=CsTeamsMeetingPolicy&view=skype-ps) untuk informasi selengkapnya.

