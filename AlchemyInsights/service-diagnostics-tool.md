---
title: Alat diagnostik layanan untuk Windows Virtual Desktop
ms.author: pebaum
author: pebaum
manager: scotv
ms.date: 04/5/2021
ms.audience: Admin
ms.topic: article
ms.service: o365-administration
ROBOTS: NOINDEX, NOFOLLOW
localization_priority: Priority
ms.collection: Adm_O365
ms.custom:
- "9004219"
- "10873"
ms.openlocfilehash: dfa59c86508c8658c880f4f3f21a002524e909d1
ms.sourcegitcommit: 254b25150fa326628084d08479b0e7dd8b7d479a
ms.translationtype: MT
ms.contentlocale: id-ID
ms.lasthandoff: 04/05/2021
ms.locfileid: "51595868"
---
# <a name="service-diagnostics-tool-for-windows-virtual-desktop"></a><span data-ttu-id="0998d-102">Alat diagnostik layanan untuk Windows Virtual Desktop</span><span class="sxs-lookup"><span data-stu-id="0998d-102">Service diagnostics tool for Windows Virtual Desktop</span></span>

<span data-ttu-id="0998d-103">Windows Virtual Desktop (WVD) menawarkan alat diagnostik yang memungkinkan admin mengidentifikasi kesalahan melalui satu antarmuka.</span><span class="sxs-lookup"><span data-stu-id="0998d-103">Windows Virtual Desktop (WVD) offers a diagnostic tool that lets admins identify errors through a single interface.</span></span> <span data-ttu-id="0998d-104">Alat ini mencatat info terkait diagnostik setiap kali WVD digunakan oleh seseorang yang ditetapkan peran WVD.</span><span class="sxs-lookup"><span data-stu-id="0998d-104">This tool logs diagnostics-related info whenever WVD is used by someone assigned a WVD role.</span></span> <span data-ttu-id="0998d-105">Setiap log berisi informasi tentang peran WVD yang dilibatkan dalam aktivitas, pesan kesalahan yang muncul selama sesi, dan informasi tentang penyewa dan pengguna.</span><span class="sxs-lookup"><span data-stu-id="0998d-105">Each log contains info about the WVD role involved in the activity, the error messages that appear during the session, and the info about the tenant and user.</span></span> <span data-ttu-id="0998d-106">Analitik Log Azure dapat dikonfigurasi untuk merekam log aktivitas yang dibuat oleh alat diagnostik dengan mengikuti langkah-langkah berikut:</span><span class="sxs-lookup"><span data-stu-id="0998d-106">Azure Log Analytics can be configured to capture the activity log created by the diagnostic tool by following these steps:</span></span>

1. <span data-ttu-id="0998d-107">Buat ruang kerja Analitik Log dengan [portal Azure](https://go.microsoft.com/fwlink/?linkid=2129500) atau [Azure PowerShell](https://go.microsoft.com/fwlink/?linkid=2129501).</span><span class="sxs-lookup"><span data-stu-id="0998d-107">Create a Log Analytics workspace with the [Azure portal](https://go.microsoft.com/fwlink/?linkid=2129500) or [Azure PowerShell](https://go.microsoft.com/fwlink/?linkid=2129501).</span></span>

1. <span data-ttu-id="0998d-108">[Sambungkan komputer Windows ke Azure Monitor](https://go.microsoft.com/fwlink/?linkid=2129913).</span><span class="sxs-lookup"><span data-stu-id="0998d-108">[Connect Windows computers to Azure Monitor](https://go.microsoft.com/fwlink/?linkid=2129913).</span></span> <span data-ttu-id="0998d-109">Dapatkan ID Ruang Kerja dan Kunci Utama ruang kerja Anda.</span><span class="sxs-lookup"><span data-stu-id="0998d-109">Get the Workspace ID and the Primary Key of your workspace.</span></span> <span data-ttu-id="0998d-110">Panduan penyiapan memerlukan informasi ini untuk mengonfigurasi agen dengan benar dan memastikannya dapat berkomunikasi dengan Azure Monitor.</span><span class="sxs-lookup"><span data-stu-id="0998d-110">The setup wizard needs this info to properly configure the agent and to ensure it can communicate with Azure Monitor.</span></span>

1. <span data-ttu-id="0998d-111">[Mendorong data diagnostik ke ruang kerja Anda.](https://go.microsoft.com/fwlink/?linkid=2128284)</span><span class="sxs-lookup"><span data-stu-id="0998d-111">[Push diagnostics data to your workspace](https://go.microsoft.com/fwlink/?linkid=2128284).</span></span> <span data-ttu-id="0998d-112">Anda bisa mendorong data diagnostik dari penyewa WVD Anda ke Analitik Log untuk ruang kerja Anda.</span><span class="sxs-lookup"><span data-stu-id="0998d-112">You can push diagnostics data from your WVD tenant to the Log Analytics for your workspace.</span></span>

1. <span data-ttu-id="0998d-113">[Identifikasi dan mendiagnosis](https://docs.microsoft.com/azure/virtual-desktop/diagnostics-role-service#diagnose-issues-with-powershell) masalah yang bersesalifikasi internal maupun eksternal sehubungan dengan WVD.</span><span class="sxs-lookup"><span data-stu-id="0998d-113">[Identify and diagnose](https://docs.microsoft.com/azure/virtual-desktop/diagnostics-role-service#diagnose-issues-with-powershell) issues that are internal or external in relation to WVD.</span></span>

<span data-ttu-id="0998d-114">Untuk mempelajari selengkapnya tentang mengonfigurasi alat diagnostik layanan untuk WVD, lihat Menggunakan Analitik Log untuk fitur diagnostik.</span><span class="sxs-lookup"><span data-stu-id="0998d-114">To learn more about configuring the service diagnostics tool for WVD, see Use Log Analytics for the diagnostics feature.</span></span>