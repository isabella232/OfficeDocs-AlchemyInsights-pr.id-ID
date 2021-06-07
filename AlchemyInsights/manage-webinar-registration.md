---
title: Mengelola pendaftaran webinar
ms.author: pebaum
author: pebaum
manager: scotv
ms.date: 06/02/2021
ms.audience: Admin
ms.topic: article
ms.service: o365-administration
ROBOTS: NOINDEX, NOFOLLOW
localization_priority: Priority
ms.collection: Adm_O365
ms.custom:
- "11512"
- "9006672"
ms.openlocfilehash: c5b0721d286b07d7e0f84199885b6f527a2b42a2
ms.sourcegitcommit: f7a9e97d04b7b6cbb633b32094d40f1874bf0fce
ms.translationtype: HT
ms.contentlocale: id-ID
ms.lasthandoff: 06/06/2021
ms.locfileid: "52793916"
---
# <a name="manage-webinar-registration"></a>Mengelola pendaftaran webinar

Anda mengelola siapa yang bisa mendaftar Teams Webinar gratis dengan Teams Perintah Powershell. Untuk menginstal Teams Powershell, lihat [Teams PowerShell](/microsoftteams/teams-powershell-install). 

Secara default, *WhoCanRegister* diaktifkan dan diatur ke **EveryoneInCompany**. Untuk memperbolehkan siapa saja, termasuk pengguna anonim, untuk mendaftar, Anda harus menyetel Kebijakan Rapat ke **Setiap** Orang dengan menggunakan perintah Powershell:

`Set-CsTeamsMeetingPolicy -WhoCanRegister Everyone`

**Catatan**: Jika bergabung anonim dinonaktifkan dalam pengaturan rapat, pengguna anonim tidak dapat bergabung dalam webinar. Untuk mempelajari selengkapnya dan mengaktifkan pengaturan ini, lihat [Mengelola pengaturan rapat di Microsoft Teams](/microsoftteams/meeting-settings-in-teams).

Jika Anda ingin menonaktifkan pendaftaran rapat, atur *AllowMeetingRegistration* ke **False.**

Untuk mempelajari selengkapnya tentang mengonfigurasi siapa yang bisa mendaftar untuk webinar, lihat [Mengonfigurasi siapa yang bisa mendaftar untuk webinar.](/microsoftteams/set-up-webinars?source=docs#configure-who-can-register-for-webinars) Untuk informasi selengkapnya tentang pengaturan untuk Microsoft Lists, lihat [Pengaturan kontrol untuk Daftar Microsoft.](/sharepoint/control-lists)
