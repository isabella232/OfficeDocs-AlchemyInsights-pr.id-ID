---
title: Memigrasi opsi ke SharePoint online
ms.author: pebaum
author: v-miegge
manager: v-cojank
ms.date: 11/04/2019
ms.audience: ITPro
ms.topic: article
ROBOTS: NOINDEX, NOFOLLOW
localization_priority: Normal
ms.collection: Adm_O365
ms.assetid: c8c339c9-2e50-4daa-aa91-3eb5053e2bc6
ms.openlocfilehash: 830b39c51658cbc02f4be81acdfdf3b164a8df70
ms.sourcegitcommit: b0d5b68366028abcf08610672d5bc9d3b25ac433
ms.translationtype: MT
ms.contentlocale: id-ID
ms.lasthandoff: 03/24/2020
ms.locfileid: "42932733"
---
# <a name="migrate-options-to-sharepoint-online"></a><span data-ttu-id="7a1cd-102">Memigrasi opsi ke SharePoint online</span><span class="sxs-lookup"><span data-stu-id="7a1cd-102">Migrate options to SharePoint Online</span></span>

<span data-ttu-id="7a1cd-103">**Penting**: banyak SharePoint online dan OneDrive pelanggan menjalankan aplikasi penting bisnis terhadap layanan yang berjalan di latar belakang.</span><span class="sxs-lookup"><span data-stu-id="7a1cd-103">**Important**: Many SharePoint Online and OneDrive customers run business-critical applications against the service that run in the background.</span></span> <span data-ttu-id="7a1cd-104">Ini termasuk migrasi konten, pencegahan kehilangan data (DLP), dan solusi pencadangan.</span><span class="sxs-lookup"><span data-stu-id="7a1cd-104">These include content migration, Data Loss Prevention (DLP), and backup solutions.</span></span> <span data-ttu-id="7a1cd-105">Selama waktu yang belum pernah terjadi sebelumnya, kami mengambil langkah untuk memastikan bahwa SharePoint online dan layanan OneDrive tetap sangat tersedia dan dapat diandalkan untuk pengguna yang bergantung pada layanan lebih dari sebelumnya dalam skenario kerja jarak jauh.</span><span class="sxs-lookup"><span data-stu-id="7a1cd-105">During these unprecedented times, we are taking steps to ensure that SharePoint Online and OneDrive services remain highly available and reliable for your users who depend on the service more than ever in remote work scenarios.</span></span>

<span data-ttu-id="7a1cd-106">Untuk mendukung tujuan ini, kami telah menerapkan batas pelambatan yang lebih ketat pada aplikasi latar belakang (migrasi, DLP dan solusi cadangan) selama jam siang hari kerja.</span><span class="sxs-lookup"><span data-stu-id="7a1cd-106">In support of this objective, we have implemented tighter throttling limits on background apps (migration, DLP and backup solutions) during weekday daytime hours.</span></span> <span data-ttu-id="7a1cd-107">Anda harus mengharapkan bahwa aplikasi ini akan mencapai throughput yang sangat terbatas selama waktu ini.</span><span class="sxs-lookup"><span data-stu-id="7a1cd-107">You should expect that these apps will achieve very limited throughput during these times.</span></span> <span data-ttu-id="7a1cd-108">Namun, selama jam malam dan akhir pekan untuk wilayah ini, Layanan akan siap untuk memproses volume permintaan yang jauh lebih tinggi dari aplikasi latar belakang.</span><span class="sxs-lookup"><span data-stu-id="7a1cd-108">However, during evening and weekend hours for the region, the service will be ready to process a significantly higher volume of requests from background apps.</span></span>

<span data-ttu-id="7a1cd-109">**Opsi migrasi**</span><span class="sxs-lookup"><span data-stu-id="7a1cd-109">**Migration options**</span></span>

<span data-ttu-id="7a1cd-110">Ada pilihan yang berbeda yang tersedia untuk bermigrasi konten ke SharePoint online, tergantung pada ukuran dan jumlah file yang Anda butuhkan untuk bergerak, silakan lihat daftar pilihan yang [terletak di sini](https://docs.microsoft.com/sharepointmigration/migrate-to-sharepoint-online).</span><span class="sxs-lookup"><span data-stu-id="7a1cd-110">There are different options available to migrate content to SharePoint Online, depending on the size and quantity of files you need to move, please see a list of options [located here](https://docs.microsoft.com/sharepointmigration/migrate-to-sharepoint-online).</span></span>

<span data-ttu-id="7a1cd-111">Untuk informasi lebih lanjut tentang migrasi konten, silakan kunjungi link di bawah ini.</span><span class="sxs-lookup"><span data-stu-id="7a1cd-111">For more information on content migration, please visit the links below.</span></span>

- [<span data-ttu-id="7a1cd-112">Alat migrasi SharePoint</span><span class="sxs-lookup"><span data-stu-id="7a1cd-112">Sharepoint Migration Tool</span></span>](https://docs.microsoft.com/sharepointmigration/introducing-the-sharepoint-migration-tool)

- [<span data-ttu-id="7a1cd-113">Memulai Migration Manager</span><span class="sxs-lookup"><span data-stu-id="7a1cd-113">Get started with the Migration Manager</span></span>](https://docs.microsoft.com/sharepointmigration/mm-get-started)

- [<span data-ttu-id="7a1cd-114">SharePoint online dan kecepatan migrasi ODB</span><span class="sxs-lookup"><span data-stu-id="7a1cd-114">Sharepoint Online and ODB Migration Speed</span></span>](https://docs.microsoft.com/sharepointmigration/sharepoint-online-and-onedrive-migration-speed)

- [<span data-ttu-id="7a1cd-115">Hindari mendapatkan mengalami kelambatan atau diblokir di SharePoint online</span><span class="sxs-lookup"><span data-stu-id="7a1cd-115">Avoid getting throttled or blocked in SharePoint Online</span></span>](https://docs.microsoft.com/sharepoint/dev/general-development/how-to-avoid-getting-throttled-or-blocked-in-sharepoint-online)

- [<span data-ttu-id="7a1cd-116">Alat penilaian migrasi SharePoint (SMAT)</span><span class="sxs-lookup"><span data-stu-id="7a1cd-116">SharePoint Migration Assessment Tool (SMAT)</span></span>](https://www.microsoft.com/download/details.aspx?id=53598&amp;751be11f-ede8-5a0c-058c-2ee190a24fa6=True)

<span data-ttu-id="7a1cd-117">**Catatan**: saat ini alat SharePoint migrasi hanya mendukung migrasi dari SharePoint 2010 dan 2013.</span><span class="sxs-lookup"><span data-stu-id="7a1cd-117">**Note**: Currently the SharePoint Migration tool only support migrations from SharePoint 2010  and 2013.</span></span> <span data-ttu-id="7a1cd-118">Versi 2016 atau 2019 tidak didukung saat ini.</span><span class="sxs-lookup"><span data-stu-id="7a1cd-118">Version 2016 or 2019 are not supported at this time.</span></span>
