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
ms.openlocfilehash: b9369b2c2ca31f7d2fceac37ef1e2252b82e933b
ms.sourcegitcommit: 0c104e2bd34ccc09bcea389e470692e92bcf1f8f
ms.translationtype: MT
ms.contentlocale: id-ID
ms.lasthandoff: 05/26/2021
ms.locfileid: "52657932"
---
# <a name="configure-endpoint-dlp"></a><span data-ttu-id="fb99d-102">Mengonfigurasi DLP Titik Akhir</span><span class="sxs-lookup"><span data-stu-id="fb99d-102">Configure Endpoint DLP</span></span>

<span data-ttu-id="fb99d-103">DLP Titik Akhir Microsoft memungkinkan Anda memperluas kemampuan pemantauan dan proteksi DLP ke informasi sensitif di perangkat Windows 10.</span><span class="sxs-lookup"><span data-stu-id="fb99d-103">Microsoft Endpoint DLP allows you to extend DLP protection and monitoring capability to sensitive information on Windows 10 devices.</span></span> <span data-ttu-id="fb99d-104">Setelah perangkat dimasukkan ke manajemen perangkat, Anda dapat membuat kebijakan DLP untuk menerapkan tindakan perlindungan pada item.</span><span class="sxs-lookup"><span data-stu-id="fb99d-104">After devices are onboarded into device management, you can create DLP policies to enforce protective actions on items.</span></span> <span data-ttu-id="fb99d-105">Penjelajah Aktivitas dapat digunakan untuk memantau aktivitas bagi item sensitif.</span><span class="sxs-lookup"><span data-stu-id="fb99d-105">The Activity Explorer can be used to monitor activity for sensitive items.</span></span> <span data-ttu-id="fb99d-106">Untuk informasi selengkapnya, lihat [Onboarding perangkat ke manajemen perangkat](/microsoft-365/compliance/endpoint-dlp-getting-started#onboarding-devices-into-device-management).</span><span class="sxs-lookup"><span data-stu-id="fb99d-106">For more info, see [Onboarding devices into device management](/microsoft-365/compliance/endpoint-dlp-getting-started#onboarding-devices-into-device-management).</span></span>  

<span data-ttu-id="fb99d-107">Untuk memulai dengan DLP Titik Akhir:</span><span class="sxs-lookup"><span data-stu-id="fb99d-107">To get started with Endpoint DLP:</span></span>

- <span data-ttu-id="fb99d-108">Pastikan Anda memiliki lisensi SKU/langganan yang sesuai.</span><span class="sxs-lookup"><span data-stu-id="fb99d-108">Ensure you have the appropriate SKU/subscriptions licensing.</span></span> <span data-ttu-id="fb99d-109">Untuk informasi selengkapnya, lihat [lisensi SKU/langganan](/microsoft-365/compliance/endpoint-dlp-getting-started#skusubscriptions-licensing).</span><span class="sxs-lookup"><span data-stu-id="fb99d-109">For more info, see [SKU/subscriptions licensing](/microsoft-365/compliance/endpoint-dlp-getting-started#skusubscriptions-licensing).</span></span>
- <span data-ttu-id="fb99d-110">Periksa izin yang diperlukan untuk mengaktifkan manajemen perangkat, mengakses halaman onboarding, atau mengaktifkan/menonaktifkan pemantauan perangkat.</span><span class="sxs-lookup"><span data-stu-id="fb99d-110">Check the permissions required to enable device management, access the onboarding page, or turn on/off device monitoring.</span></span> <span data-ttu-id="fb99d-111">Untuk informasi selengkapnya, lihat [Izin](/microsoft-365/compliance/endpoint-dlp-getting-started#permissions).</span><span class="sxs-lookup"><span data-stu-id="fb99d-111">For more info, see [Permissions](/microsoft-365/compliance/endpoint-dlp-getting-started#permissions).</span></span>
- <span data-ttu-id="fb99d-112">Masukkan perangkat ke manajemen Perangkat dengan mengikuti prosedur perangkat onboarding.</span><span class="sxs-lookup"><span data-stu-id="fb99d-112">Onboard devices into Device management by following the onboarding devices procedure.</span></span> <span data-ttu-id="fb99d-113">Untuk informasi selengkapnya, lihat [Perangkat onboarding](/microsoft-365/compliance/endpoint-dlp-getting-started#onboarding-devices).</span><span class="sxs-lookup"><span data-stu-id="fb99d-113">For more info, see [Onboarding devices](/microsoft-365/compliance/endpoint-dlp-getting-started#onboarding-devices).</span></span> 
- <span data-ttu-id="fb99d-114">Buat kebijakan DLP untuk melindungi item sensitif Anda.</span><span class="sxs-lookup"><span data-stu-id="fb99d-114">Create DLP policies to protect your sensitive items.</span></span> <span data-ttu-id="fb99d-115">Untuk penjelasannya, lihat [Skenario kebijakan DLP titik akhir](/microsoft-365/compliance/endpoint-dlp-using?view=o365-worldwide#endpoint-dlp-policy-scenarios).</span><span class="sxs-lookup"><span data-stu-id="fb99d-115">For info, see [Endpoint DLP policy scenarios](/microsoft-365/compliance/endpoint-dlp-using?view=o365-worldwide#endpoint-dlp-policy-scenarios).</span></span>

<span data-ttu-id="fb99d-116">Untuk informasi selengkapnya tentang DLP Titik Akhir Microsoft, lihat [Pelajari tentang pencegahan kehilangan data Titik Akhir Microsoft 365 (pratinjau)](/microsoft-365/compliance/endpoint-dlp-learn-about).</span><span class="sxs-lookup"><span data-stu-id="fb99d-116">For more information on the Microsoft Endpoint DLP, see [Learn about Microsoft 365 Endpoint data loss prevention (preview)](/microsoft-365/compliance/endpoint-dlp-learn-about).</span></span>

<span data-ttu-id="fb99d-117">**Langkah-langkah Pengumpulan Data Penting, jika Dukungan diperlukan:**</span><span class="sxs-lookup"><span data-stu-id="fb99d-117">**Important Data Collection steps, if Support is needed:**</span></span>

1. <span data-ttu-id="fb99d-118">Unduh [MDATP Client Analyzer Preview.](https://aka.ms/betamdatpanalyzer)</span><span class="sxs-lookup"><span data-stu-id="fb99d-118">Download [MDATP Client Analyzer Preview](https://aka.ms/betamdatpanalyzer).</span></span>
1. <span data-ttu-id="fb99d-119">Jalankan alat tersebut sebagai Admin dari jendela cmd:</span><span class="sxs-lookup"><span data-stu-id="fb99d-119">Run the tool as Admin from the cmd window:</span></span>

    <span data-ttu-id="fb99d-120">**MDATPClientAnalyzerPreview\MDATPClientAnalyzer.cmd –t**</span><span class="sxs-lookup"><span data-stu-id="fb99d-120">**MDATPClientAnalyzerPreview\MDATPClientAnalyzer.cmd –t**</span></span>

1. <span data-ttu-id="fb99d-121">Ketika diminta dengan **Masukkan jumlah menit untuk mengumpulkan penelusuran:**, masukkan jumlah menit yang diperlukan untuk menjalankan skenario.</span><span class="sxs-lookup"><span data-stu-id="fb99d-121">When prompted with **Enter the number of minutes to collect traces:**, enter the number of minutes required to run the scenario.</span></span>
1. <span data-ttu-id="fb99d-122">Jalankan skenario.</span><span class="sxs-lookup"><span data-stu-id="fb99d-122">Run the scenario.</span></span>

<span data-ttu-id="fb99d-123">Kumpulkan output file Zip untuk diberikan kepada agen Dukungan.</span><span class="sxs-lookup"><span data-stu-id="fb99d-123">Collect the Zip file output to give to the Support agent.</span></span>
