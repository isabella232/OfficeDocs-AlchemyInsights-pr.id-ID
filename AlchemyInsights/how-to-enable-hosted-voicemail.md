---
title: Cara mengaktifkan Pesan Suara yang Dihosting
ms.author: v-aiyengar
author: AshaIyengar21
manager: dansimp
ms.date: 12/09/2020
ms.audience: Admin
ms.topic: article
ms.service: o365-administration
ROBOTS: NOINDEX, NOFOLLOW
localization_priority: Normal
ms.collection: Adm_O365
ms.custom:
- "9002347"
- "7563"
ms.openlocfilehash: 4d70e92a7c1bf8f3cc62d4a310aa140ee2dfdef4c798ae17faa961736d9db500
ms.sourcegitcommit: b5f7da89a650d2915dc652449623c78be6247175
ms.translationtype: MT
ms.contentlocale: id-ID
ms.lasthandoff: 08/05/2021
ms.locfileid: "54055557"
---
# <a name="how-to-enable-hosted-voicemail"></a>Cara mengaktifkan Pesan Suara yang Dihosting

Untuk mengaktifkan Pesan Suara, **HostedVoicemail** harus diatur ke $true.

Properti **HostedVoicemail** pada pengguna menggunakan Remote PowerShell (RPS).

Untuk informasi selengkapnya tentang menyambungkan ke RPS, lihat Microsoft Teams Gambaran Umum [PowerShell](https://docs.microsoft.com/microsoftteams/teams-powershell-overview) untuk informasi selengkapnya tentang menyambungkan ke RPS.

1. Admin Teams harus masuk ke PowerShell Jarak Jauh untuk Teams.
1. Dari perintah PowerShell, Admin Teams dapat menjalankan **user@contoso.com set-csuser -HostedVoiceMail $true** tempat sip uri adalah pengguna yang dimaksud.

> [!NOTE]
> Perubahan pada kebijakan bisa memakan waktu hingga 24 jam untuk direplikasi.