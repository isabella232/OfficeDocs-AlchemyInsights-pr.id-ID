---
title: SharePoint migrasi pelambatan dengan galat 503
ms.author: pebaum
author: pebaum
ms.date: 8/8/2019
ms.audience: ITPro
ms.topic: article
ROBOTS: NOINDEX, NOFOLLOW
localization_priority: Normal
ms.collection: Adm_O365
ms.assetid: ''
ms.custom:
- "9000136"
- "2541"
ms.openlocfilehash: 7e12c74d33e3cee7c626ad899a4e7f2f0a409bca
ms.sourcegitcommit: b0d5b68366028abcf08610672d5bc9d3b25ac433
ms.translationtype: MT
ms.contentlocale: id-ID
ms.lasthandoff: 03/24/2020
ms.locfileid: "42931661"
---
# <a name="sharepoint-migration-throttling-with-503-errors"></a><span data-ttu-id="6d15b-102">SharePoint migrasi pelambatan dengan galat 503</span><span class="sxs-lookup"><span data-stu-id="6d15b-102">SharePoint migration throttling with 503 errors</span></span>

<span data-ttu-id="6d15b-103">**Penting**: banyak SharePoint online dan OneDrive pelanggan menjalankan aplikasi penting bisnis terhadap layanan yang berjalan di latar belakang.</span><span class="sxs-lookup"><span data-stu-id="6d15b-103">**Important**: Many SharePoint Online and OneDrive customers run business-critical applications against the service that run in the background.</span></span> <span data-ttu-id="6d15b-104">Ini termasuk migrasi konten, pencegahan kehilangan data (DLP), dan solusi pencadangan.</span><span class="sxs-lookup"><span data-stu-id="6d15b-104">These include content migration, Data Loss Prevention (DLP), and backup solutions.</span></span> <span data-ttu-id="6d15b-105">Selama waktu yang belum pernah terjadi sebelumnya, kami mengambil langkah untuk memastikan bahwa SharePoint online dan layanan OneDrive tetap sangat tersedia dan dapat diandalkan untuk pengguna yang bergantung pada layanan lebih dari sebelumnya dalam skenario kerja jarak jauh.</span><span class="sxs-lookup"><span data-stu-id="6d15b-105">During these unprecedented times, we are taking steps to ensure that SharePoint Online and OneDrive services remain highly available and reliable for your users who depend on the service more than ever in remote work scenarios.</span></span>

<span data-ttu-id="6d15b-106">Untuk mendukung tujuan ini, kami telah menerapkan batas pelambatan yang lebih ketat pada aplikasi latar belakang (migrasi, DLP dan solusi cadangan) selama jam siang hari kerja.</span><span class="sxs-lookup"><span data-stu-id="6d15b-106">In support of this objective, we have implemented tighter throttling limits on background apps (migration, DLP and backup solutions) during weekday daytime hours.</span></span> <span data-ttu-id="6d15b-107">Anda harus mengharapkan bahwa aplikasi ini akan mencapai throughput yang sangat terbatas selama waktu ini.</span><span class="sxs-lookup"><span data-stu-id="6d15b-107">You should expect that these apps will achieve very limited throughput during these times.</span></span> <span data-ttu-id="6d15b-108">Namun, selama jam malam dan akhir pekan untuk wilayah ini, Layanan akan siap untuk memproses volume permintaan yang jauh lebih tinggi dari aplikasi latar belakang.</span><span class="sxs-lookup"><span data-stu-id="6d15b-108">However, during evening and weekend hours for the region, the service will be ready to process a significantly higher volume of requests from background apps.</span></span>

<span data-ttu-id="6d15b-109">**503 galat saat migrasi ke SharePoint online**</span><span class="sxs-lookup"><span data-stu-id="6d15b-109">**503 errors when migrating to SharePoint Online**</span></span>

<span data-ttu-id="6d15b-110">Tampaknya Anda bermigrasi ke SharePoint online dan menerima 503 kesalahan.</span><span class="sxs-lookup"><span data-stu-id="6d15b-110">It appears you are migrating to SharePoint Online and receiving 503 errors.</span></span> <span data-ttu-id="6d15b-111">Silakan ikuti langkah di bawah ini sehingga kami dapat membantu Anda sesegera mungkin.</span><span class="sxs-lookup"><span data-stu-id="6d15b-111">Please follow the steps below so we may assist you as soon as possible.</span></span> 

1. <span data-ttu-id="6d15b-112">Klik **Hubungi dukungan**, dan kemudian **permintaan layanan baru**.</span><span class="sxs-lookup"><span data-stu-id="6d15b-112">Click **Contact Support**, and then **New Service Request**.</span></span>
2. <span data-ttu-id="6d15b-113">Untuk judul dan deskripsi, ketik **migrasi throttling SharePoint dengan 503**.</span><span class="sxs-lookup"><span data-stu-id="6d15b-113">For the title and description, type **SharePoint Migration Throttling with 503**.</span></span>
3. <span data-ttu-id="6d15b-114">Setelah tiket diserahkan, silakan update dengan informasi berikut:</span><span class="sxs-lookup"><span data-stu-id="6d15b-114">Once the ticket has been submitted, please update it with the following information:</span></span>
    - <span data-ttu-id="6d15b-115">Berapa banyak sisa migrasi (misalnya, berapa banyak TBs?).</span><span class="sxs-lookup"><span data-stu-id="6d15b-115">How much left of migration (for example, how many TBs?).</span></span>
    - <span data-ttu-id="6d15b-116">Tanggal mulai dan akhir migrasi.</span><span class="sxs-lookup"><span data-stu-id="6d15b-116">Migration start and end date.</span></span>
    - <span data-ttu-id="6d15b-117">Jelaskan di mana Anda memigrasi konten, seperti SharePoint Server, kotak, GDrive, berbagi file, dsb.</span><span class="sxs-lookup"><span data-stu-id="6d15b-117">Describe where you are migrating your content from, such as SharePoint Server, Box, GDrive, File shares, etc..</span></span>
    - <span data-ttu-id="6d15b-118">Perkirakan jumlah kesalahan pelambatan (misalnya, x throttle per jam?) dan Kapan pelambatan terjadi.</span><span class="sxs-lookup"><span data-stu-id="6d15b-118">Estimate the number of throttling errors (for example, x throttle per hour?) and when did the throttling happen.</span></span>
    - <span data-ttu-id="6d15b-119">Alat migrasi yang Anda gunakan (misalnya, SPMT atau ShareGate).</span><span class="sxs-lookup"><span data-stu-id="6d15b-119">Which migration tool you are using (for example, SPMT or ShareGate).</span></span>


