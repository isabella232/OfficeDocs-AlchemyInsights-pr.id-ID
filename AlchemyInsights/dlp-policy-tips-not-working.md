---
title: Tips DLP kebijakan tidak bekerja
ms.author: deniseb
author: denisebmsft
manager: laurawims
ms.date: 11/7/2018
ms.audience: ITPro
ms.topic: article
ROBOTS: NOINDEX, NOFOLLOW
localization_priority: Normal
ms.assetid: c03d30be-474a-4a34-b3c0-240eb2a2c466
ms.custom:
- "1428"
- "3200001"
ms.openlocfilehash: 51b4472fa721443192eb542cac45965df67634df
ms.sourcegitcommit: b0d5b68366028abcf08610672d5bc9d3b25ac433
ms.translationtype: MT
ms.contentlocale: id-ID
ms.lasthandoff: 03/24/2020
ms.locfileid: "42932589"
---
# <a name="dlp-policy-tip-issues"></a><span data-ttu-id="57e45-102">Masalah DLP kebijakan Tips</span><span class="sxs-lookup"><span data-stu-id="57e45-102">DLP Policy Tip issues</span></span>

<span data-ttu-id="57e45-103">**Penting**: banyak SharePoint online dan OneDrive pelanggan menjalankan aplikasi penting bisnis terhadap layanan yang berjalan di latar belakang.</span><span class="sxs-lookup"><span data-stu-id="57e45-103">**Important**: Many SharePoint Online and OneDrive customers run business-critical applications against the service that run in the background.</span></span> <span data-ttu-id="57e45-104">Ini termasuk migrasi konten, pencegahan kehilangan data (DLP), dan solusi pencadangan.</span><span class="sxs-lookup"><span data-stu-id="57e45-104">These include content migration, Data Loss Prevention (DLP), and backup solutions.</span></span> <span data-ttu-id="57e45-105">Selama waktu yang belum pernah terjadi sebelumnya, kami mengambil langkah untuk memastikan bahwa SharePoint online dan layanan OneDrive tetap sangat tersedia dan dapat diandalkan untuk pengguna yang bergantung pada layanan lebih dari sebelumnya dalam skenario kerja jarak jauh.</span><span class="sxs-lookup"><span data-stu-id="57e45-105">During these unprecedented times, we are taking steps to ensure that SharePoint Online and OneDrive services remain highly available and reliable for your users who depend on the service more than ever in remote work scenarios.</span></span>

<span data-ttu-id="57e45-106">Untuk mendukung tujuan ini, kami telah menerapkan batas pelambatan yang lebih ketat pada aplikasi latar belakang (migrasi, DLP dan solusi cadangan) selama jam siang hari kerja.</span><span class="sxs-lookup"><span data-stu-id="57e45-106">In support of this objective, we have implemented tighter throttling limits on background apps (migration, DLP and backup solutions) during weekday daytime hours.</span></span> <span data-ttu-id="57e45-107">Anda harus mengharapkan bahwa aplikasi ini akan mencapai throughput yang sangat terbatas selama waktu ini.</span><span class="sxs-lookup"><span data-stu-id="57e45-107">You should expect that these apps will achieve very limited throughput during these times.</span></span> <span data-ttu-id="57e45-108">Namun, selama jam malam dan akhir pekan untuk wilayah ini, Layanan akan siap untuk memproses volume permintaan yang jauh lebih tinggi dari aplikasi latar belakang.</span><span class="sxs-lookup"><span data-stu-id="57e45-108">However, during evening and weekend hours for the region, the service will be ready to process a significantly higher volume of requests from background apps.</span></span>

<span data-ttu-id="57e45-109">**Tips kebijakan DLP**</span><span class="sxs-lookup"><span data-stu-id="57e45-109">**DLP policy tips**</span></span>

