---
title: Mengonfigurasi pengaturan privasi di Microsoft Edge
ms.author: v-aiyengar
author: AshaIyengar21
manager: dansimp
ms.date: 03/24/2021
ms.audience: Admin
ms.topic: article
ms.service: o365-administration
ROBOTS: NOINDEX, NOFOLLOW
localization_priority: Normal
ms.collection: Adm_O365
ms.custom:
- "9004632"
- "8367"
ms.openlocfilehash: 2367a7a55d1837fa7c7095fd0ac10ff1cf7ae72d
ms.sourcegitcommit: db908b3da2c7a6508a77bf4f2c80afb294fadbd1
ms.translationtype: MT
ms.contentlocale: id-ID
ms.lasthandoff: 03/29/2021
ms.locfileid: "51405105"
---
# <a name="configure-privacy-settings-in-microsoft-edge"></a><span data-ttu-id="ebcd9-102">Mengonfigurasi pengaturan privasi di Microsoft Edge</span><span class="sxs-lookup"><span data-stu-id="ebcd9-102">Configure privacy settings in Microsoft Edge</span></span>

<span data-ttu-id="ebcd9-103">Secara default, jika Microsoft Edge digunakan di platform non-Windows, data diagnostik dan informasi situs tidak akan dikirim ke Microsoft.</span><span class="sxs-lookup"><span data-stu-id="ebcd9-103">By default, if Microsoft Edge is deployed on non-Windows platforms, diagnostic data and site information aren't sent to Microsoft.</span></span> <span data-ttu-id="ebcd9-104">Namun, jika Microsoft Edge disebarkan di Windows 10, data diagnostik dan informasi situs akan dikirim sesuai dengan pengaturan [data Diagnostik Windows pengguna.](https://go.microsoft.com/fwlink/?linkid=2132472)</span><span class="sxs-lookup"><span data-stu-id="ebcd9-104">However, if Microsoft Edge is deployed on Windows 10, diagnostic data and site information are sent according to users' [Windows Diagnostic data settings](https://go.microsoft.com/fwlink/?linkid=2132472).</span></span>

<span data-ttu-id="ebcd9-105">Untuk mengonfigurasi cara Microsoft Edge menangani pengumpulan data untuk organisasi Anda, gunakan kebijakan grup berikut:</span><span class="sxs-lookup"><span data-stu-id="ebcd9-105">To configure how Microsoft Edge handles data collection for your organization, use the following group policies:</span></span>
- <span data-ttu-id="ebcd9-106">[MetricsReportingEnabled](https://go.microsoft.com/fwlink/?linkid=2132470) aktif pada pelaporan penggunaan dan data terkait crash.</span><span class="sxs-lookup"><span data-stu-id="ebcd9-106">[MetricsReportingEnabled](https://go.microsoft.com/fwlink/?linkid=2132470) turns on reporting of usage and crash-related data.</span></span>
- <span data-ttu-id="ebcd9-107">[SendSiteInfoToImproveServices](https://go.microsoft.com/fwlink/?linkid=2132470) mengirimkan informasi situs yang digunakan untuk meningkatkan layanan Microsoft.</span><span class="sxs-lookup"><span data-stu-id="ebcd9-107">[SendSiteInfoToImproveServices](https://go.microsoft.com/fwlink/?linkid=2132470) sends site information used to improve Microsoft services.</span></span>

<span data-ttu-id="ebcd9-108">Untuk mempelajari selengkapnya, lihat [Mengonfigurasi pengaturan kebijakan](https://go.microsoft.com/fwlink/?linkid=2132577).</span><span class="sxs-lookup"><span data-stu-id="ebcd9-108">To learn more, see [Configure policy settings](https://go.microsoft.com/fwlink/?linkid=2132577).</span></span>
