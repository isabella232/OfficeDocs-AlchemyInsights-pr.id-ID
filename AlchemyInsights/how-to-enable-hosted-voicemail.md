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
# <a name="how-to-enable-hosted-voicemail"></a><span data-ttu-id="f3c6b-102">Cara mengaktifkan pesan suara yang dihosting</span><span class="sxs-lookup"><span data-stu-id="f3c6b-102">How to enable Hosted Voicemail</span></span>

<span data-ttu-id="f3c6b-103">Untuk mengaktifkan pesan suara, **Hostedvoicemail** harus diatur ke $True.</span><span class="sxs-lookup"><span data-stu-id="f3c6b-103">To enable Voicemail, **HostedVoicemail** must be set to $true.</span></span>

<span data-ttu-id="f3c6b-104">Properti **Hostedvoicemail** pada pengguna menggunakan PowerShell jarak jauh (RPS).</span><span class="sxs-lookup"><span data-stu-id="f3c6b-104">The **HostedVoicemail** property on the user using Remote PowerShell (RPS).</span></span>

<span data-ttu-id="f3c6b-105">Untuk informasi selengkapnya tentang menyambungkan ke RPS, lihat [gambaran umum Microsoft teams PowerShell](https://docs.microsoft.com/microsoftteams/teams-powershell-overview) untuk informasi selengkapnya tentang menyambungkan ke RPS.</span><span class="sxs-lookup"><span data-stu-id="f3c6b-105">For more information on connecting to RPS, see [Microsoft Teams PowerShell Overview](https://docs.microsoft.com/microsoftteams/teams-powershell-overview) for more information on connecting to RPS.</span></span>

1. <span data-ttu-id="f3c6b-106">Admin teams harus masuk ke PowerShell jarak jauh untuk teams.</span><span class="sxs-lookup"><span data-stu-id="f3c6b-106">The Teams Admin should be logged into Remote PowerShell for Teams.</span></span>
1. <span data-ttu-id="f3c6b-107">Dari wantian perintah, admin teams dapat menjalankan **set-csuser user@contoso.com-HostedVoiceMail $True** tempat SIP URI berasal dari pengguna yang bersangkutan.</span><span class="sxs-lookup"><span data-stu-id="f3c6b-107">From PowerShell prompt the Teams Admin can run **set-csuser user@contoso.com -HostedVoiceMail $true** where the sip uri is of the user in question.</span></span>

> [!NOTE]
> <span data-ttu-id="f3c6b-108">Perubahan pada kebijakan dapat memakan waktu hingga 24 jam untuk meniru.</span><span class="sxs-lookup"><span data-stu-id="f3c6b-108">Changes to policies can take up to 24 hours to replicate.</span></span>