<span data-ttu-id="57e45-110">Saat menggunakan **kebijakan DLP**, pengguna dapat diberitahu tentang pelanggaran kebijakan dengan **Tips kebijakan**.</span><span class="sxs-lookup"><span data-stu-id="57e45-110">When using **DLP policies**, users can be notified of a policy violation with **policy tips**.</span></span> <span data-ttu-id="57e45-111">Admin dapat mengkonfigurasi kebijakan Tips untuk menampilkan saat pengujian kebijakan DLP mereka atau ketika kebijakan dalam mode penegakan penuh.</span><span class="sxs-lookup"><span data-stu-id="57e45-111">Admins can configure policy tips to display while testing their DLP policy or when the policy is in full enforcement mode.</span></span>
  
<span data-ttu-id="57e45-112">Untuk mengkonfigurasi Tips kebijakan DLP kebijakan di pusat keamanan dan kepatuhan dalam mode penegakan penuh, lakukan hal berikut:</span><span class="sxs-lookup"><span data-stu-id="57e45-112">To configure policy tips on your DLP policy in the Security and Compliance center in full enforcement mode, do the following:</span></span>
  
- <span data-ttu-id="57e45-113">Pastikan kiat kebijakan telah **diaktifkan** pada aturan DLP dengan menggunakan langkah [di sini](https://docs.microsoft.com/office365/securitycompliance/use-notifications-and-policy-tips).</span><span class="sxs-lookup"><span data-stu-id="57e45-113">Ensure policy tips have been **enabled** on the DLP rule using the steps [here](https://docs.microsoft.com/office365/securitycompliance/use-notifications-and-policy-tips).</span></span>

- <span data-ttu-id="57e45-114">Pastikan **konten Anda sesuai** dengan apa yang **diperlukan** untuk memicu aturan yang diuraikan dalam artikel ini di [sini](https://docs.microsoft.com/office365/securitycompliance/what-the-sensitive-information-types-look-for).</span><span class="sxs-lookup"><span data-stu-id="57e45-114">Ensure your **content matches** what is **required** to trigger the rule outlined in this article [here](https://docs.microsoft.com/office365/securitycompliance/what-the-sensitive-information-types-look-for).</span></span>

- <span data-ttu-id="57e45-115">Tips kebijakan ditampilkan di OWA dan Outlook.</span><span class="sxs-lookup"><span data-stu-id="57e45-115">Policy tips display in both OWA and Outlook.</span></span> <span data-ttu-id="57e45-116">Namun, saat menggunakan **Outlook 2013 atau yang lebih baru**, Tips kebijakan hanya ditampilkan di bawah kondisi tertentu.</span><span class="sxs-lookup"><span data-stu-id="57e45-116">However, when using **Outlook 2013 or later**, policy tips are only displayed under certain conditions.</span></span> <span data-ttu-id="57e45-117">Kondisi ini tercantum di sini: [kondisi yang didukung untuk Outlook 2013 atau yang lebih baru untuk menampilkan Tips kebijakan](https://docs.microsoft.com/office365/securitycompliance/use-notifications-and-policy-tips#outlook-2013-and-later-supports-showing-policy-tips-for-only-some-conditions)</span><span class="sxs-lookup"><span data-stu-id="57e45-117">These conditions are listed here: [Supported conditions for Outlook 2013 or later for displaying Policy Tips](https://docs.microsoft.com/office365/securitycompliance/use-notifications-and-policy-tips#outlook-2013-and-later-supports-showing-policy-tips-for-only-some-conditions)</span></span>

<span data-ttu-id="57e45-118">Untuk informasi tambahan tentang Tips DLP kebijakan, lihat: [Tampilkan Tips kebijakan DLP kebijakan](https://docs.microsoft.com/office365/securitycompliance/use-notifications-and-policy-tips)</span><span class="sxs-lookup"><span data-stu-id="57e45-118">For additional information on DLP policy tips, see: [Show policy tips for DLP Policies](https://docs.microsoft.com/office365/securitycompliance/use-notifications-and-policy-tips)</span></span>
  