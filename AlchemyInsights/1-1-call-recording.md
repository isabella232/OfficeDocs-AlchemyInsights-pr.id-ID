---
title: perekaman panggilan 1:1
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
ms.openlocfilehash: af09e8805409446a42a62c82aa577ad27f09a17a
ms.sourcegitcommit: 6312ee31561db36104f32282d019d069ede69174
ms.translationtype: MT
ms.contentlocale: id-ID
ms.lasthandoff: 03/11/2021
ms.locfileid: "50733852"
---
# <a name="11-call-recording"></a><span data-ttu-id="d8c1c-102">perekaman panggilan 1:1</span><span class="sxs-lookup"><span data-stu-id="d8c1c-102">1:1 call recording</span></span>

<span data-ttu-id="d8c1c-103">Administrator perlu melakukan tindakan sekarang untuk terus memungkinkan pengguna merekam panggilan 1:1.</span><span class="sxs-lookup"><span data-stu-id="d8c1c-103">Administrators need to take action now to continue allowing users to Record 1:1 calls.</span></span>
 
<span data-ttu-id="d8c1c-104">Mulai 12 April 2021, kita akan mulai memberlakukan opsi kebijakan panggilan teams baru *Allowcloudrecordingforcalls*.</span><span class="sxs-lookup"><span data-stu-id="d8c1c-104">Beginning April 12, 2021, we will start enforcing a new Teams Calling Policy option *AllowCloudRecordingForCalls*.</span></span> 

<span data-ttu-id="d8c1c-105">Saat ini kemampuan perekaman panggilan 1:1 dikontrol oleh opsi *Allowcloudrecording* di kebijakan teams Rapat.</span><span class="sxs-lookup"><span data-stu-id="d8c1c-105">Currently 1:1 call recording capabilities are controlled by the *AllowCloudRecording* option in Teams Meeting Policies.</span></span> <span data-ttu-id="d8c1c-106">Jika pengguna Anda diperbolehkan untuk merekam Rapat teams, mereka juga bisa merekam panggilan 1:1.</span><span class="sxs-lookup"><span data-stu-id="d8c1c-106">If your users are allowed to record Teams Meetings they can also record 1:1 calls.</span></span>

<span data-ttu-id="d8c1c-107">Jika Anda lebih suka memblokir semua pengguna dari merekam panggilan 1:1, Anda tidak perlu melakukan tindakan apa pun.</span><span class="sxs-lookup"><span data-stu-id="d8c1c-107">If you prefer to block all users from recording 1:1 calls, you do not need to take any action.</span></span> <span data-ttu-id="d8c1c-108">Opsi kebijakan panggilan *Allowcloudrecordingforcalls* akan $false secara default.</span><span class="sxs-lookup"><span data-stu-id="d8c1c-108">*AllowCloudRecordingForCalls* calling policy option will be $False by default.</span></span>

<span data-ttu-id="d8c1c-109">Perubahan ini didokumentasikan dalam postingan pusat pesan berikut ini: [(Diperbarui) pengenalan kebijakan perekaman panggilan 1:1](https://portal.microsoft.com/Adminportal/Home?ref=MessageCenter/:/messages/MC238796) untuk mengatur opsi kebijakan panggilan teams Anda harus menggunakan [teams PowerShell](https://docs.microsoft.com/microsoftteams/teams-powershell-install).</span><span class="sxs-lookup"><span data-stu-id="d8c1c-109">This change is documented in the following Message Center Post: [(Updated) 1:1 Call recording policy introduction](https://portal.microsoft.com/Adminportal/Home?ref=MessageCenter/:/messages/MC238796) To set the Teams Calling Policy Option you must use [Teams PowerShell](https://docs.microsoft.com/microsoftteams/teams-powershell-install).</span></span>

<span data-ttu-id="d8c1c-110">**Untuk mengaktifkan perekaman panggilan di panggilan 1:1:** Set-CsTeamsCallingPolicy-identitas global-AllowCloudRecordingForCalls $True</span><span class="sxs-lookup"><span data-stu-id="d8c1c-110">**To enable call recording in 1:1 calls:** Set-CsTeamsCallingPolicy -Identity Global -AllowCloudRecordingForCalls $True</span></span>

<span data-ttu-id="d8c1c-111">**Untuk menonaktifkan perekaman panggilan di panggilan 1:1:** Set-CsTeamsCallingPolicy-identitas global-AllowCloudRecordingForCalls $false</span><span class="sxs-lookup"><span data-stu-id="d8c1c-111">**To disable call recording in 1:1 calls:** Set-CsTeamsCallingPolicy -Identity Global -AllowCloudRecordingForCalls $False</span></span>

