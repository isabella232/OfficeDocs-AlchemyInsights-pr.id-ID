---
title: Aturan DLP untuk SSN tidak berfungsi
ms.author: deniseb
author: denisebmsft
manager: laurawi
ms.date: 11/5/2018
ms.audience: ITPro
ms.topic: article
ROBOTS: NOINDEX, NOFOLLOW
localization_priority: Normal
ms.custom:
- "1242"
- "3200001"
ms.assetid: ac265ee6-c946-476e-9bf0-0ea0e8adc98a
ms.openlocfilehash: 0b83a858975ffe1bb70f16a7452a13d57dff5340
ms.sourcegitcommit: b0d5b68366028abcf08610672d5bc9d3b25ac433
ms.translationtype: MT
ms.contentlocale: id-ID
ms.lasthandoff: 03/24/2020
ms.locfileid: "42932527"
---
# <a name="dlp-issues-with-social-security-numbers"></a><span data-ttu-id="4f6e2-102">Masalah DLP dengan nomor jaminan sosial</span><span class="sxs-lookup"><span data-stu-id="4f6e2-102">DLP issues with Social Security Numbers</span></span>

<span data-ttu-id="4f6e2-103">**Penting**: banyak SharePoint online dan OneDrive pelanggan menjalankan aplikasi penting bisnis terhadap layanan yang berjalan di latar belakang.</span><span class="sxs-lookup"><span data-stu-id="4f6e2-103">**Important**: Many SharePoint Online and OneDrive customers run business-critical applications against the service that run in the background.</span></span> <span data-ttu-id="4f6e2-104">Ini termasuk migrasi konten, pencegahan kehilangan data (DLP), dan solusi pencadangan.</span><span class="sxs-lookup"><span data-stu-id="4f6e2-104">These include content migration, Data Loss Prevention (DLP), and backup solutions.</span></span> <span data-ttu-id="4f6e2-105">Selama waktu yang belum pernah terjadi sebelumnya, kami mengambil langkah untuk memastikan bahwa SharePoint online dan layanan OneDrive tetap sangat tersedia dan dapat diandalkan untuk pengguna yang bergantung pada layanan lebih dari sebelumnya dalam skenario kerja jarak jauh.</span><span class="sxs-lookup"><span data-stu-id="4f6e2-105">During these unprecedented times, we are taking steps to ensure that SharePoint Online and OneDrive services remain highly available and reliable for your users who depend on the service more than ever in remote work scenarios.</span></span>

<span data-ttu-id="4f6e2-106">Untuk mendukung tujuan ini, kami telah menerapkan batas pelambatan yang lebih ketat pada aplikasi latar belakang (migrasi, DLP dan solusi cadangan) selama jam siang hari kerja.</span><span class="sxs-lookup"><span data-stu-id="4f6e2-106">In support of this objective, we have implemented tighter throttling limits on background apps (migration, DLP and backup solutions) during weekday daytime hours.</span></span> <span data-ttu-id="4f6e2-107">Anda harus mengharapkan bahwa aplikasi ini akan mencapai throughput yang sangat terbatas selama waktu ini.</span><span class="sxs-lookup"><span data-stu-id="4f6e2-107">You should expect that these apps will achieve very limited throughput during these times.</span></span> <span data-ttu-id="4f6e2-108">Namun, selama jam malam dan akhir pekan untuk wilayah ini, Layanan akan siap untuk memproses volume permintaan yang jauh lebih tinggi dari aplikasi latar belakang.</span><span class="sxs-lookup"><span data-stu-id="4f6e2-108">However, during evening and weekend hours for the region, the service will be ready to process a significantly higher volume of requests from background apps.</span></span>

<span data-ttu-id="4f6e2-109">**Masalah DLP dengan SSNs**</span><span class="sxs-lookup"><span data-stu-id="4f6e2-109">**DLP issues with SSNs**</span></span>

