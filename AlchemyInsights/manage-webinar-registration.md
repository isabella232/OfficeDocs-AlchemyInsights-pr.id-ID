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
# <a name="manage-webinar-registration"></a><span data-ttu-id="6a498-102">Mengelola pendaftaran webinar</span><span class="sxs-lookup"><span data-stu-id="6a498-102">Manage webinar registration</span></span>

<span data-ttu-id="6a498-103">Anda mengelola siapa yang bisa mendaftar Teams Webinar gratis dengan Teams Perintah Powershell.</span><span class="sxs-lookup"><span data-stu-id="6a498-103">You manage who can register for Teams Webinars by using Teams Powershell commands.</span></span> <span data-ttu-id="6a498-104">Untuk menginstal Teams Powershell, lihat [Teams PowerShell](/microsoftteams/teams-powershell-install).</span><span class="sxs-lookup"><span data-stu-id="6a498-104">To install Teams Powershell, see [Teams PowerShell](/microsoftteams/teams-powershell-install).</span></span> 

<span data-ttu-id="6a498-105">Secara default, *WhoCanRegister* diaktifkan dan diatur ke **EveryoneInCompany**.</span><span class="sxs-lookup"><span data-stu-id="6a498-105">By default, *WhoCanRegister* is enabled and set to **EveryoneInCompany**.</span></span> <span data-ttu-id="6a498-106">Untuk memperbolehkan siapa saja, termasuk pengguna anonim, untuk mendaftar, Anda harus menyetel Kebijakan Rapat ke **Setiap** Orang dengan menggunakan perintah Powershell:</span><span class="sxs-lookup"><span data-stu-id="6a498-106">To allow anyone, including anonymous users, to register, you must set the Meeting Policy to **Everyone** by using the Powershell command:</span></span>

`Set-CsTeamsMeetingPolicy -WhoCanRegister Everyone`

<span data-ttu-id="6a498-107">**Catatan**: Jika bergabung anonim dinonaktifkan dalam pengaturan rapat, pengguna anonim tidak dapat bergabung dalam webinar.</span><span class="sxs-lookup"><span data-stu-id="6a498-107">**Note**: If anonymous join is turned off in meeting settings, anonymous users can't join webinars.</span></span> <span data-ttu-id="6a498-108">Untuk mempelajari selengkapnya dan mengaktifkan pengaturan ini, lihat [Mengelola pengaturan rapat di Microsoft Teams](/microsoftteams/meeting-settings-in-teams).</span><span class="sxs-lookup"><span data-stu-id="6a498-108">To learn more and enable this setting, see [Manage meeting settings in Microsoft Teams](/microsoftteams/meeting-settings-in-teams).</span></span>

<span data-ttu-id="6a498-109">Jika Anda ingin menonaktifkan pendaftaran rapat, atur *AllowMeetingRegistration* ke **False.**</span><span class="sxs-lookup"><span data-stu-id="6a498-109">If you want to turn off meeting registration, set *AllowMeetingRegistration* to **False**.</span></span>

<span data-ttu-id="6a498-110">Untuk mempelajari selengkapnya tentang mengonfigurasi siapa yang bisa mendaftar untuk webinar, lihat [Mengonfigurasi siapa yang bisa mendaftar untuk webinar.](/microsoftteams/set-up-webinars?source=docs#configure-who-can-register-for-webinars)</span><span class="sxs-lookup"><span data-stu-id="6a498-110">To learn more about configuring who can register for webinars, see [Configure who can register for webinars](/microsoftteams/set-up-webinars?source=docs#configure-who-can-register-for-webinars).</span></span> <span data-ttu-id="6a498-111">Untuk informasi selengkapnya tentang pengaturan untuk Microsoft Lists, lihat [Pengaturan kontrol untuk Daftar Microsoft.](/sharepoint/control-lists)</span><span class="sxs-lookup"><span data-stu-id="6a498-111">For more information about settings for Microsoft Lists, see [Control settings for Microsoft Lists](/sharepoint/control-lists).</span></span>
