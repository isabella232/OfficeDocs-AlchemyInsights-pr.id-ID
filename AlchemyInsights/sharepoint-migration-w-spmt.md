---
title: SharePoint migrasi dengan SPMT
ms.author: v-todmc
author: todmccoy
manager: mnirkhe
ms.date: 9/18/19
ms.audience: Admin
ms.topic: article
ROBOTS: NOINDEX, NOFOLLOW
localization_priority: Normal
ms.collection: Adm_O365
ms.custom:
- "5300030"
- "2594"
ms.openlocfilehash: e7719d1fc6dda0d5bd340775219401dade2933fe
ms.sourcegitcommit: b0d5b68366028abcf08610672d5bc9d3b25ac433
ms.translationtype: MT
ms.contentlocale: id-ID
ms.lasthandoff: 03/24/2020
ms.locfileid: "42931553"
---
# <a name="sharepoint-migration-with-spmt"></a><span data-ttu-id="28ccf-102">SharePoint migrasi dengan SPMT</span><span class="sxs-lookup"><span data-stu-id="28ccf-102">SharePoint Migration with SPMT</span></span>

<span data-ttu-id="28ccf-103">**Penting**: banyak SharePoint online dan OneDrive pelanggan menjalankan aplikasi penting bisnis terhadap layanan yang berjalan di latar belakang.</span><span class="sxs-lookup"><span data-stu-id="28ccf-103">**Important**: Many SharePoint Online and OneDrive customers run business-critical applications against the service that run in the background.</span></span> <span data-ttu-id="28ccf-104">Ini termasuk migrasi konten, pencegahan kehilangan data (DLP), dan solusi pencadangan.</span><span class="sxs-lookup"><span data-stu-id="28ccf-104">These include content migration, Data Loss Prevention (DLP), and backup solutions.</span></span> <span data-ttu-id="28ccf-105">Selama waktu yang belum pernah terjadi sebelumnya, kami mengambil langkah untuk memastikan bahwa SharePoint online dan layanan OneDrive tetap sangat tersedia dan dapat diandalkan untuk pengguna yang bergantung pada layanan lebih dari sebelumnya dalam skenario kerja jarak jauh.</span><span class="sxs-lookup"><span data-stu-id="28ccf-105">During these unprecedented times, we are taking steps to ensure that SharePoint Online and OneDrive services remain highly available and reliable for your users who depend on the service more than ever in remote work scenarios.</span></span>

<span data-ttu-id="28ccf-106">Untuk mendukung tujuan ini, kami telah menerapkan batas pelambatan yang lebih ketat pada aplikasi latar belakang (migrasi, DLP dan solusi cadangan) selama jam siang hari kerja.</span><span class="sxs-lookup"><span data-stu-id="28ccf-106">In support of this objective, we have implemented tighter throttling limits on background apps (migration, DLP and backup solutions) during weekday daytime hours.</span></span> <span data-ttu-id="28ccf-107">Anda harus mengharapkan bahwa aplikasi ini akan mencapai throughput yang sangat terbatas selama waktu ini.</span><span class="sxs-lookup"><span data-stu-id="28ccf-107">You should expect that these apps will achieve very limited throughput during these times.</span></span> <span data-ttu-id="28ccf-108">Namun, selama jam malam dan akhir pekan untuk wilayah ini, Layanan akan siap untuk memproses volume permintaan yang jauh lebih tinggi dari aplikasi latar belakang.</span><span class="sxs-lookup"><span data-stu-id="28ccf-108">However, during evening and weekend hours for the region, the service will be ready to process a significantly higher volume of requests from background apps.</span></span>

<span data-ttu-id="28ccf-109">**Alat migrasi SharePoint**</span><span class="sxs-lookup"><span data-stu-id="28ccf-109">**SharePoint Migration Tool**</span></span>

<span data-ttu-id="28ccf-110">Dirancang untuk digunakan untuk migrasi mulai dari set terkecil file ke migrasi perusahaan berskala besar, SharePoint Migration tool akan memungkinkan Anda untuk mentransfer informasi Anda ke awan dan mengambil keuntungan dari kolaborasi terbaru, kecerdasan, dan solusi keamanan dengan Office 365.</span><span class="sxs-lookup"><span data-stu-id="28ccf-110">Designed to be used for migrations ranging from the smallest set of files to a large scale enterprise migration, the SharePoint Migration Tool will allow you to transfer your information to the cloud and take advantage of the newest collaboration, intelligence, and security solutions with Office 365.</span></span>

- [<span data-ttu-id="28ccf-111">Unduh dan instal alat migrasi SharePoint</span><span class="sxs-lookup"><span data-stu-id="28ccf-111">Download and install the SharePoint Migration Tool</span></span>](https://docs.microsoft.com/sharepointmigration/introducing-the-sharepoint-migration-tool)
- [<span data-ttu-id="28ccf-112">Masalah umum SPMT masalah dan galat</span><span class="sxs-lookup"><span data-stu-id="28ccf-112">Troubleshooting common SPMT issues and errors</span></span>](https://docs.microsoft.com/sharepointmigration/troubleshooting-common-spmt-issues)
- [<span data-ttu-id="28ccf-113">Pemecahan masalah instalasi SPMT</span><span class="sxs-lookup"><span data-stu-id="28ccf-113">Troubleshooting SPMT installation issues</span></span>](https://docs.microsoft.com/sharepointmigration/spmt-install-issues#troubleshooting-spmt-installation-issues)