<span data-ttu-id="4f6e2-110">Apakah Anda mengalami masalah dengan **pencegahan kehilangan data (DLP)** yang tidak berfungsi untuk konten yang berisi **nomor jaminan sosial (SSN)** saat menggunakan jenis informasi sensitif di Office 365?</span><span class="sxs-lookup"><span data-stu-id="4f6e2-110">Are you having problems with **Data Loss Prevention (DLP)** not working for content containing a **Social Security Number (SSN)** when using a sensitive information type in Office 365?</span></span> <span data-ttu-id="4f6e2-111">Jika demikian, pastikan konten Anda berisi informasi yang diperlukan untuk apa kebijakan DLP Cari.</span><span class="sxs-lookup"><span data-stu-id="4f6e2-111">If so, make sure your content contains the needed information for what the DLP policy is looking.</span></span> 
  
<span data-ttu-id="4f6e2-112">Misalnya, untuk kebijakan SSN yang dikonfigurasi dengan tingkat kepercayaan 85%, berikut dievaluasi dan harus terdeteksi untuk aturan untuk memicu:</span><span class="sxs-lookup"><span data-stu-id="4f6e2-112">For example, for an SSN policy configured with a confidence level of 85%, the following are evaluated and must be detected for the rule to trigger:</span></span>
  
