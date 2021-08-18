---
title: Ikon Kalender tidak muncul di Microsoft Teams klien
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
ms.openlocfilehash: edd6b4a2d94b03cf4ae7bf3a8d6332ed94a7e8263aba9df1f9588eecbd0ce05a
ms.sourcegitcommit: b5f7da89a650d2915dc652449623c78be6247175
ms.translationtype: MT
ms.contentlocale: id-ID
ms.lasthandoff: 08/05/2021
ms.locfileid: "54120007"
---
# <a name="calendar-icon-isnt-showing-in-microsoft-teams-client"></a>Ikon Kalender tidak muncul di Microsoft Teams klien

Tab **Kalender** di Teams memerlukan akses ke kotak Exchange email melalui Exchange Web Services. Kotak Exchange anda bisa Online, atau Di Tempat. Bagi pengguna Online yang tidak melihat Tab **Kalender,** pastikan mereka memiliki lisensi untuk kotak [Exchange Online dan kotak surat diaktifkan.](https://docs.microsoft.com/exchange/recipients-in-exchange-online/create-user-mailboxes) Jika pengguna berada di Tempat, Anda perlu mengonfirmasi bahwa konfigurasi Hibrid sehat. Gunakan [Panduan Konfigurasi Hibrid](https://docs.microsoft.com/exchange/hybrid-deployment/hybrid-agent) untuk memecahkan masalah. Perhatikan bahwa [Teams membutuhkan Exchange 2016 CU3 atau lebih tinggi](https://docs.microsoft.com/microsoftteams/exchange-teams-interact).

Untuk informasi selengkapnya dan langkah-langkah pemecahan masalah, [lihat Microsoft Teams dan Server Exchange interaksi mereka.](https://docs.microsoft.com/microsoftteams/troubleshoot/known-issues/teams-exchange-interaction-issue)
