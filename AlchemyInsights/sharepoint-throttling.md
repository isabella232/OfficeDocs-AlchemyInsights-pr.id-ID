---
title: Pelambatan SharePoint online
ms.author: pebaum
author: pebaum
ms.audience: ITPro
ms.topic: article
ROBOTS: NOINDEX, NOFOLLOW
localization_priority: Normal
ms.assetid: b376d8ea-50c4-47f0-9720-50d80aa3f7f1
ms.openlocfilehash: 9af4f09d50992c04a1f3d5a164093049a3ec3517
ms.sourcegitcommit: b0d5b68366028abcf08610672d5bc9d3b25ac433
ms.translationtype: MT
ms.contentlocale: id-ID
ms.lasthandoff: 03/24/2020
ms.locfileid: "42931445"
---
# <a name="sharepoint-online-throttling"></a><span data-ttu-id="6932b-102">Pelambatan SharePoint online</span><span class="sxs-lookup"><span data-stu-id="6932b-102">SharePoint Online throttling</span></span>

<span data-ttu-id="6932b-103">**Penting**: banyak SharePoint online dan OneDrive pelanggan menjalankan aplikasi penting bisnis terhadap layanan yang berjalan di latar belakang.</span><span class="sxs-lookup"><span data-stu-id="6932b-103">**Important**: Many SharePoint Online and OneDrive customers run business-critical applications against the service that run in the background.</span></span> <span data-ttu-id="6932b-104">Ini termasuk migrasi konten, pencegahan kehilangan data (DLP), dan solusi pencadangan.</span><span class="sxs-lookup"><span data-stu-id="6932b-104">These include content migration, Data Loss Prevention (DLP), and backup solutions.</span></span> <span data-ttu-id="6932b-105">Selama waktu yang belum pernah terjadi sebelumnya, kami mengambil langkah untuk memastikan bahwa SharePoint online dan layanan OneDrive tetap sangat tersedia dan dapat diandalkan untuk pengguna yang bergantung pada layanan lebih dari sebelumnya dalam skenario kerja jarak jauh.</span><span class="sxs-lookup"><span data-stu-id="6932b-105">During these unprecedented times, we are taking steps to ensure that SharePoint Online and OneDrive services remain highly available and reliable for your users who depend on the service more than ever in remote work scenarios.</span></span>

<span data-ttu-id="6932b-106">Untuk mendukung tujuan ini, kami telah menerapkan batas pelambatan yang lebih ketat pada aplikasi latar belakang (migrasi, DLP dan solusi cadangan) selama jam siang hari kerja.</span><span class="sxs-lookup"><span data-stu-id="6932b-106">In support of this objective, we have implemented tighter throttling limits on background apps (migration, DLP and backup solutions) during weekday daytime hours.</span></span> <span data-ttu-id="6932b-107">Anda harus mengharapkan bahwa aplikasi ini akan mencapai throughput yang sangat terbatas selama waktu ini.</span><span class="sxs-lookup"><span data-stu-id="6932b-107">You should expect that these apps will achieve very limited throughput during these times.</span></span> <span data-ttu-id="6932b-108">Namun, selama jam malam dan akhir pekan untuk wilayah ini, Layanan akan siap untuk memproses volume permintaan yang jauh lebih tinggi dari aplikasi latar belakang.</span><span class="sxs-lookup"><span data-stu-id="6932b-108">However, during evening and weekend hours for the region, the service will be ready to process a significantly higher volume of requests from background apps.</span></span>

<span data-ttu-id="6932b-109">**Pelambatan SharePoint online**</span><span class="sxs-lookup"><span data-stu-id="6932b-109">**SharePoint Online throttling**</span></span>

<span data-ttu-id="6932b-110">SharePoint Online menggunakan pelambatan untuk mempertahankan kinerja optimal dan keandalan Layanan SharePoint online.</span><span class="sxs-lookup"><span data-stu-id="6932b-110">SharePoint Online uses throttling to maintain optimal performance and reliability of the SharePoint Online service.</span></span> <span data-ttu-id="6932b-111">Pelambatan membatasi jumlah tindakan pengguna atau panggilan bersamaan (dengan skrip atau kode) untuk mencegah penggunaan sumber daya berlebihan.</span><span class="sxs-lookup"><span data-stu-id="6932b-111">Throttling limits the number of user actions or concurrent calls (by script or code) to prevent overuse of resources.</span></span> <span data-ttu-id="6932b-112">Untuk informasi lebih lanjut, silakan kunjungi link di bawah ini.</span><span class="sxs-lookup"><span data-stu-id="6932b-112">For more information, please visit the links below.</span></span>

- [<span data-ttu-id="6932b-113">Hindari mendapatkan mengalami kelambatan atau diblokir di SharePoint online</span><span class="sxs-lookup"><span data-stu-id="6932b-113">Avoid getting throttled or blocked in SharePoint Online</span></span>](https://docs.microsoft.com/sharepoint/dev/general-development/how-to-avoid-getting-throttled-or-blocked-in-sharepoint-online)

- [<span data-ttu-id="6932b-114">Data migrasi dan SPO throttling</span><span class="sxs-lookup"><span data-stu-id="6932b-114">Data Migration and SPO Throttling </span></span>](https://blogs.technet.microsoft.com/sposupport/2017/08/12/data-migration-and-spo-service-throttling/)

- [<span data-ttu-id="6932b-115">SharePoint online dan OneDrive kecepatan migrasi</span><span class="sxs-lookup"><span data-stu-id="6932b-115">SharePoint Online and OneDrive Migration Speed</span></span>](https://docs.microsoft.com/sharepointmigration/sharepoint-online-and-onedrive-migration-speed)

 - [<span data-ttu-id="6932b-116">Menangani SharePoint online pelambatan menggunakan eksponensial mundur</span><span class="sxs-lookup"><span data-stu-id="6932b-116">Handle SharePoint Online throttling by using exponential back off</span></span>](https://docs.microsoft.com/sharepoint/dev/solution-guidance/handle-sharepoint-online-throttling-by-using-exponential-back-off)

- [<span data-ttu-id="6932b-117">Perencanaan kapasitas dan pengujian beban SharePoint online</span><span class="sxs-lookup"><span data-stu-id="6932b-117">Capacity planning and load testing SharePoint Online</span></span>](https://docs.microsoft.com/office365/enterprise/capacity-planning-and-load-testing-sharepoint-online)