- <span data-ttu-id="4f6e2-113">**[Format:](https://docs.microsoft.com/office365/securitycompliance/what-the-sensitive-information-types-look-for#format-80)** 9 digit, yang mungkin dalam pola diformat atau tidak diformat</span><span class="sxs-lookup"><span data-stu-id="4f6e2-113">**[Format:](https://docs.microsoft.com/office365/securitycompliance/what-the-sensitive-information-types-look-for#format-80)** 9 digits, which may be in a formatted or unformatted pattern</span></span>

- <span data-ttu-id="4f6e2-114">**[Pola:](https://msconnect.microsoft.com/https:/docs.microsoft.com/office365/securitycompliance/what-the-sensitive-information-types-look-for#pattern-80)** Empat fungsi mencari SSNs dalam empat pola yang berbeda:</span><span class="sxs-lookup"><span data-stu-id="4f6e2-114">**[Pattern:](https://msconnect.microsoft.com/https:/docs.microsoft.com/office365/securitycompliance/what-the-sensitive-information-types-look-for#pattern-80)** Four functions look for SSNs in four different patterns:</span></span>

  - <span data-ttu-id="4f6e2-115">Func_ssn menemukan SSNs dengan pra-2011 format yang kuat yang diformat dengan tanda hubung atau spasi (DDD-DD-DDDD atau DDD DD DDDD)</span><span class="sxs-lookup"><span data-stu-id="4f6e2-115">Func_ssn finds SSNs with pre-2011 strong formatting that are formatted with dashes or spaces (ddd-dd-dddd OR ddd dd dddd)</span></span>

  - <span data-ttu-id="4f6e2-116">Func_unformatted_ssn menemukan SSNs dengan pra-2011 format yang kuat yang telah diformat sebagai sembilan digit berturut-turut (ddddddddd)</span><span class="sxs-lookup"><span data-stu-id="4f6e2-116">Func_unformatted_ssn finds SSNs with pre-2011 strong formatting that are unformatted as nine consecutive digits (ddddddddd)</span></span>

  - <span data-ttu-id="4f6e2-117">Func_randomized_formatted_ssn menemukan Post-2011 SSNs yang diformat dengan tanda hubung atau spasi (DDD-DD-DDDD atau DDD DD DDDD)</span><span class="sxs-lookup"><span data-stu-id="4f6e2-117">Func_randomized_formatted_ssn finds post-2011 SSNs that are formatted with dashes or spaces (ddd-dd-dddd OR ddd dd dddd)</span></span>

  - <span data-ttu-id="4f6e2-118">Func_randomized_unformatted_ssn menemukan Post-2011 SSNs yang terformat sebagai sembilan digit berturut-turut (ddddddddd)</span><span class="sxs-lookup"><span data-stu-id="4f6e2-118">Func_randomized_unformatted_ssn finds post-2011 SSNs that are unformatted as nine consecutive digits (ddddddddd)</span></span>

- <span data-ttu-id="4f6e2-119">**[Checksum:](https://docs.microsoft.com/office365/securitycompliance/what-the-sensitive-information-types-look-for#checksum-79)** Tidak, tidak ada checksum</span><span class="sxs-lookup"><span data-stu-id="4f6e2-119">**[Checksum:](https://docs.microsoft.com/office365/securitycompliance/what-the-sensitive-information-types-look-for#checksum-79)** No, there is no Checksum</span></span>

- <span data-ttu-id="4f6e2-120">**[Definisi:](https://docs.microsoft.com/office365/securitycompliance/what-the-sensitive-information-types-look-for#definition-80)** Sebuah kebijakan DLP adalah 85% yakin bahwa hal itu terdeteksi jenis informasi sensitif jika, dalam kedekatan 300 karakter:</span><span class="sxs-lookup"><span data-stu-id="4f6e2-120">**[Definition:](https://docs.microsoft.com/office365/securitycompliance/what-the-sensitive-information-types-look-for#definition-80)** A DLP policy is 85% confident that it's detected this type of sensitive information if, within a proximity of 300 characters:</span></span>

  - <span data-ttu-id="4f6e2-121">[Fungsi Func_ssn](https://docs.microsoft.com/office365/securitycompliance/what-the-sensitive-information-types-look-for#pattern-80) menemukan konten yang sesuai dengan pola.</span><span class="sxs-lookup"><span data-stu-id="4f6e2-121">The [function Func_ssn](https://docs.microsoft.com/office365/securitycompliance/what-the-sensitive-information-types-look-for#pattern-80) finds content that matches the pattern.</span></span>

  - <span data-ttu-id="4f6e2-122">Kata kunci dari [Keyword_ssn](https://docs.microsoft.com/office365/securitycompliance/what-the-sensitive-information-types-look-for#keyword_ssn) ditemukan.</span><span class="sxs-lookup"><span data-stu-id="4f6e2-122">A keyword from [Keyword_ssn](https://docs.microsoft.com/office365/securitycompliance/what-the-sensitive-information-types-look-for#keyword_ssn) is found.</span></span> <span data-ttu-id="4f6e2-123">Contoh kata kunci meliputi: *jaminan sosial, jaminan sosial #, SOC SEC, SSN* .</span><span class="sxs-lookup"><span data-stu-id="4f6e2-123">Examples of keywords includes:  *Social Security, Social Security#, Soc Sec ,SSN*  .</span></span> <span data-ttu-id="4f6e2-124">Sebagai contoh, contoh berikut akan memicu kebijakan DLP SSN: **SSN: 489-36-8350**</span><span class="sxs-lookup"><span data-stu-id="4f6e2-124">For example, the following sample would trigger for the DLP SSN policy: **SSN: 489-36-8350**</span></span>
  
<span data-ttu-id="4f6e2-125">Untuk informasi lebih lanjut tentang apa yang diperlukan untuk SSNs untuk terdeteksi untuk konten Anda, lihat bagian berikut dalam artikel ini: [apa jenis informasi sensitif mencari SSNs](https://docs.microsoft.com/office365/securitycompliance/what-the-sensitive-information-types-look-for#us-social-security-number-ssn)</span><span class="sxs-lookup"><span data-stu-id="4f6e2-125">For more information on what is required for SSNs to be detected for your content, see the following section in this article: [What the Sensitive Information Types look for SSNs](https://docs.microsoft.com/office365/securitycompliance/what-the-sensitive-information-types-look-for#us-social-security-number-ssn)</span></span>
  
<span data-ttu-id="4f6e2-126">Menggunakan jenis informasi sensitif internal yang berbeda, lihat artikel berikut untuk informasi tentang apa yang diperlukan untuk jenis lain: [apa jenis informasi sensitif](https://docs.microsoft.com/office365/securitycompliance/what-the-sensitive-information-types-look-for) mencari</span><span class="sxs-lookup"><span data-stu-id="4f6e2-126">Using a different built-in sensitive information type, see the following article for information on what is required for other types: [What the Sensitive Information Types look for](https://docs.microsoft.com/office365/securitycompliance/what-the-sensitive-information-types-look-for)</span></span>
  