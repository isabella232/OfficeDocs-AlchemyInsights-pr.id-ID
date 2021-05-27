---
title: Pemeriksa Titik Akhir Pertahanan memeriksa status sensor
ms.author: pebaum
author: pebaum
manager: scotv
ms.date: 05/21/2021
ms.audience: Admin
ms.topic: article
ms.service: o365-administration
ROBOTS: NOINDEX, NOFOLLOW
localization_priority: Priority
ms.collection: Adm_O365
ms.custom:
- "11084"
- "9003537"
ms.openlocfilehash: a53a0109c3b974806d04135dd2c102de81ec560f
ms.sourcegitcommit: ded29f44e5019b1929218b02733b390899843680
ms.translationtype: MT
ms.contentlocale: id-ID
ms.lasthandoff: 05/24/2021
ms.locfileid: "52676177"
---
# <a name="defender-endpoint-check-sensor-status"></a><span data-ttu-id="6a1c6-102">Pemeriksa Titik Akhir Pertahanan memeriksa status sensor</span><span class="sxs-lookup"><span data-stu-id="6a1c6-102">Defender Endpoint check sensor status</span></span>

<span data-ttu-id="6a1c6-103">Petak **Perangkat dengan masalah sensor** berada di dasbor Operasi Keamanan.</span><span class="sxs-lookup"><span data-stu-id="6a1c6-103">The **Devices with sensor issues** tile is located on the Security Operations dashboard.</span></span> <span data-ttu-id="6a1c6-104">Ubin ini menyediakan informasi dalam kemampuan perangkat individu untuk menyediakan data sensor dan berkomunikasi dengan Pertahanan untuk layanan Titik Akhir.</span><span class="sxs-lookup"><span data-stu-id="6a1c6-104">This tile provides information on the individual device’s ability to provide sensor data and communicate with the Defender for Endpoint service.</span></span> <span data-ttu-id="6a1c6-105">Laporan ini melaporkan berapa banyak perangkat yang memerlukan perhatian dan membantu Anda mengidentifikasi perangkat yang bermasalah dan mengambil tindakan untuk memperbaiki masalah yang diketahui.</span><span class="sxs-lookup"><span data-stu-id="6a1c6-105">It reports how many devices require attention and helps you identify problematic devices and take action to correct known issues.</span></span>

<span data-ttu-id="6a1c6-106">Dua indikator status pada ubin memberikan informasi tentang jumlah perangkat yang tidak melaporkan dengan benar ke layanan:</span><span class="sxs-lookup"><span data-stu-id="6a1c6-106">Two status indicators on the tile provide information on the number of devices not reporting properly to the service:</span></span>

- <span data-ttu-id="6a1c6-107">**Salah konfigurasikan** Perangkat yang mungkin sebagian melaporkan data sensor ke Pertahanan untuk layanan Titik Akhir dan mungkin memiliki kesalahan konfigurasi yang perlu diperbaiki.</span><span class="sxs-lookup"><span data-stu-id="6a1c6-107">**Misconfigured** Devices that might partially be reporting sensor data to the Defender for Endpoint service and might have configuration errors that need to be corrected.</span></span>
- <span data-ttu-id="6a1c6-108">**Tidak Aktif** Perangkat yang telah berhenti melaporkan ke layanan Pertahanan untuk Titik Akhir selama lebih dari tujuh hari dalam sebulan terakhir.</span><span class="sxs-lookup"><span data-stu-id="6a1c6-108">**Inactive** Devices that have stopped reporting to the Defender for Endpoint service for more than seven days in the past month.</span></span>

<span data-ttu-id="6a1c6-109">Mengklik salah satu grup mengarahkan Anda ke daftar Perangkat, difilter menurut pilihan Anda.</span><span class="sxs-lookup"><span data-stu-id="6a1c6-109">Clicking any of the groups directs you to Devices list, filtered according to your choices.</span></span> <span data-ttu-id="6a1c6-110">Pada daftar Perangkat, Anda bisa memfilter daftar status kesehatan dengan status berikut ini:</span><span class="sxs-lookup"><span data-stu-id="6a1c6-110">On the Devices list, you can filter the health state list by the following status:</span></span>

