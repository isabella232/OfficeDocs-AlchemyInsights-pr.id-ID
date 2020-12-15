---
title: Alat diagnostik layanan untuk Desktop Virtual Windows
ms.author: v-aiyengar
author: AshaIyengar21
manager: dansimp
ms.date: 12/14/2020
ms.audience: Admin
ms.topic: article
ms.service: o365-administration
ROBOTS: NOINDEX, NOFOLLOW
localization_priority: Normal
ms.collection: Adm_O365
ms.custom:
- "9003893"
- "6947"
ms.openlocfilehash: c2e6f7fbcddc6721425840e87202a165cdb22664
ms.sourcegitcommit: 87bf574162e536003164ff9af50005c5a7dce601
ms.translationtype: MT
ms.contentlocale: id-ID
ms.lasthandoff: 12/14/2020
ms.locfileid: "49678623"
---
# <a name="service-diagnostics-tool-for-windows-virtual-desktop"></a><span data-ttu-id="0fbc7-102">Alat diagnostik layanan untuk Desktop Virtual Windows</span><span class="sxs-lookup"><span data-stu-id="0fbc7-102">Service diagnostics tool for Windows Virtual Desktop</span></span>

<span data-ttu-id="0fbc7-103">Windows Virtual desktop (WVD) menawarkan alat diagnostik yang memungkinkan admin mengidentifikasi kesalahan melalui satu antarmuka.</span><span class="sxs-lookup"><span data-stu-id="0fbc7-103">Windows Virtual Desktop (WVD) offers a diagnostic tool that lets admins identify errors through a single interface.</span></span> <span data-ttu-id="0fbc7-104">Alat ini mencatat informasi terkait diagnostik setiap kali WVD digunakan oleh seseorang yang ditugaskan sebagai peran WVD.</span><span class="sxs-lookup"><span data-stu-id="0fbc7-104">This tool logs diagnostics-related info whenever WVD is used by someone assigned a WVD role.</span></span> <span data-ttu-id="0fbc7-105">Setiap log berisi info tentang peran WVD yang terlibat dalam aktivitas, pesan kesalahan yang muncul selama sesi, dan informasi tentang penyewa dan pengguna.</span><span class="sxs-lookup"><span data-stu-id="0fbc7-105">Each log contains info about the WVD role involved in the activity, the error messages that appear during the session, and the info about the tenant and user.</span></span> <span data-ttu-id="0fbc7-106">Analitik log Azure bisa dikonfigurasikan untuk merekam log aktivitas yang dibuat oleh alat diagnostik.</span><span class="sxs-lookup"><span data-stu-id="0fbc7-106">Azure Log Analytics can be configured to capture the activity log created by the diagnostic tool.</span></span> <span data-ttu-id="0fbc7-107">Berikut caranya:</span><span class="sxs-lookup"><span data-stu-id="0fbc7-107">Here's how:</span></span>

1. <span data-ttu-id="0fbc7-108">Membuat ruang kerja analitik log dengan [Azure portal](https://go.microsoft.com/fwlink/?linkid=2129500) atau [Azure PowerShell](https://go.microsoft.com/fwlink/?linkid=2129501).</span><span class="sxs-lookup"><span data-stu-id="0fbc7-108">Create a Log Analytics workspace with the [Azure portal](https://go.microsoft.com/fwlink/?linkid=2129500) or [Azure PowerShell](https://go.microsoft.com/fwlink/?linkid=2129501).</span></span>
1. <span data-ttu-id="0fbc7-109">[Sambungkan komputer Windows ke Azure monitor](https://go.microsoft.com/fwlink/?linkid=2129913).</span><span class="sxs-lookup"><span data-stu-id="0fbc7-109">[Connect Windows computers to Azure Monitor](https://go.microsoft.com/fwlink/?linkid=2129913).</span></span> <span data-ttu-id="0fbc7-110">Dapatkan ID ruang kerja dan kunci utama ruang kerja Anda.</span><span class="sxs-lookup"><span data-stu-id="0fbc7-110">Get the Workspace ID and the Primary Key of your workspace.</span></span> <span data-ttu-id="0fbc7-111">Panduan penyetelan memerlukan info ini untuk mengonfigurasi agen dengan benar dan memastikan bahwa alat tersebut dapat berkomunikasi dengan Azure monitor.</span><span class="sxs-lookup"><span data-stu-id="0fbc7-111">The setup wizard needs this info to properly configure the agent and to ensure it can communicate with Azure Monitor.</span></span>
1. <span data-ttu-id="0fbc7-112">[Dorong diagnostik data ke ruang kerja Anda](https://go.microsoft.com/fwlink/?linkid=2128284).</span><span class="sxs-lookup"><span data-stu-id="0fbc7-112">[Push diagnostics data to your workspace](https://go.microsoft.com/fwlink/?linkid=2128284).</span></span> <span data-ttu-id="0fbc7-113">Anda dapat mendorong diagnostik data dari penyewa WVD ke log analitik untuk ruang kerja Anda.</span><span class="sxs-lookup"><span data-stu-id="0fbc7-113">You can push diagnostics data from your WVD tenant to the Log Analytics for your workspace.</span></span>
1. <span data-ttu-id="0fbc7-114">[Mengidentifikasi dan mendiagnosis masalah](https://go.microsoft.com/fwlink/?linkid=2128338) yang bersifat internal atau eksternal dalam kaitannya dengan wvd.</span><span class="sxs-lookup"><span data-stu-id="0fbc7-114">[Identify and diagnose issues](https://go.microsoft.com/fwlink/?linkid=2128338) that are internal or external in relation to WVD.</span></span>

<span data-ttu-id="0fbc7-115">Untuk mempelajari selengkapnya tentang mengonfigurasi alat diagnostik layanan untuk WVD, lihat [menggunakan log analitik untuk fitur diagnostik](https://go.microsoft.com/fwlink/?linkid=2128084).</span><span class="sxs-lookup"><span data-stu-id="0fbc7-115">To learn more about configuring the service diagnostics tool for WVD, see [Use Log Analytics for the diagnostics feature](https://go.microsoft.com/fwlink/?linkid=2128084).</span></span>
