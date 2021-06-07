---
title: Mengaktifkan Teams Webinar Baru
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
- "11513"
- "9006672"
ms.openlocfilehash: 5a732e6746e9fd23e54a0b2ffeabb59623012a0e
ms.sourcegitcommit: 9de78b30602f917d58705057cdcce31fec349969
ms.translationtype: MT
ms.contentlocale: id-ID
ms.lasthandoff: 06/04/2021
ms.locfileid: "52793787"
---
# <a name="enable-teams-webinars"></a>Mengaktifkan Teams Webinar Baru

Webinar diaktifkan secara default. Anda bisa mengelola siapa yang bisa menjadwalkan dan mendaftar Teams Webinar dengan menggunakan Teams PowerShell.

- Semua pengguna yang bisa membuat rapat juga bisa membuat rapat webinar. Jika Anda ingin mengelola siapa yang bisa menjadwalkan Teams Webinar, gunakan *AllowMeetingRegistration.* 
- Secara default, *WhoCanRegister* diaktifkan dan diatur ke **Semua Orang.** Jika Anda ingin menonaktifkan pendaftaran rapat, atur *AllowMeetingRegistration* ke **False.**

Untuk mengubah pengaturan ini, Anda harus menginstal [Teams PowerShell](/microsoftteams/teams-powershell-install). Juga, Kebijakan Rapat diberlakukan di Teams Webinar. Misalnya, jika ikut anonim dinonaktifkan di pengaturan rapat, pengguna anonim tidak bisa bergabung dalam webinar.

Untuk mempelajari selengkapnya tentang mengonfigurasi siapa yang bisa mendaftar untuk webinar, lihat [Mengonfigurasi siapa yang bisa mendaftar untuk webinar.](/microsoftteams/set-up-webinars?source=docs#configure-who-can-register-for-webinars) Untuk informasi selengkapnya tentang pengaturan untuk Microsoft Lists, lihat [Pengaturan kontrol untuk Daftar Microsoft.](/sharepoint/control-lists)