- <span data-ttu-id="6a1c6-111">**Aktif** Perangkat yang secara aktif melaporkan ke Pertahanan untuk layanan Titik Akhir.</span><span class="sxs-lookup"><span data-stu-id="6a1c6-111">**Active** Devices that are actively reporting to the Defender for Endpoint service.</span></span>
- <span data-ttu-id="6a1c6-112">**Salah konfigurasikan** Perangkat yang mungkin sebagian melaporkan data sensor ke Pertahanan untuk layanan Titik Akhir tetapi memiliki kesalahan konfigurasi yang perlu diperbaiki.</span><span class="sxs-lookup"><span data-stu-id="6a1c6-112">**Misconfigured** Devices that might partially be reporting sensor data to the Defender for Endpoint service but have configuration errors that need to be corrected.</span></span> <span data-ttu-id="6a1c6-113">Perangkat yang dikonfigurasi dengan tidak benar dapat memiliki satu atau kombinasi masalah berikut ini:</span><span class="sxs-lookup"><span data-stu-id="6a1c6-113">Misconfigured devices can have either one or a combination of the following issues:</span></span>

    - <span data-ttu-id="6a1c6-114">Tidak ada data sensor - Perangkat telah berhenti mengirim data sensor.</span><span class="sxs-lookup"><span data-stu-id="6a1c6-114">No sensor data - Devices has stopped sending sensor data.</span></span> <span data-ttu-id="6a1c6-115">Peringatan terbatas dapat dipicu dari perangkat.</span><span class="sxs-lookup"><span data-stu-id="6a1c6-115">Limited alerts can be triggered from the device.</span></span>
    - <span data-ttu-id="6a1c6-116">Komunikasi yang terganggu - Kemampuan untuk berkomunikasi dengan perangkat mengalami gangguan.</span><span class="sxs-lookup"><span data-stu-id="6a1c6-116">Impaired communications - Ability to communicate with device is impaired.</span></span> <span data-ttu-id="6a1c6-117">Mengirim file untuk analisis mendalam, memblokir file, memisahkan perangkat dari jaringan, dan tindakan lain yang memerlukan komunikasi dengan perangkat mungkin tidak berfungsi.</span><span class="sxs-lookup"><span data-stu-id="6a1c6-117">Sending files for deep analysis, blocking files, isolating device from network and other actions that require communication with the device may not work.</span></span>
- <span data-ttu-id="6a1c6-118">**Tidak Aktif** Perangkat yang telah berhenti melaporkan ke Layanan Pertahanan untuk Titik Akhir.</span><span class="sxs-lookup"><span data-stu-id="6a1c6-118">**Inactive** Devices that have stopped reporting to the Defender for Endpoint service.</span></span>

<span data-ttu-id="6a1c6-119">Anda dapat mengunduh seluruh daftar dalam format CSV menggunakan fitur Ekspor.</span><span class="sxs-lookup"><span data-stu-id="6a1c6-119">You can download the entire list in CSV format using the Export feature.</span></span>

<span data-ttu-id="6a1c6-120">Untuk informasi selengkapnya, lihat [Memeriksa status kesehatan sensor di Pertahanan Microsoft untuk Titik Akhir.](/microsoft-365/security/defender-endpoint/check-sensor-status)</span><span class="sxs-lookup"><span data-stu-id="6a1c6-120">For more information, see [Check sensor health state in Microsoft Defender for Endpoint](/microsoft-365/security/defender-endpoint/check-sensor-status).</span></span>

<span data-ttu-id="6a1c6-121">Untuk informasi selengkapnya tentang hal yang menyebabkan perangkat tidak aktif atau salah konfigurasikan, lihat Memperbaiki sensor yang tidak sehat di [Pertahanan Microsoft untuk Titik Akhir.](/microsoft-365/security/defender-endpoint/fix-unhealthy-sensors)</span><span class="sxs-lookup"><span data-stu-id="6a1c6-121">For more information about what caused a device to be inactive or misconfigured, see [Fix unhealthy sensors in Microsoft Defender for Endpoint](/microsoft-365/security/defender-endpoint/fix-unhealthy-sensors).</span></span>
