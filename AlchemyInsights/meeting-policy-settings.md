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
- "2657"
- "9000734"
ms.openlocfilehash: dac06690b51459ca166c15a5ef0f4c7e7a6d36f0
ms.sourcegitcommit: 0495112ad4fd0e695140ec66d190e62f03030584
ms.translationtype: MT
ms.contentlocale: id-ID
ms.lasthandoff: 10/02/2019
ms.locfileid: "37376688"
---
# <a name="manage-meeting-policies-in-microsoft-teams"></a><span data-ttu-id="a3907-102">Mengelola Kebijakan Rapat di Microsoft teams</span><span class="sxs-lookup"><span data-stu-id="a3907-102">Manage meeting policies in Microsoft Teams</span></span>

<span data-ttu-id="a3907-103">Kebijakan Rapat digunakan untuk mengontrol fitur yang tersedia untuk Rapat peserta pertemuan yang dijadwalkan oleh pengguna di organisasi Anda.</span><span class="sxs-lookup"><span data-stu-id="a3907-103">Meeting policies are used to control the features that are available to meeting participants for meetings that are scheduled by users in your organization.</span></span> <span data-ttu-id="a3907-104">Beberapa fitur kebijakan Rapat mungkin tidak diimplementasikan di pusat admin teams (ini diberi label "segera hadir" dalam dokumentasi).</span><span class="sxs-lookup"><span data-stu-id="a3907-104">Some features of meeting policies might not be implemented in the Teams admin center yet (these are labeled "coming soon" in the documentation).</span></span> <span data-ttu-id="a3907-105">Dalam hal ini, atau jika Anda menerima pesan kesalahan seperti "kami tidak dapat memperbarui kebijakan sekarang, namun coba lagi nanti" di pusat admin Microsoft teams, sebaiknya gunakan PowerShell untuk membuat atau memodifikasi Kebijakan Rapat tim.</span><span class="sxs-lookup"><span data-stu-id="a3907-105">In this case, or if you are getting an error like "We can't update the policy right now but try it again later" in the Microsoft Teams admin center, we recommend that you use PowerShell to create or modify Teams meeting policies.</span></span> 

<span data-ttu-id="a3907-106">Untuk informasi selengkapnya tentang kebijakan Rapat, lihat sumber daya berikut ini:</span><span class="sxs-lookup"><span data-stu-id="a3907-106">For more information about meeting policies, see the following resources:</span></span>

- <span data-ttu-id="a3907-107">Untuk mempelajari tentang membuat kebijakan, membuat perubahan, dan menetapkan pengguna ke kebijakan, lihat [mengelola kebijakan Rapat di teams](https://docs.microsoft.com/en-us/microsoftteams/meeting-policies-in-teams).</span><span class="sxs-lookup"><span data-stu-id="a3907-107">To learn about creating policies, making changes, and assigning users to the policy, see [Manage meeting policies in Teams](https://docs.microsoft.com/en-us/microsoftteams/meeting-policies-in-teams).</span></span>

- <span data-ttu-id="a3907-108">Untuk membuat perubahan kebijakan menggunakan cmdlet PowerShell, lihat [ringkasan tim PowerShell](https://docs.microsoft.com/microsoftteams/teams-powershell-overview).</span><span class="sxs-lookup"><span data-stu-id="a3907-108">To make policy changes using PowerShell cmdlets, see [Teams PowerShell Overview](https://docs.microsoft.com/microsoftteams/teams-powershell-overview).</span></span> 
    - <span data-ttu-id="a3907-109">Anda harus menggunakan [modul Skype for Business PowerShell](https://www.microsoft.com/download/details.aspx?id=39366) untuk kebijakan Rapat tim.</span><span class="sxs-lookup"><span data-stu-id="a3907-109">You need to use the [Skype for Business PowerShell module](https://www.microsoft.com/download/details.aspx?id=39366) for Teams meeting policies.</span></span> 
    - <span data-ttu-id="a3907-110">Meninjau [\*-csteamsmeetingpolicy cmdlet dokumentasi](https://docs.microsoft.com/search/?search=CsTeamsMeetingPolicy&view=skype-ps) untuk informasi lebih lanjut.</span><span class="sxs-lookup"><span data-stu-id="a3907-110">Review the [\*-CsTeamsMeetingPolicy cmdlets documentation](https://docs.microsoft.com/search/?search=CsTeamsMeetingPolicy&view=skype-ps) for more information.</span></span>

<span data-ttu-id="a3907-111">**Catatan:** Diperlukan waktu hingga 24 jam agar perubahan kebijakan diterapkan bagi pengguna.</span><span class="sxs-lookup"><span data-stu-id="a3907-111">**Note:** It can take up to 24 hours for policy changes to take effect for users.</span></span> <span data-ttu-id="a3907-112">Anda mungkin tidak dapat membuat perubahan pada kebijakan yang baru dibuat dengan segera; menunggu 4 jam dan mencoba untuk mengubah kebijakan baru dibuat lagi.</span><span class="sxs-lookup"><span data-stu-id="a3907-112">You might not be able to make changes to newly created policies immediately; wait 4 hours and attempt to modify a newly created policy again.</span></span> <span data-ttu-id="a3907-113">Jika Anda masih mengalami masalah, coba PowerShell.</span><span class="sxs-lookup"><span data-stu-id="a3907-113">If you're still having problems, try PowerShell.</span></span>  