---
title: Pengaturan kebijakan Rapat
ms.author: pebaum
author: pebaum
manager: mnirkhe
ms.audience: Admin
ms.topic: article
ROBOTS: NOINDEX, NOFOLLOW
localization_priority: Normal
ms.collection: Adm_O365
ms.custom:
- "9000734"
- "2657"
ms.openlocfilehash: 509bd0c686830c04ed27f97372411677c0a7f4a4
ms.sourcegitcommit: 9aaa61d717e0fd475d2e9f0507c42aa40d073b5f
ms.translationtype: MT
ms.contentlocale: id-ID
ms.lasthandoff: 02/15/2020
ms.locfileid: "42042847"
---
# <a name="manage-meeting-policies-in-microsoft-teams"></a><span data-ttu-id="44323-102">Mengelola Kebijakan Rapat di Microsoft teams</span><span class="sxs-lookup"><span data-stu-id="44323-102">Manage meeting policies in Microsoft Teams</span></span>

<span data-ttu-id="44323-103">**Catatan: diperlukan waktu hingga 24 jam agar perubahan kebijakan diterapkan bagi pengguna.**</span><span class="sxs-lookup"><span data-stu-id="44323-103">**Note: It can take up to 24 hours for policy changes to take effect for users.**</span></span> <span data-ttu-id="44323-104">Anda mungkin tidak dapat membuat perubahan pada kebijakan yang baru dibuat dengan segera; menunggu 4 jam dan mencoba untuk mengubah kebijakan baru dibuat lagi.</span><span class="sxs-lookup"><span data-stu-id="44323-104">You might not be able to make changes to newly created policies immediately; wait 4 hours and attempt to modify a newly created policy again.</span></span>

<span data-ttu-id="44323-105">Kebijakan Rapat digunakan untuk mengontrol fitur yang tersedia untuk Rapat peserta pertemuan yang dijadwalkan oleh pengguna di organisasi Anda.</span><span class="sxs-lookup"><span data-stu-id="44323-105">Meeting policies are used to control the features that are available to meeting participants for meetings that are scheduled by users in your organization.</span></span> <span data-ttu-id="44323-106">Beberapa fitur kebijakan Rapat mungkin tidak diimplementasikan di pusat admin teams (ini diberi label "segera hadir" dalam dokumentasi).</span><span class="sxs-lookup"><span data-stu-id="44323-106">Some features of meeting policies might not be implemented in the Teams admin center yet (these are labeled "coming soon" in the documentation).</span></span> <span data-ttu-id="44323-107">Dalam hal ini, atau jika Anda menerima pesan kesalahan seperti "kami tidak dapat memperbarui kebijakan sekarang, namun coba lagi nanti" di pusat admin Microsoft teams, sebaiknya gunakan PowerShell untuk membuat atau memodifikasi Kebijakan Rapat tim.</span><span class="sxs-lookup"><span data-stu-id="44323-107">In this case, or if you are getting an error like "We can't update the policy right now but try it again later" in the Microsoft Teams admin center, we recommend that you use PowerShell to create or modify Teams meeting policies.</span></span> 

<span data-ttu-id="44323-108">Untuk informasi selengkapnya tentang kebijakan Rapat, lihat sumber daya berikut ini:</span><span class="sxs-lookup"><span data-stu-id="44323-108">For more information about meeting policies, see the following resources:</span></span>

- <span data-ttu-id="44323-109">Untuk mempelajari tentang membuat kebijakan, membuat perubahan, dan menetapkan pengguna ke kebijakan, lihat [mengelola kebijakan Rapat di teams](https://docs.microsoft.com/microsoftteams/meeting-policies-in-teams).</span><span class="sxs-lookup"><span data-stu-id="44323-109">To learn about creating policies, making changes, and assigning users to the policy, see [Manage meeting policies in Teams](https://docs.microsoft.com/microsoftteams/meeting-policies-in-teams).</span></span>

- <span data-ttu-id="44323-110">Untuk membuat perubahan kebijakan menggunakan cmdlet PowerShell, lihat [ringkasan tim PowerShell](https://docs.microsoft.com/microsoftteams/teams-powershell-overview).</span><span class="sxs-lookup"><span data-stu-id="44323-110">To make policy changes using PowerShell cmdlets, see [Teams PowerShell Overview](https://docs.microsoft.com/microsoftteams/teams-powershell-overview).</span></span> 
    - <span data-ttu-id="44323-111">Anda harus menggunakan [modul Skype for Business PowerShell](https://www.microsoft.com/download/details.aspx?id=39366) untuk kebijakan Rapat tim.</span><span class="sxs-lookup"><span data-stu-id="44323-111">You need to use the [Skype for Business PowerShell module](https://www.microsoft.com/download/details.aspx?id=39366) for Teams meeting policies.</span></span> 
    - <span data-ttu-id="44323-112">Meninjau [\*-csteamsmeetingpolicy cmdlet dokumentasi](https://docs.microsoft.com/search/?search=CsTeamsMeetingPolicy&view=skype-ps) untuk informasi lebih lanjut.</span><span class="sxs-lookup"><span data-stu-id="44323-112">Review the [\*-CsTeamsMeetingPolicy cmdlets documentation](https://docs.microsoft.com/search/?search=CsTeamsMeetingPolicy&view=skype-ps) for more information.</span></span>

