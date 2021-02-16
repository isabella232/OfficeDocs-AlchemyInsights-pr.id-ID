---
title: Mengaktifkan perangkat
ms.author: v-jmathew
author: v-jmathew
manager: scotv
ms.audience: Admin
ms.topic: article
ms.service: o365-administration
ROBOTS: NOINDEX, NOFOLLOW
localization_priority: Normal
ms.collection: Adm_O365
ms.custom:
- "9003257"
- "8278"
ms.openlocfilehash: 9e4b03dcba7a2c98a5d63213ee49f9ba8f91d670
ms.sourcegitcommit: 0470a728d184ceb89d1419f7ed57166e07bb778b
ms.translationtype: MT
ms.contentlocale: id-ID
ms.lasthandoff: 02/15/2021
ms.locfileid: "50256871"
---
# <a name="enable-device"></a><span data-ttu-id="6374e-102">Mengaktifkan perangkat</span><span class="sxs-lookup"><span data-stu-id="6374e-102">Enable Device</span></span>

<span data-ttu-id="6374e-103">**Untuk mengaktifkan perangkat menggunakan perintah PowerShell**</span><span class="sxs-lookup"><span data-stu-id="6374e-103">**To enable the device using Powershell command**</span></span>

<span data-ttu-id="6374e-104">Jalankan perintah berikut:</span><span class="sxs-lookup"><span data-stu-id="6374e-104">Run the following commands:</span></span>

- <span data-ttu-id="6374e-105">Untuk mendapatkan objek perangkat: `Get-MsolDevice -Name <Name>`</span><span class="sxs-lookup"><span data-stu-id="6374e-105">To get device object: `Get-MsolDevice -Name <Name>`</span></span>
- <span data-ttu-id="6374e-106">Untuk mengaktifkan perangkat: `Enable-MsolDevice -DeviceId <DeviceId>`</span><span class="sxs-lookup"><span data-stu-id="6374e-106">To enable device: `Enable-MsolDevice -DeviceId <DeviceId>`</span></span>

<span data-ttu-id="6374e-107">Untuk informasi selengkapnya tentang mengonfigurasi gabungan hibrid pada domain terkelola, lihat [mengonfigurasi gabungan hibrid](https://docs.microsoft.com/azure/active-directory/devices/hybrid-azuread-join-managed-domains).</span><span class="sxs-lookup"><span data-stu-id="6374e-107">For more information on Configuring Hybrid Join on managed domains, see [Configure Hybrid Join](https://docs.microsoft.com/azure/active-directory/devices/hybrid-azuread-join-managed-domains).</span></span>
