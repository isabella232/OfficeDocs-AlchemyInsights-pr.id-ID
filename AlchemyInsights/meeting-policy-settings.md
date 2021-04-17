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
ms.openlocfilehash: 39151d3a56cc09a8ae2dd77fb7bf1e99066cc77a
ms.sourcegitcommit: 8bc60ec34bc1e40685e3976576e04a2623f63a7c
ms.translationtype: MT
ms.contentlocale: id-ID
ms.lasthandoff: 04/15/2021
ms.locfileid: "51825446"
---
# <a name="manage-meeting-policies-in-microsoft-teams"></a>Mengelola kebijakan rapat di Microsoft Teams

**Catatan: Perubahan kebijakan dapat memakan waktu hingga 24 jam agar dapat diterapkan bagi pengguna.** Anda mungkin tidak bisa membuat perubahan ke kebijakan yang baru dibuat dengan segera; tunggu 4 jam dan coba mengubah kebijakan yang baru dibuat lagi.

Kebijakan rapat digunakan untuk mengontrol fitur yang tersedia bagi peserta rapat untuk rapat yang dijadwalkan oleh pengguna di organisasi Anda. Beberapa fitur kebijakan rapat mungkin belum diterapkan di pusat admin Teams (fitur ini diberi label "segera hadir" dalam dokumentasi). Dalam hal ini, atau jika mendapatkan kesalahan seperti "Kami tidak dapat memperbarui kebijakan saat ini, tetapi coba lagi nanti" di pusat admin Microsoft Teams, sebaiknya gunakan PowerShell untuk membuat atau mengubah kebijakan rapat Teams. 

Untuk informasi selengkapnya tentang kebijakan rapat, lihat sumber daya berikut ini:

- Untuk mempelajari tentang membuat kebijakan, membuat perubahan, dan menetapkan pengguna ke kebijakan, lihat [Mengelola kebijakan rapat di Teams](https://docs.microsoft.com/microsoftteams/meeting-policies-in-teams).

- Untuk membuat perubahan kebijakan menggunakan cmdlet PowerShell, lihat [Gambaran Umum PowerShell Teams.](https://docs.microsoft.com/microsoftteams/teams-powershell-overview) 
    - Anda perlu menggunakan modul [PowerShell Skype for Business untuk](https://docs.microsoft.com/skypeforbusiness/set-up-your-computer-for-windows-powershell/download-and-install-the-skype-for-business-online-connector) kebijakan rapat Teams. 
    - Tinjau [dokumentasi cmdlet *-CsTeamsMeetingPolicy](https://docs.microsoft.com/search/?search=CsTeamsMeetingPolicy&view=skype-ps) untuk informasi selengkapnya.

