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
# <a name="enable-teams-webinars"></a><span data-ttu-id="8b3e4-102">Mengaktifkan Teams Webinar Baru</span><span class="sxs-lookup"><span data-stu-id="8b3e4-102">Enable Teams Webinars</span></span>

<span data-ttu-id="8b3e4-103">Webinar diaktifkan secara default.</span><span class="sxs-lookup"><span data-stu-id="8b3e4-103">Webinars are enabled by default.</span></span> <span data-ttu-id="8b3e4-104">Anda bisa mengelola siapa yang bisa menjadwalkan dan mendaftar Teams Webinar dengan menggunakan Teams PowerShell.</span><span class="sxs-lookup"><span data-stu-id="8b3e4-104">You can manage who can schedule and register for Teams Webinars by using Teams PowerShell commands.</span></span>

- <span data-ttu-id="8b3e4-105">Semua pengguna yang bisa membuat rapat juga bisa membuat rapat webinar.</span><span class="sxs-lookup"><span data-stu-id="8b3e4-105">All users who can create a meeting can also create a webinar meeting.</span></span> <span data-ttu-id="8b3e4-106">Jika Anda ingin mengelola siapa yang bisa menjadwalkan Teams Webinar, gunakan *AllowMeetingRegistration.*</span><span class="sxs-lookup"><span data-stu-id="8b3e4-106">If you want to manage who can schedule Teams Webinars, use *AllowMeetingRegistration*.</span></span> 
- <span data-ttu-id="8b3e4-107">Secara default, *WhoCanRegister* diaktifkan dan diatur ke **Semua Orang.**</span><span class="sxs-lookup"><span data-stu-id="8b3e4-107">By default, *WhoCanRegister* is enabled and set to **Everyone**.</span></span> <span data-ttu-id="8b3e4-108">Jika Anda ingin menonaktifkan pendaftaran rapat, atur *AllowMeetingRegistration* ke **False.**</span><span class="sxs-lookup"><span data-stu-id="8b3e4-108">If you want to turn off meeting registration, set *AllowMeetingRegistration* to **False**.</span></span>

<span data-ttu-id="8b3e4-109">Untuk mengubah pengaturan ini, Anda harus menginstal [Teams PowerShell](/microsoftteams/teams-powershell-install).</span><span class="sxs-lookup"><span data-stu-id="8b3e4-109">To change these settings, you must install [Teams PowerShell](/microsoftteams/teams-powershell-install).</span></span> <span data-ttu-id="8b3e4-110">Juga, Kebijakan Rapat diberlakukan di Teams Webinar.</span><span class="sxs-lookup"><span data-stu-id="8b3e4-110">Also, Meeting Policies are enforced on Teams Webinars.</span></span> <span data-ttu-id="8b3e4-111">Misalnya, jika ikut anonim dinonaktifkan di pengaturan rapat, pengguna anonim tidak bisa bergabung dalam webinar.</span><span class="sxs-lookup"><span data-stu-id="8b3e4-111">For example, if anonymous join is turned off in meeting settings, anonymous users can't join webinars.</span></span>

<span data-ttu-id="8b3e4-112">Untuk mempelajari selengkapnya tentang mengonfigurasi siapa yang bisa mendaftar untuk webinar, lihat [Mengonfigurasi siapa yang bisa mendaftar untuk webinar.](/microsoftteams/set-up-webinars?source=docs#configure-who-can-register-for-webinars)</span><span class="sxs-lookup"><span data-stu-id="8b3e4-112">To learn more about configuring who can register for webinars, see [Configure who can register for webinars](/microsoftteams/set-up-webinars?source=docs#configure-who-can-register-for-webinars).</span></span> <span data-ttu-id="8b3e4-113">Untuk informasi selengkapnya tentang pengaturan untuk Microsoft Lists, lihat [Pengaturan kontrol untuk Daftar Microsoft.](/sharepoint/control-lists)</span><span class="sxs-lookup"><span data-stu-id="8b3e4-113">For more information about settings for Microsoft Lists, see [Control settings for Microsoft Lists](/sharepoint/control-lists).</span></span>