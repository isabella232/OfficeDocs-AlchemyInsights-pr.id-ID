---
title: DLP tidak bekerja seperti yang diharapkan
ms.author: deniseb
author: denisebmsft
manager: laurawi
ms.date: 1/9/2019
ms.audience: ITPro
ms.topic: article
ms.prod: office-online-server
ROBOTS: NOINDEX, NOFOLLOW
localization_priority: Normal
ms.custom:
- "1241"
- "3200001"
ms.assetid: f6fcf5ad-55a1-4f25-af27-1f7c1ce06409
ms.openlocfilehash: a56e18ddadef3a2f9056978b8542c1dba8f29665
ms.sourcegitcommit: b0d5b68366028abcf08610672d5bc9d3b25ac433
ms.translationtype: MT
ms.contentlocale: id-ID
ms.lasthandoff: 03/24/2020
ms.locfileid: "42932625"
---
# <a name="dlp-not-working-as-expected"></a><span data-ttu-id="7afeb-102">DLP tidak bekerja seperti yang diharapkan</span><span class="sxs-lookup"><span data-stu-id="7afeb-102">DLP not working as expected</span></span>

<span data-ttu-id="7afeb-103">**Penting**: banyak SharePoint online dan OneDrive pelanggan menjalankan aplikasi penting bisnis terhadap layanan yang berjalan di latar belakang.</span><span class="sxs-lookup"><span data-stu-id="7afeb-103">**Important**: Many SharePoint Online and OneDrive customers run business-critical applications against the service that run in the background.</span></span> <span data-ttu-id="7afeb-104">Ini termasuk migrasi konten, pencegahan kehilangan data (DLP), dan solusi pencadangan.</span><span class="sxs-lookup"><span data-stu-id="7afeb-104">These include content migration, Data Loss Prevention (DLP), and backup solutions.</span></span> <span data-ttu-id="7afeb-105">Selama waktu yang belum pernah terjadi sebelumnya, kami mengambil langkah untuk memastikan bahwa SharePoint online dan layanan OneDrive tetap sangat tersedia dan dapat diandalkan untuk pengguna yang bergantung pada layanan lebih dari sebelumnya dalam skenario kerja jarak jauh.</span><span class="sxs-lookup"><span data-stu-id="7afeb-105">During these unprecedented times, we are taking steps to ensure that SharePoint Online and OneDrive services remain highly available and reliable for your users who depend on the service more than ever in remote work scenarios.</span></span>

<span data-ttu-id="7afeb-106">Untuk mendukung tujuan ini, kami telah menerapkan batas pelambatan yang lebih ketat pada aplikasi latar belakang (migrasi, DLP dan solusi cadangan) selama jam siang hari kerja.</span><span class="sxs-lookup"><span data-stu-id="7afeb-106">In support of this objective, we have implemented tighter throttling limits on background apps (migration, DLP and backup solutions) during weekday daytime hours.</span></span> <span data-ttu-id="7afeb-107">Anda harus mengharapkan bahwa aplikasi ini akan mencapai throughput yang sangat terbatas selama waktu ini.</span><span class="sxs-lookup"><span data-stu-id="7afeb-107">You should expect that these apps will achieve very limited throughput during these times.</span></span> <span data-ttu-id="7afeb-108">Namun, selama jam malam dan akhir pekan untuk wilayah ini, Layanan akan siap untuk memproses volume permintaan yang jauh lebih tinggi dari aplikasi latar belakang.</span><span class="sxs-lookup"><span data-stu-id="7afeb-108">However, during evening and weekend hours for the region, the service will be ready to process a significantly higher volume of requests from background apps.</span></span>

 <span data-ttu-id="7afeb-109">**Menyiapkan DLP**</span><span class="sxs-lookup"><span data-stu-id="7afeb-109">**Setting up DLP**</span></span>

<span data-ttu-id="7afeb-110">Apakah Anda mengalami masalah dengan **pencegahan kehilangan data (DLP)** di Office 365 tidak bekerja seperti yang diharapkan?</span><span class="sxs-lookup"><span data-stu-id="7afeb-110">Are you having problems with **Data Loss Prevention (DLP)** in Office 365 not working as expected?</span></span> <span data-ttu-id="7afeb-111">Jika demikian, pastikan bahwa Anda **DLP kebijakan** diatur dengan benar, dan bahwa data Anda berisi apa **kebijakan DLP** sedang mencari ketika sedang dievaluasi.</span><span class="sxs-lookup"><span data-stu-id="7afeb-111">If so, make sure that your **DLP policy** is set up correctly, and that your data contains what the **DLP policy** is looking for when it is being evaluated.</span></span>
  
