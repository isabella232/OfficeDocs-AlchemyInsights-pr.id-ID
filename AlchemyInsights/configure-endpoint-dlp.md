---
title: Mengkonfigurasi DLP titik akhir
ms.author: pebaum
author: pebaum
manager: scotv
ms.date: 08/03/2020
ms.audience: Admin
ms.topic: article
ROBOTS: NOINDEX, NOFOLLOW
localization_priority: Priority
ms.collection: Adm_O365
ms.custom:
- "6108"
- "3200001"
ms.openlocfilehash: 039c8f78c5896b66eab5763fb0bbddd3f0b06f2d
ms.sourcegitcommit: 1dada930649a2625eb6d15910b2bfd5e1e00e5b6
ms.translationtype: MT
ms.contentlocale: id-ID
ms.lasthandoff: 08/03/2020
ms.locfileid: "46555557"
---
# <a name="configure-endpoint-dlp"></a><span data-ttu-id="22d59-102">Mengkonfigurasi DLP titik akhir</span><span class="sxs-lookup"><span data-stu-id="22d59-102">Configure Endpoint DLP</span></span>

<span data-ttu-id="22d59-103">Microsoft Endpoint DLP memungkinkan Anda untuk memperpanjang proteksi DLP dan kemampuan pemantauan untuk informasi sensitif pada perangkat Windows 10.</span><span class="sxs-lookup"><span data-stu-id="22d59-103">Microsoft Endpoint DLP allows you to extend DLP protection and monitoring capability to sensitive information on Windows 10 devices.</span></span> <span data-ttu-id="22d59-104">Setelah perangkat onboarded ke manajemen perangkat, Anda dapat membuat kebijakan DLP untuk menegakkan tindakan perlindungan pada item.</span><span class="sxs-lookup"><span data-stu-id="22d59-104">After devices are onboarded into device management, you can create DLP policies to enforce protective actions on items.</span></span> <span data-ttu-id="22d59-105">Penjelajah aktivitas dapat digunakan untuk memantau aktivitas untuk item yang sensitif.</span><span class="sxs-lookup"><span data-stu-id="22d59-105">The Activity Explorer can be used to monitor activity for sensitive items.</span></span> <span data-ttu-id="22d59-106">Untuk info selengkapnya, lihat [perangkat orientasi dalam pengelolaan perangkat](https://docs.microsoft.com/microsoft-365/compliance/endpoint-dlp-getting-started#onboarding-devices-into-device-management).</span><span class="sxs-lookup"><span data-stu-id="22d59-106">For more info, see [Onboarding devices into device management](https://docs.microsoft.com/microsoft-365/compliance/endpoint-dlp-getting-started#onboarding-devices-into-device-management).</span></span>  

<span data-ttu-id="22d59-107">Untuk memulai dengan Endpoint DLP:</span><span class="sxs-lookup"><span data-stu-id="22d59-107">To get started with Endpoint DLP:</span></span>

- <span data-ttu-id="22d59-108">Pastikan Anda memiliki lisensi SKU/langganan yang sesuai.</span><span class="sxs-lookup"><span data-stu-id="22d59-108">Ensure you have the appropriate SKU/subscriptions licensing.</span></span> <span data-ttu-id="22d59-109">Untuk informasi lebih lanjut, lihat [SKU/langganan lisensi](https://docs.microsoft.com/microsoft-365/compliance/endpoint-dlp-getting-started#skusubscriptions-licensing).</span><span class="sxs-lookup"><span data-stu-id="22d59-109">For more info, see [SKU/subscriptions licensing](https://docs.microsoft.com/microsoft-365/compliance/endpoint-dlp-getting-started#skusubscriptions-licensing).</span></span>
- <span data-ttu-id="22d59-110">Periksa izin yang diperlukan untuk mengaktifkan manajemen perangkat, mengakses halaman onboarding, atau mengaktifkan/menonaktifkan pemantauan perangkat.</span><span class="sxs-lookup"><span data-stu-id="22d59-110">Check the permissions required to enable device management, access the onboarding page, or turn on/off device monitoring.</span></span> <span data-ttu-id="22d59-111">Untuk informasi lebih lanjut, lihat [izin](https://docs.microsoft.com/microsoft-365/compliance/endpoint-dlp-getting-started#permissions).</span><span class="sxs-lookup"><span data-stu-id="22d59-111">For more info, see [Permissions](https://docs.microsoft.com/microsoft-365/compliance/endpoint-dlp-getting-started#permissions).</span></span>
- <span data-ttu-id="22d59-112">Perangkat onboard ke dalam manajemen Device dengan mengikuti prosedur onboarding Devices.</span><span class="sxs-lookup"><span data-stu-id="22d59-112">Onboard devices into Device management by following the onboarding devices procedure.</span></span> <span data-ttu-id="22d59-113">Jika Anda melewatkan opsi perangkat orientasi (pratinjau) di bawah **setelan**kepatuhan M365, konfirmasikan bahwa Anda memiliki lisensi dan izin yang sesuai yang dirujuk di atas.</span><span class="sxs-lookup"><span data-stu-id="22d59-113">If you're missing the Device Onboarding (preview) option under M365 Compliance  **Settings**, confirm you have the appropriate license and permissions referenced above.</span></span> <span data-ttu-id="22d59-114">Untuk info selengkapnya, lihat [perangkat orientasi](https://docs.microsoft.com/microsoft-365/compliance/endpoint-dlp-getting-started#onboarding-devices).</span><span class="sxs-lookup"><span data-stu-id="22d59-114">For more info, see [Onboarding devices](https://docs.microsoft.com/microsoft-365/compliance/endpoint-dlp-getting-started#onboarding-devices).</span></span> 
- <span data-ttu-id="22d59-115">Buat DLP kebijakan untuk melindungi item sensitif Anda.</span><span class="sxs-lookup"><span data-stu-id="22d59-115">Create DLP policies to protect your sensitive items.</span></span> <span data-ttu-id="22d59-116">Untuk informasi, lihat [akhir DLP kebijakan skenario](https://docs.microsoft.com/microsoft-365/compliance/endpoint-dlp-using?view=o365-worldwide#endpoint-dlp-policy-scenarios).</span><span class="sxs-lookup"><span data-stu-id="22d59-116">For info, see [Endpoint DLP policy scenarios](https://docs.microsoft.com/microsoft-365/compliance/endpoint-dlp-using?view=o365-worldwide#endpoint-dlp-policy-scenarios).</span></span>

<span data-ttu-id="22d59-117">Untuk informasi lebih lanjut tentang Microsoft Endpoint DLP, lihat [Pelajari tentang microsoft 365 Endpoint pencegahan kehilangan data (pratinjau)](https://docs.microsoft.com/microsoft-365/compliance/endpoint-dlp-learn-about).</span><span class="sxs-lookup"><span data-stu-id="22d59-117">For more information on the Microsoft Endpoint DLP, see [Learn about Microsoft 365 Endpoint data loss prevention (preview)](https://docs.microsoft.com/microsoft-365/compliance/endpoint-dlp-learn-about).</span></span>