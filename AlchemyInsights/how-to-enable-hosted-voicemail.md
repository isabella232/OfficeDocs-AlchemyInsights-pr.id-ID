---
title: Cara mengaktifkan pesan suara yang dihosting
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
ms.openlocfilehash: 26eb22054d246a6ca5a2491c68a5d9e4ed90d45b
ms.sourcegitcommit: 523098560e54a50184a99c974809dfbfffadacb5
ms.translationtype: MT
ms.contentlocale: id-ID
ms.lasthandoff: 12/09/2020
ms.locfileid: "49677998"
---
# <a name="how-to-enable-hosted-voicemail"></a>Cara mengaktifkan pesan suara yang dihosting

Untuk mengaktifkan pesan suara, **Hostedvoicemail** harus diatur ke $True.

Properti **Hostedvoicemail** pada pengguna menggunakan PowerShell jarak jauh (RPS).

Untuk informasi selengkapnya tentang menyambungkan ke RPS, lihat [gambaran umum Microsoft teams PowerShell](https://docs.microsoft.com/microsoftteams/teams-powershell-overview) untuk informasi selengkapnya tentang menyambungkan ke RPS.

1. Admin teams harus masuk ke PowerShell jarak jauh untuk teams.
1. Dari wantian perintah, admin teams dapat menjalankan **set-csuser user@contoso.com-HostedVoiceMail $True** tempat SIP URI berasal dari pengguna yang bersangkutan.

> [!NOTE]
> Perubahan pada kebijakan dapat memakan waktu hingga 24 jam untuk meniru.