<span data-ttu-id="7afeb-112">Kebijakan DLP memungkinkan Anda mengidentifikasi dan melindungi informasi sensitif di organisasi Anda.</span><span class="sxs-lookup"><span data-stu-id="7afeb-112">DLP policies allows you to identify and protect sensitive information in your organization.</span></span> <span data-ttu-id="7afeb-113">Untuk setup DLP kebijakan, gunakan informasi [di sini](https://docs.microsoft.com/office365/securitycompliance/prevent-data-loss#set-up-dlp).</span><span class="sxs-lookup"><span data-stu-id="7afeb-113">To setup DLP policies, use the information [here](https://docs.microsoft.com/office365/securitycompliance/prevent-data-loss#set-up-dlp).</span></span>
  
 <span data-ttu-id="7afeb-114">**Apa yang dicari oleh kebijakan DLP**</span><span class="sxs-lookup"><span data-stu-id="7afeb-114">**What DLP policies look for**</span></span>
  
<span data-ttu-id="7afeb-115">Saat menggunakan **jenis informasi sensitif internal** di pusat keamanan dan kepatuhan Office 365, kebijakan DLP mencari pola dan elemen tertentu saat mendeteksi jenis sensitif ini.</span><span class="sxs-lookup"><span data-stu-id="7afeb-115">When using the **built-in sensitive information types** in Office 365 Security and Compliance center, DLP policies look for specific patterns and elements when detecting these sensitive types.</span></span>
  
- <span data-ttu-id="7afeb-116">**Jenis informasi sensitif internal**</span><span class="sxs-lookup"><span data-stu-id="7afeb-116">**Built-in Sensitive Information Types**</span></span>

    <span data-ttu-id="7afeb-117">Untuk informasi tentang jenis sensitif internal dan apa yang dicari oleh kebijakan DLP saat mendeteksi jenis sensitif, lihat: [apa jenis informasi sensitif Cari](https://docs.microsoft.com/office365/securitycompliance/what-the-sensitive-information-types-look-for).</span><span class="sxs-lookup"><span data-stu-id="7afeb-117">For information on the built-in Sensitive types and what a DLP policy looks for when detecting the Sensitive type, see: [What the sensitive information types look for](https://docs.microsoft.com/office365/securitycompliance/what-the-sensitive-information-types-look-for).</span></span>

- <span data-ttu-id="7afeb-118">**Jenis informasi sensitif khusus**</span><span class="sxs-lookup"><span data-stu-id="7afeb-118">**Custom Sensitive Information Types**</span></span>

    <span data-ttu-id="7afeb-119">Jika Anda mencoba untuk membuat jenis informasi sensitif kustom, gunakan artikel berikut ini untuk informasi tentang cara membuat jenis sensitif kustom: [membuat jenis informasi sensitif kustom](https://docs.microsoft.com/office365/securitycompliance/create-a-custom-sensitive-information-type).</span><span class="sxs-lookup"><span data-stu-id="7afeb-119">If you are trying to create custom sensitive information types, use the following article for information on how to create a custom sensitive type: [Create a custom sensitive information type](https://docs.microsoft.com/office365/securitycompliance/create-a-custom-sensitive-information-type).</span></span>

<span data-ttu-id="7afeb-120">**Menguji kebijakan DLP**</span><span class="sxs-lookup"><span data-stu-id="7afeb-120">**Test a DLP policy**</span></span>

<span data-ttu-id="7afeb-121">Untuk menguji data Anda dengan jenis informasi sensitif internal atau kustom, gunakan opsi **jenis uji** di bawah **klasifikasi** > **jenis Info sensitif**.</span><span class="sxs-lookup"><span data-stu-id="7afeb-121">To test your data with a built-in or custom sensitive information type, use the **Test type** option under **Classifications** > **Sensitive info types**.</span></span> <span data-ttu-id="7afeb-122">Untuk informasi selengkapnya, lihat [menguji jenis informasi sensitif kustom](https://docs.microsoft.com/office365/securitycompliance/create-a-custom-sensitive-information-type#test-custom-sensitive-information-types-in-the-security--compliance-center).</span><span class="sxs-lookup"><span data-stu-id="7afeb-122">For more information, see [Test custom sensitive information types](https://docs.microsoft.com/office365/securitycompliance/create-a-custom-sensitive-information-type#test-custom-sensitive-information-types-in-the-security--compliance-center).</span></span>

 <span data-ttu-id="7afeb-123">**Laporan**</span><span class="sxs-lookup"><span data-stu-id="7afeb-123">**Reports**</span></span>
  
- <span data-ttu-id="7afeb-124">Dapatkan wawasan data sensitif dengan [laporan DLP.](https://docs.microsoft.com/office365/securitycompliance/data-loss-prevention-policies#dlp-reports)</span><span class="sxs-lookup"><span data-stu-id="7afeb-124">Get sensitive data insights with [DLP Reports.](https://docs.microsoft.com/office365/securitycompliance/data-loss-prevention-policies#dlp-reports)</span></span>

- <span data-ttu-id="7afeb-125">Lihat detail spesifik acara dengan [laporan insiden](https://docs.microsoft.com/office365/securitycompliance/data-loss-prevention-policies#incident-reports).</span><span class="sxs-lookup"><span data-stu-id="7afeb-125">See specific details of the event with an [Incident Report](https://docs.microsoft.com/office365/securitycompliance/data-loss-prevention-policies#incident-reports).</span></span>
