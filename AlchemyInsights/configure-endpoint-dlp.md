---
title: Mengonfigurasi DLP Titik Akhir
ms.author: pebaum
author: pebaum
manager: scotv
ms.date: 08/03/2020
ms.audience: Admin
ms.topic: article
ms.service: o365-administration
ROBOTS: NOINDEX, NOFOLLOW
localization_priority: Priority
ms.collection: Adm_O365
ms.custom:
- "6108"
- "3200001"
ms.openlocfilehash: 36af769b67f8c9aa4b8d17e9f4f3f3b82c8a8534
ms.sourcegitcommit: db908b3da2c7a6508a77bf4f2c80afb294fadbd1
ms.translationtype: HT
ms.contentlocale: id-ID
ms.lasthandoff: 03/29/2021
ms.locfileid: "51402429"
---
# <a name="configure-endpoint-dlp"></a><span data-ttu-id="34218-102">Mengonfigurasi DLP Titik Akhir</span><span class="sxs-lookup"><span data-stu-id="34218-102">Configure Endpoint DLP</span></span>

<span data-ttu-id="34218-103">DLP Titik Akhir Microsoft memungkinkan Anda memperluas kemampuan pemantauan dan proteksi DLP ke informasi sensitif di perangkat Windows 10.</span><span class="sxs-lookup"><span data-stu-id="34218-103">Microsoft Endpoint DLP allows you to extend DLP protection and monitoring capability to sensitive information on Windows 10 devices.</span></span> <span data-ttu-id="34218-104">Setelah perangkat dimasukkan ke manajemen perangkat, Anda dapat membuat kebijakan DLP untuk menerapkan tindakan perlindungan pada item.</span><span class="sxs-lookup"><span data-stu-id="34218-104">After devices are onboarded into device management, you can create DLP policies to enforce protective actions on items.</span></span> <span data-ttu-id="34218-105">Penjelajah Aktivitas dapat digunakan untuk memantau aktivitas bagi item sensitif.</span><span class="sxs-lookup"><span data-stu-id="34218-105">The Activity Explorer can be used to monitor activity for sensitive items.</span></span> <span data-ttu-id="34218-106">Untuk informasi selengkapnya, lihat [Onboarding perangkat ke manajemen perangkat](https://docs.microsoft.com/microsoft-365/compliance/endpoint-dlp-getting-started#onboarding-devices-into-device-management).</span><span class="sxs-lookup"><span data-stu-id="34218-106">For more info, see [Onboarding devices into device management](https://docs.microsoft.com/microsoft-365/compliance/endpoint-dlp-getting-started#onboarding-devices-into-device-management).</span></span>  

<span data-ttu-id="34218-107">Untuk memulai dengan DLP Titik Akhir:</span><span class="sxs-lookup"><span data-stu-id="34218-107">To get started with Endpoint DLP:</span></span>

- <span data-ttu-id="34218-108">Pastikan Anda memiliki lisensi SKU/langganan yang sesuai.</span><span class="sxs-lookup"><span data-stu-id="34218-108">Ensure you have the appropriate SKU/subscriptions licensing.</span></span> <span data-ttu-id="34218-109">Untuk informasi selengkapnya, lihat [lisensi SKU/langganan](https://docs.microsoft.com/microsoft-365/compliance/endpoint-dlp-getting-started#skusubscriptions-licensing).</span><span class="sxs-lookup"><span data-stu-id="34218-109">For more info, see [SKU/subscriptions licensing](https://docs.microsoft.com/microsoft-365/compliance/endpoint-dlp-getting-started#skusubscriptions-licensing).</span></span>
- <span data-ttu-id="34218-110">Periksa izin yang diperlukan untuk mengaktifkan manajemen perangkat, mengakses halaman onboarding, atau mengaktifkan/menonaktifkan pemantauan perangkat.</span><span class="sxs-lookup"><span data-stu-id="34218-110">Check the permissions required to enable device management, access the onboarding page, or turn on/off device monitoring.</span></span> <span data-ttu-id="34218-111">Untuk informasi selengkapnya, lihat [Izin](https://docs.microsoft.com/microsoft-365/compliance/endpoint-dlp-getting-started#permissions).</span><span class="sxs-lookup"><span data-stu-id="34218-111">For more info, see [Permissions](https://docs.microsoft.com/microsoft-365/compliance/endpoint-dlp-getting-started#permissions).</span></span>
- <span data-ttu-id="34218-112">Masukkan perangkat ke manajemen Perangkat dengan mengikuti prosedur perangkat onboarding.</span><span class="sxs-lookup"><span data-stu-id="34218-112">Onboard devices into Device management by following the onboarding devices procedure.</span></span> <span data-ttu-id="34218-113">Jika Anda tidak dapat menemukan opsi Onboarding Perangkat (pratinjau) di bawah **Pengaturan** Kepatuhan M365, pastikan Anda memiliki lisensi dan izin yang sesuai, seperti yang ditunjukkan di atas.</span><span class="sxs-lookup"><span data-stu-id="34218-113">If you're missing the Device Onboarding (preview) option under M365 Compliance  **Settings**, confirm you have the appropriate license and permissions referenced above.</span></span> <span data-ttu-id="34218-114">Untuk informasi selengkapnya, lihat [Perangkat onboarding](https://docs.microsoft.com/microsoft-365/compliance/endpoint-dlp-getting-started#onboarding-devices).</span><span class="sxs-lookup"><span data-stu-id="34218-114">For more info, see [Onboarding devices](https://docs.microsoft.com/microsoft-365/compliance/endpoint-dlp-getting-started#onboarding-devices).</span></span> 
- <span data-ttu-id="34218-115">Buat kebijakan DLP untuk melindungi item sensitif Anda.</span><span class="sxs-lookup"><span data-stu-id="34218-115">Create DLP policies to protect your sensitive items.</span></span> <span data-ttu-id="34218-116">Untuk penjelasannya, lihat [Skenario kebijakan DLP titik akhir](https://docs.microsoft.com/microsoft-365/compliance/endpoint-dlp-using?view=o365-worldwide#endpoint-dlp-policy-scenarios &preserve-view=true).</span><span class="sxs-lookup"><span data-stu-id="34218-116">For info, see [Endpoint DLP policy scenarios](https://docs.microsoft.com/microsoft-365/compliance/endpoint-dlp-using?view=o365-worldwide#endpoint-dlp-policy-scenarios &preserve-view=true).</span></span>

<span data-ttu-id="34218-117">Untuk informasi selengkapnya tentang DLP Titik Akhir Microsoft, lihat [Pelajari tentang pencegahan kehilangan data Titik Akhir Microsoft 365 (pratinjau)](https://docs.microsoft.com/microsoft-365/compliance/endpoint-dlp-learn-about).</span><span class="sxs-lookup"><span data-stu-id="34218-117">For more information on the Microsoft Endpoint DLP, see [Learn about Microsoft 365 Endpoint data loss prevention (preview)](https://docs.microsoft.com/microsoft-365/compliance/endpoint-dlp-learn-about).</span></span>

<span data-ttu-id="34218-118">**Langkah-langkah Pengumpulan Data Penting, jika Dukungan diperlukan:**</span><span class="sxs-lookup"><span data-stu-id="34218-118">**Important Data Collection steps, if Support is needed:**</span></span>

1. <span data-ttu-id="34218-119">Unduh Pratinjau Penganalisis Klien MDATP dari [https://aka.ms/betamdatpanalyzer](https://aka.ms/betamdatpanalyzer "https://aka.ms/betamdatpanalyzer")</span><span class="sxs-lookup"><span data-stu-id="34218-119">Download MDATP Client Analyzer Preview from [https://aka.ms/betamdatpanalyzer](https://aka.ms/betamdatpanalyzer "https://aka.ms/betamdatpanalyzer")</span></span>
2. <span data-ttu-id="34218-120">Jalankan alat tersebut sebagai Admin dari jendela cmd:</span><span class="sxs-lookup"><span data-stu-id="34218-120">Run the tool as Admin from the cmd window:</span></span>
3. <span data-ttu-id="34218-121">MDATPClientAnalyzerPreview\MDATPClientAnalyzer.cmd –t</span><span class="sxs-lookup"><span data-stu-id="34218-121">MDATPClientAnalyzerPreview\MDATPClientAnalyzer.cmd –t</span></span>
4. <span data-ttu-id="34218-122">Ketika diminta dengan “Masukkan jumlah menit untuk mengumpulkan jejak: ", masukkan jumlah menit yang diperlukan untuk menjalankan skenario</span><span class="sxs-lookup"><span data-stu-id="34218-122">When prompted with “Enter the number of minutes to collect traces: ", enter the number of minutes that are required to run the scenario</span></span>
5. <span data-ttu-id="34218-123">Jalankan skenario</span><span class="sxs-lookup"><span data-stu-id="34218-123">Run the scenario</span></span>

<span data-ttu-id="34218-124">Kumpulkan output file Zip untuk diberikan kepada agen Dukungan.</span><span class="sxs-lookup"><span data-stu-id="34218-124">Collect the Zip file output to be given to the Support agent.</span></span>
