---
title: Pengaturan kebijakan rapat
ms.author: pebaum
author: pebaum
manager: scotv
ms.audience: Admin
ms.topic: article
ms.service: o365-administration
ROBOTS: NOINDEX, NOFOLLOW
localization_priority: Normal
ms.collection: Adm_O365
ms.custom:
- "9000734"
- "2657"
ms.openlocfilehash: 39151d3a56cc09a8ae2dd77fb7bf1e99066cc77a
ms.sourcegitcommit: 8bc60ec34bc1e40685e3976576e04a2623f63a7c
ms.translationtype: MT
ms.contentlocale: id-ID
ms.lasthandoff: 04/15/2021
ms.locfileid: "51825446"
---
# <a name="manage-meeting-policies-in-microsoft-teams"></a><span data-ttu-id="ecdbc-102">Mengelola kebijakan rapat di Microsoft Teams</span><span class="sxs-lookup"><span data-stu-id="ecdbc-102">Manage meeting policies in Microsoft Teams</span></span>

<span data-ttu-id="ecdbc-103">**Catatan: Perubahan kebijakan dapat memakan waktu hingga 24 jam agar dapat diterapkan bagi pengguna.**</span><span class="sxs-lookup"><span data-stu-id="ecdbc-103">**Note: It can take up to 24 hours for policy changes to take effect for users.**</span></span> <span data-ttu-id="ecdbc-104">Anda mungkin tidak bisa membuat perubahan ke kebijakan yang baru dibuat dengan segera; tunggu 4 jam dan coba mengubah kebijakan yang baru dibuat lagi.</span><span class="sxs-lookup"><span data-stu-id="ecdbc-104">You might not be able to make changes to newly created policies immediately; wait 4 hours and attempt to modify a newly created policy again.</span></span>

<span data-ttu-id="ecdbc-105">Kebijakan rapat digunakan untuk mengontrol fitur yang tersedia bagi peserta rapat untuk rapat yang dijadwalkan oleh pengguna di organisasi Anda.</span><span class="sxs-lookup"><span data-stu-id="ecdbc-105">Meeting policies are used to control the features that are available to meeting participants for meetings that are scheduled by users in your organization.</span></span> <span data-ttu-id="ecdbc-106">Beberapa fitur kebijakan rapat mungkin belum diterapkan di pusat admin Teams (fitur ini diberi label "segera hadir" dalam dokumentasi).</span><span class="sxs-lookup"><span data-stu-id="ecdbc-106">Some features of meeting policies might not be implemented in the Teams admin center yet (these are labeled "coming soon" in the documentation).</span></span> <span data-ttu-id="ecdbc-107">Dalam hal ini, atau jika mendapatkan kesalahan seperti "Kami tidak dapat memperbarui kebijakan saat ini, tetapi coba lagi nanti" di pusat admin Microsoft Teams, sebaiknya gunakan PowerShell untuk membuat atau mengubah kebijakan rapat Teams.</span><span class="sxs-lookup"><span data-stu-id="ecdbc-107">In this case, or if you are getting an error like "We can't update the policy right now but try it again later" in the Microsoft Teams admin center, we recommend that you use PowerShell to create or modify Teams meeting policies.</span></span> 

<span data-ttu-id="ecdbc-108">Untuk informasi selengkapnya tentang kebijakan rapat, lihat sumber daya berikut ini:</span><span class="sxs-lookup"><span data-stu-id="ecdbc-108">For more information about meeting policies, see the following resources:</span></span>

- <span data-ttu-id="ecdbc-109">Untuk mempelajari tentang membuat kebijakan, membuat perubahan, dan menetapkan pengguna ke kebijakan, lihat [Mengelola kebijakan rapat di Teams](https://docs.microsoft.com/microsoftteams/meeting-policies-in-teams).</span><span class="sxs-lookup"><span data-stu-id="ecdbc-109">To learn about creating policies, making changes, and assigning users to the policy, see [Manage meeting policies in Teams](https://docs.microsoft.com/microsoftteams/meeting-policies-in-teams).</span></span>

- <span data-ttu-id="ecdbc-110">Untuk membuat perubahan kebijakan menggunakan cmdlet PowerShell, lihat [Gambaran Umum PowerShell Teams.](https://docs.microsoft.com/microsoftteams/teams-powershell-overview)</span><span class="sxs-lookup"><span data-stu-id="ecdbc-110">To make policy changes using PowerShell cmdlets, see [Teams PowerShell Overview](https://docs.microsoft.com/microsoftteams/teams-powershell-overview).</span></span> 
    - <span data-ttu-id="ecdbc-111">Anda perlu menggunakan modul [PowerShell Skype for Business untuk](https://docs.microsoft.com/skypeforbusiness/set-up-your-computer-for-windows-powershell/download-and-install-the-skype-for-business-online-connector) kebijakan rapat Teams.</span><span class="sxs-lookup"><span data-stu-id="ecdbc-111">You need to use the [Skype for Business PowerShell module](https://docs.microsoft.com/skypeforbusiness/set-up-your-computer-for-windows-powershell/download-and-install-the-skype-for-business-online-connector) for Teams meeting policies.</span></span> 
    - <span data-ttu-id="ecdbc-112">Tinjau [dokumentasi cmdlet \*-CsTeamsMeetingPolicy](https://docs.microsoft.com/search/?search=CsTeamsMeetingPolicy&view=skype-ps) untuk informasi selengkapnya.</span><span class="sxs-lookup"><span data-stu-id="ecdbc-112">Review the [\*-CsTeamsMeetingPolicy cmdlets documentation](https://docs.microsoft.com/search/?search=CsTeamsMeetingPolicy&view=skype-ps) for more information.</span></span>

