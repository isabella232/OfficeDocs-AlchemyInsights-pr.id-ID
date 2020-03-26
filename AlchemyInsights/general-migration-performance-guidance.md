---
title: Panduan kinerja migrasi umum
ms.author: pebaum
author: pebaum
ms.audience: ITPro
ms.topic: article
ROBOTS: NOINDEX, NOFOLLOW
localization_priority: Priority
ms.assetid: 686e8f18-b871-4dd2-864f-8562947ab583
ms.collection: Adm_O365
ms.custom:
- "5300030"
- "3179"
ms.openlocfilehash: 10a0069c41d2e5128b2592425d815364a83b730f
ms.sourcegitcommit: b0d5b68366028abcf08610672d5bc9d3b25ac433
ms.translationtype: HT
ms.contentlocale: id-ID
ms.lasthandoff: 03/24/2020
ms.locfileid: "42932482"
---
# <a name="general-migration-performance-guidance"></a><span data-ttu-id="b5961-102">Panduan kinerja migrasi umum</span><span class="sxs-lookup"><span data-stu-id="b5961-102">General migration performance guidance</span></span>

<span data-ttu-id="b5961-103">**Penting**: Banyak pelanggan SharePoint Online dan OneDrive menjalankan aplikasi yang sangat penting bagi bisnis di samping layanan yang berjalan di latar belakang.</span><span class="sxs-lookup"><span data-stu-id="b5961-103">**Important**: Many SharePoint Online and OneDrive customers run business-critical applications against the service that run in the background.</span></span> <span data-ttu-id="b5961-104">Aplikasi ini mencakup migrasi konten, Pencegahan Kehilangan Data (DLP), dan solusi pencadangan.</span><span class="sxs-lookup"><span data-stu-id="b5961-104">These include content migration, Data Loss Prevention (DLP), and backup solutions.</span></span> <span data-ttu-id="b5961-105">Selama masa yang belum pernah terjadi ini, kami mengambil langkah-langkah untuk memastikan bahwa layanan SharePoint Online dan OneDrive tetap tersedia dan dapat diandalkan bagi pengguna Anda yang bergantung pada layanan ini lebih daripada sebelumnya dalam skenario kerja jarak jauh.</span><span class="sxs-lookup"><span data-stu-id="b5961-105">During these unprecedented times, we are taking steps to ensure that SharePoint Online and OneDrive services remain highly available and reliable for your users who depend on the service more than ever in remote work scenarios.</span></span>

<span data-ttu-id="b5961-106">Untuk mendukung tujuan ini, kami telah menerapkan pembatasan yang lebih ketat pada aplikasi latar belakang (migrasi, DLP, dan solusi cadangan) selama jam kerja siang pada hari kerja.</span><span class="sxs-lookup"><span data-stu-id="b5961-106">In support of this objective, we have implemented tighter throttling limits on background apps (migration, DLP and backup solutions) during weekday daytime hours.</span></span> <span data-ttu-id="b5961-107">Anda hendaknya mengantisipasi bahwa aplikasi ini akan mencapai throughput yang sangat terbatas dalam kurun waktu ini.</span><span class="sxs-lookup"><span data-stu-id="b5961-107">You should expect that these apps will achieve very limited throughput during these times.</span></span> <span data-ttu-id="b5961-108">Namun, selama jam malam dan akhir pekan untuk wilayah ini, layanan akan siap untuk memproses jauh lebih banyak volume permintaan dari aplikasi latar belakang.</span><span class="sxs-lookup"><span data-stu-id="b5961-108">However, during evening and weekend hours for the region, the service will be ready to process a significantly higher volume of requests from background apps.</span></span>

<span data-ttu-id="b5961-109">**Panduan kinerja migrasi**</span><span class="sxs-lookup"><span data-stu-id="b5961-109">**Migration performance guidance**</span></span>

<span data-ttu-id="b5961-110">Kinerja migrasi dapat dipengaruhi oleh infrastruktur jaringan, ukuran file, waktu migrasi, dan pembatasan.</span><span class="sxs-lookup"><span data-stu-id="b5961-110">Migration performance can be impacted by network infrastructure, file size, migration time, and throttling.</span></span> <span data-ttu-id="b5961-111">Memahami hal ini akan membantu Anda dalam merencanakan dan memaksimalkan efisiensi migrasi.</span><span class="sxs-lookup"><span data-stu-id="b5961-111">Understanding these will help you plan and maximize the efficiency of your migration.</span></span>

- [<span data-ttu-id="b5961-112">Panduan kinerja migrasi umum</span><span class="sxs-lookup"><span data-stu-id="b5961-112">General migration performance guidance</span></span>](https://docs.microsoft.com/sharepointmigration/sharepoint-online-and-onedrive-migration-speed)
