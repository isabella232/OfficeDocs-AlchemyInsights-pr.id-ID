---
title: Pengaturan kebijakan Rapat
ms.author: pebaum
author: pebaum
manager: mnirkhe
ms.audience: Admin
ms.topic: article
ms.service: o365-administration
ROBOTS: NOINDEX, NOFOLLOW
localization_priority: Normal
ms.collection: Adm_O365
ms.custom:
- "9000734"
- "2657"
ms.openlocfilehash: 24a55417df0f89063fbdd9ade6d104be4f8ab49c
ms.sourcegitcommit: 0eb4f9bde53395b5fd4b5cd4ffc56ca96db91298
ms.translationtype: MT
ms.contentlocale: id-ID
ms.lasthandoff: 03/10/2021
ms.locfileid: "50704609"
---
# <a name="manage-meeting-policies-in-microsoft-teams"></a><span data-ttu-id="bd061-102">Mengelola Kebijakan Rapat di Microsoft teams</span><span class="sxs-lookup"><span data-stu-id="bd061-102">Manage meeting policies in Microsoft Teams</span></span>

<span data-ttu-id="bd061-103">**Catatan: perlu waktu hingga 24 jam agar perubahan kebijakan diterapkan untuk pengguna.**</span><span class="sxs-lookup"><span data-stu-id="bd061-103">**Note: It can take up to 24 hours for policy changes to take effect for users.**</span></span> <span data-ttu-id="bd061-104">Anda mungkin tidak dapat membuat perubahan pada kebijakan yang baru dibuat segera; Tunggu 4 jam dan coba Ubah kembali kebijakan yang baru dibuat.</span><span class="sxs-lookup"><span data-stu-id="bd061-104">You might not be able to make changes to newly created policies immediately; wait 4 hours and attempt to modify a newly created policy again.</span></span>

<span data-ttu-id="bd061-105">Kebijakan Rapat digunakan untuk mengontrol fitur yang tersedia bagi peserta rapat untuk Rapat yang dijadwalkan oleh pengguna di organisasi Anda.</span><span class="sxs-lookup"><span data-stu-id="bd061-105">Meeting policies are used to control the features that are available to meeting participants for meetings that are scheduled by users in your organization.</span></span> <span data-ttu-id="bd061-106">Beberapa fitur kebijakan Rapat mungkin tidak diterapkan di pusat admin teams (yang disebut "segera hadir" di dokumentasi).</span><span class="sxs-lookup"><span data-stu-id="bd061-106">Some features of meeting policies might not be implemented in the Teams admin center yet (these are labeled "coming soon" in the documentation).</span></span> <span data-ttu-id="bd061-107">Dalam kasus ini, atau jika Anda mendapatkan kesalahan seperti "kami tidak dapat memperbarui kebijakan sekarang tapi mencobanya lagi nanti" di pusat admin Microsoft teams, kami menyarankan agar Anda menggunakan PowerShell untuk membuat atau mengubah kebijakan Rapat teams.</span><span class="sxs-lookup"><span data-stu-id="bd061-107">In this case, or if you are getting an error like "We can't update the policy right now but try it again later" in the Microsoft Teams admin center, we recommend that you use PowerShell to create or modify Teams meeting policies.</span></span> 

<span data-ttu-id="bd061-108">Untuk informasi selengkapnya tentang kebijakan Rapat, lihat sumber daya berikut ini:</span><span class="sxs-lookup"><span data-stu-id="bd061-108">For more information about meeting policies, see the following resources:</span></span>

- <span data-ttu-id="bd061-109">Untuk mempelajari tentang membuat kebijakan, membuat perubahan, dan menetapkan pengguna ke kebijakan, lihat [mengelola kebijakan Rapat di teams](https://docs.microsoft.com/microsoftteams/meeting-policies-in-teams).</span><span class="sxs-lookup"><span data-stu-id="bd061-109">To learn about creating policies, making changes, and assigning users to the policy, see [Manage meeting policies in Teams](https://docs.microsoft.com/microsoftteams/meeting-policies-in-teams).</span></span>

- <span data-ttu-id="bd061-110">Untuk membuat perubahan kebijakan menggunakan cmdlet PowerShell, lihat [gambaran umum PowerShell teams](https://docs.microsoft.com/microsoftteams/teams-powershell-overview).</span><span class="sxs-lookup"><span data-stu-id="bd061-110">To make policy changes using PowerShell cmdlets, see [Teams PowerShell Overview](https://docs.microsoft.com/microsoftteams/teams-powershell-overview).</span></span> 
    - <span data-ttu-id="bd061-111">Anda perlu menggunakan [modul PowerShell untuk Rapat Skype for Business](https://docs.microsoft.com/skypeforbusiness/set-up-your-computer-for-windows-powershell/download-and-install-the-skype-for-business-online-connector) .</span><span class="sxs-lookup"><span data-stu-id="bd061-111">You need to use the [Skype for Business PowerShell module](https://docs.microsoft.com/skypeforbusiness/set-up-your-computer-for-windows-powershell/download-and-install-the-skype-for-business-online-connector) for Teams meeting policies.</span></span> 
    - <span data-ttu-id="bd061-112">Tinjau [dokumentasi cmdlet \*-csteamsmeetingpolicy](https://docs.microsoft.com/search/?search=CsTeamsMeetingPolicy&view=skype-ps) untuk informasi selengkapnya.</span><span class="sxs-lookup"><span data-stu-id="bd061-112">Review the [\*-CsTeamsMeetingPolicy cmdlets documentation](https://docs.microsoft.com/search/?search=CsTeamsMeetingPolicy&view=skype-ps) for more information.</span></span>

