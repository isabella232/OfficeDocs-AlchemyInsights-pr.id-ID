---
title: Rekaman panggilan 1:1
ms.author: v-smandalika
author: v-smandalika
manager: dansimp
ms.date: 12/18/2020
ms.audience: Admin
ms.topic: article
ms.service: o365-administration
ROBOTS: NOINDEX, NOFOLLOW
localization_priority: Normal
ms.collection: Adm_O365
ms.custom:
- "9002530"
- "7648"
ms.openlocfilehash: 18c68fee514681b2a81c3cfa022c29ce83834f22
ms.sourcegitcommit: 610a5d950cdf488870601762ef52d881e3e22a48
ms.translationtype: MT
ms.contentlocale: id-ID
ms.lasthandoff: 05/28/2021
ms.locfileid: "52696961"
---
# <a name="11-call-recording"></a><span data-ttu-id="69236-102">Rekaman panggilan 1:1</span><span class="sxs-lookup"><span data-stu-id="69236-102">1:1 call recording</span></span>

<span data-ttu-id="69236-103">Jika tombol **Mulai Perekaman** berwarna abu-abu dalam panggilan 1:1, Anda perlu mengubah pengaturan kebijakan untuk pengguna yang terkena dampak.</span><span class="sxs-lookup"><span data-stu-id="69236-103">If the **Start Recording** button is grayed out in a 1:1 call, you need to change the policy settings for the impacted user.</span></span>   

<span data-ttu-id="69236-104">Mulai 31 Mei 2021, kami akan mulai memberlakukan Kebijakan Teams *Baru AllowCloudRecordingForCalls*.</span><span class="sxs-lookup"><span data-stu-id="69236-104">Beginning May 31, 2021, we'll start enforcing a new Teams Calling Policy *AllowCloudRecordingForCalls*.</span></span> <span data-ttu-id="69236-105">Sebelum perubahan ini, rekaman panggilan 1:1 dikontrol oleh *AllowCloudRecording Teams* Meeting.</span><span class="sxs-lookup"><span data-stu-id="69236-105">Prior to this change, 1:1 call recording is controlled by the *AllowCloudRecording* Teams Meeting Policy.</span></span> <span data-ttu-id="69236-106">Perubahan ini didokumentasikan dalam postingan Pusat Pesan: [(Diperbarui) 1:1 Pengenalan kebijakan perekaman panggilan](https://portal.microsoft.com/Adminportal/Home?ref=MessageCenter/:/messages/MC238796).</span><span class="sxs-lookup"><span data-stu-id="69236-106">This change is documented in the Message Center post: [(Updated) 1:1 Call recording policy introduction](https://portal.microsoft.com/Adminportal/Home?ref=MessageCenter/:/messages/MC238796).</span></span>  

<span data-ttu-id="69236-107">*AllowCloudRecordingForCalls*   opsi kebijakan panggilan otomatis diatur **$False** secara default.</span><span class="sxs-lookup"><span data-stu-id="69236-107">*AllowCloudRecordingForCalls* calling policy option is set to **$False** by default.</span></span> <span data-ttu-id="69236-108">Jika Anda lebih suka memblokir semua pengguna merekam panggilan 1:1, Anda tidak perlu melakukan tindakan apa pun.</span><span class="sxs-lookup"><span data-stu-id="69236-108">If you prefer to block all users from recording 1:1 calls, you don't need to take any action.</span></span>  

<span data-ttu-id="69236-109">Untuk mengaktifkan perekaman panggilan bagi semua pengguna dalam panggilan 1:1, gunakan Teams PowerShell untuk menjalankan cmdlet berikut:</span><span class="sxs-lookup"><span data-stu-id="69236-109">To enable call recording for all users in 1:1 calls use Teams PowerShell to run the following cmdlet:</span></span> 

<span data-ttu-id="69236-110">**Set-CsTeamsCallingPolicy -Identity Global -AllowCloudRecordingForCalls $True**</span><span class="sxs-lookup"><span data-stu-id="69236-110">**Set-CsTeamsCallingPolicy -Identity Global -AllowCloudRecordingForCalls $True**</span></span> 

<span data-ttu-id="69236-111">Alternatifnya, Anda bisa membuat kebijakan baru dan mengatur **-AllowCloudRecordingForCalls** **$true** dan menetapkan kebijakan tersebut ke pengguna Anda.</span><span class="sxs-lookup"><span data-stu-id="69236-111">Alternatively, you can create a new policy and set **-AllowCloudRecordingForCalls** to **$true** and assign that policy to your users.</span></span> 

<span data-ttu-id="69236-112">Untuk informasi selengkapnya, lihat [Kontrol Kebijakan Perekaman Panggilan 1:1 Are (Hampir!) Di sini](https://techcommunity.microsoft.com/t5/microsoft-teams-support/1-1-call-recording-policy-controls-are-almost-here/ba-p/2217668).</span><span class="sxs-lookup"><span data-stu-id="69236-112">For more information, see [1:1 Call Recording Policy Controls Are (Almost!) Here](https://techcommunity.microsoft.com/t5/microsoft-teams-support/1-1-call-recording-policy-controls-are-almost-here/ba-p/2217668).</span></span>
