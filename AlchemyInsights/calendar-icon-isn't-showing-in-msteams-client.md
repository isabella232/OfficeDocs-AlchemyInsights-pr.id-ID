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
# <a name="calendar-icon-isnt-showing-in-microsoft-teams-client"></a><span data-ttu-id="0fd4b-102">Ikon kalender tidak ditampilkan di klien Microsoft teams</span><span class="sxs-lookup"><span data-stu-id="0fd4b-102">Calendar icon isn't showing in Microsoft Teams client</span></span>

<span data-ttu-id="0fd4b-103">Tab **kalender** di teams memerlukan akses ke kotak surat Exchange melalui layanan web Exchange.</span><span class="sxs-lookup"><span data-stu-id="0fd4b-103">The **Calendar** Tab in Teams requires access to an Exchange mailbox via Exchange Web Services.</span></span> <span data-ttu-id="0fd4b-104">Kotak surat Exchange bisa online, atau di tempat.</span><span class="sxs-lookup"><span data-stu-id="0fd4b-104">The Exchange mailbox can be Online, or On-Premises.</span></span> <span data-ttu-id="0fd4b-105">Untuk pengguna online yang tidak melihat tab **kalender** , pastikan mereka [dilisensikan untuk kotak surat Exchange Online dan kotak surat diaktifkan](https://docs.microsoft.com/exchange/recipients-in-exchange-online/create-user-mailboxes).</span><span class="sxs-lookup"><span data-stu-id="0fd4b-105">For Online users who do not see the **Calendar** Tab, make sure they [are licensed for an Exchange Online mailbox and the mailbox is enabled](https://docs.microsoft.com/exchange/recipients-in-exchange-online/create-user-mailboxes).</span></span> <span data-ttu-id="0fd4b-106">Jika pengguna Anda berada di tempat, Anda perlu mengonfirmasi bahwa konfigurasi hibrid Anda sehat.</span><span class="sxs-lookup"><span data-stu-id="0fd4b-106">If your users are homed On-Premises, you need to confirm that your Hybrid configuration is healthy.</span></span> <span data-ttu-id="0fd4b-107">Gunakan [Panduan Konfigurasi Hibrid](https://docs.microsoft.com/exchange/hybrid-deployment/hybrid-agent) untuk memecahkan masalah.</span><span class="sxs-lookup"><span data-stu-id="0fd4b-107">Use the [Hybrid Configuration Wizard](https://docs.microsoft.com/exchange/hybrid-deployment/hybrid-agent) to troubleshoot.</span></span> <span data-ttu-id="0fd4b-108">Perhatikan bahwa [Teams membutuhkan Exchange 2016 CU3 atau lebih tinggi](https://docs.microsoft.com/microsoftteams/exchange-teams-interact).</span><span class="sxs-lookup"><span data-stu-id="0fd4b-108">Note that [Teams requires Exchange 2016 CU3 or higher](https://docs.microsoft.com/microsoftteams/exchange-teams-interact).</span></span>

<span data-ttu-id="0fd4b-109">Untuk informasi selengkapnya dan langkah pemecahan masalah, lihat [memecahkan masalah interaksi Microsoft teams dan server Exchange](https://docs.microsoft.com/microsoftteams/troubleshoot/known-issues/teams-exchange-interaction-issue).</span><span class="sxs-lookup"><span data-stu-id="0fd4b-109">For more information and troubleshooting steps, see [Troubleshoot Microsoft Teams and Exchange Server interaction issues](https://docs.microsoft.com/microsoftteams/troubleshoot/known-issues/teams-exchange-interaction-issue).</span></span>
