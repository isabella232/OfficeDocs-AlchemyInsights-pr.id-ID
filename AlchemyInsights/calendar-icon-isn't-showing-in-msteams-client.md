---
title: Ikon kalender tidak ditampilkan di klien Microsoft teams
ms.author: v-aiyengar
author: AshaIyengar21
manager: dansimp
ms.date: 12/05/2020
ms.audience: Admin
ms.topic: article
ms.service: o365-administration
ROBOTS: NOINDEX, NOFOLLOW
localization_priority: Normal
ms.collection: Adm_O365
ms.custom:
- "9001219"
- "6794"
- "3403"
ms.openlocfilehash: e28b1c8d5d0feef1a743c8527db424af4c205fe9
ms.sourcegitcommit: 2e4a5153e530bf15744a52e982eeb0d99757e9d2
ms.translationtype: MT
ms.contentlocale: id-ID
ms.lasthandoff: 12/04/2020
ms.locfileid: "49583534"
---
# <a name="calendar-icon-isnt-showing-in-microsoft-teams-client"></a>Ikon kalender tidak ditampilkan di klien Microsoft teams

Tab **kalender** di teams memerlukan akses ke kotak surat Exchange melalui layanan web Exchange. Kotak surat Exchange bisa online, atau di tempat. Untuk pengguna online yang tidak melihat tab **kalender** , pastikan mereka [dilisensikan untuk kotak surat Exchange Online dan kotak surat diaktifkan](https://docs.microsoft.com/exchange/recipients-in-exchange-online/create-user-mailboxes). Jika pengguna Anda berada di tempat, Anda perlu mengonfirmasi bahwa konfigurasi hibrid Anda sehat. Gunakan [Panduan Konfigurasi Hibrid](https://docs.microsoft.com/exchange/hybrid-deployment/hybrid-agent) untuk memecahkan masalah. Perhatikan bahwa [Teams membutuhkan Exchange 2016 CU3 atau lebih tinggi](https://docs.microsoft.com/microsoftteams/exchange-teams-interact).

Untuk informasi selengkapnya dan langkah pemecahan masalah, lihat [memecahkan masalah interaksi Microsoft teams dan server Exchange](https://docs.microsoft.com/microsoftteams/troubleshoot/known-issues/teams-exchange-interaction-issue).
