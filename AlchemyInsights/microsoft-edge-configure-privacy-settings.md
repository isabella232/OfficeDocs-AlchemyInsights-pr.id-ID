---
title: Mengonfigurasi pengaturan privasi Microsoft Edge
ms.author: v-smandalika
author: v-smandalika
manager: dansimp
ms.date: 12/03/2020
ms.audience: Admin
ms.topic: article
ms.service: o365-administration
ROBOTS: NOINDEX, NOFOLLOW
localization_priority: Normal
ms.collection: Adm_O365
ms.custom:
- "9003843"
- "6892"
ms.openlocfilehash: dcd1d91dcde1f585caf0e1e3af30946513a0f26c
ms.sourcegitcommit: 94036315916fbc79dca2a692c2e9bc1139dd28f6
ms.translationtype: MT
ms.contentlocale: id-ID
ms.lasthandoff: 12/08/2020
ms.locfileid: "49677794"
---
# <a name="microsoft-edge-configure-privacy-settings"></a><span data-ttu-id="44afb-102">Mengonfigurasi pengaturan privasi Microsoft Edge</span><span class="sxs-lookup"><span data-stu-id="44afb-102">Microsoft Edge configure privacy settings</span></span>

<span data-ttu-id="44afb-103">Secara default, jika Microsoft Edge disebarkan di platform non-Windows, data diagnostik dan informasi situs tidak dikirim ke Microsoft.</span><span class="sxs-lookup"><span data-stu-id="44afb-103">By default, if Microsoft Edge is deployed on non-Windows platforms, diagnostic data and site information are not sent to Microsoft.</span></span> <span data-ttu-id="44afb-104">Namun, jika Microsoft Edge disebarkan di Windows 10, data diagnostik dan informasi situs dikirim sesuai dengan [pengaturan data diagnostik Windows](https://docs.microsoft.com/windows/privacy/configure-windows-diagnostic-data-in-your-organization)pengguna.</span><span class="sxs-lookup"><span data-stu-id="44afb-104">However, if Microsoft Edge is deployed on Windows 10, diagnostic data and site information are sent according to users' [Windows Diagnostic data settings](https://docs.microsoft.com/windows/privacy/configure-windows-diagnostic-data-in-your-organization).</span></span>

<span data-ttu-id="44afb-105">Untuk mengonfigurasi cara Microsoft Edge menangani kumpulan data untuk organisasi Anda, gunakan kebijakan grup berikut ini:</span><span class="sxs-lookup"><span data-stu-id="44afb-105">To configure how Microsoft Edge handles data collection for your organization, use the following group policies:</span></span>
- <span data-ttu-id="44afb-106">[Metricsreportingenabled](https://docs.microsoft.com/DeployEdge/microsoft-edge-policies#metricsreportingenabled): kebijakan ini memungkinkan pelaporan data terkait penggunaan dan crash.</span><span class="sxs-lookup"><span data-stu-id="44afb-106">[MetricsReportingEnabled](https://docs.microsoft.com/DeployEdge/microsoft-edge-policies#metricsreportingenabled): This policy enables reporting of usage and crash-related data.</span></span>
- <span data-ttu-id="44afb-107">[Sendsiteinfotoimproveservices](https://docs.microsoft.com/DeployEdge/microsoft-edge-policies#sendsiteinfotoimproveservices): kebijakan ini mengirimkan informasi situs yang digunakan untuk menyempurnakan layanan Microsoft.</span><span class="sxs-lookup"><span data-stu-id="44afb-107">[SendSiteInfoToImproveServices](https://docs.microsoft.com/DeployEdge/microsoft-edge-policies#sendsiteinfotoimproveservices): This policy sends site information that is used to improve Microsoft services.</span></span>

<span data-ttu-id="44afb-108">Untuk mempelajari selengkapnya, lihat [mengonfigurasi pengaturan kebijakan](https://docs.microsoft.com/deployedge/microsoft-edge-enterprise-privacy-settings#configure-policy-settings).</span><span class="sxs-lookup"><span data-stu-id="44afb-108">To learn more, see [Configure policy settings](https://docs.microsoft.com/deployedge/microsoft-edge-enterprise-privacy-settings#configure-policy-settings).</span></span>