---
title: Aturan DLP untuk nomor kartu kredit tidak berfungsi
ms.author: deniseb
author: denisebmsft
manager: laurawi
ms.date: 11/5/2018
ms.audience: ITPro
ms.topic: article
ROBOTS: NOINDEX, NOFOLLOW
localization_priority: Normal
ms.custom:
- "1270"
- "3200001"
ms.assetid: 30496c79-c8b4-4337-a46d-abed12864209
ms.openlocfilehash: 6b28534d072c024a98a9b05f6cb55bfdc3435db6
ms.sourcegitcommit: b0d5b68366028abcf08610672d5bc9d3b25ac433
ms.translationtype: MT
ms.contentlocale: id-ID
ms.lasthandoff: 03/24/2020
ms.locfileid: "42932446"
---
# <a name="dlp-issues-with-credit-card-numbers"></a><span data-ttu-id="f6285-102">Masalah DLP dengan nomor kartu kredit</span><span class="sxs-lookup"><span data-stu-id="f6285-102">DLP issues with credit card numbers</span></span>

<span data-ttu-id="f6285-103">**Penting**: banyak SharePoint online dan OneDrive pelanggan menjalankan aplikasi penting bisnis terhadap layanan yang berjalan di latar belakang.</span><span class="sxs-lookup"><span data-stu-id="f6285-103">**Important**: Many SharePoint Online and OneDrive customers run business-critical applications against the service that run in the background.</span></span> <span data-ttu-id="f6285-104">Ini termasuk migrasi konten, pencegahan kehilangan data (DLP), dan solusi pencadangan.</span><span class="sxs-lookup"><span data-stu-id="f6285-104">These include content migration, Data Loss Prevention (DLP), and backup solutions.</span></span> <span data-ttu-id="f6285-105">Selama waktu yang belum pernah terjadi sebelumnya, kami mengambil langkah untuk memastikan bahwa SharePoint online dan layanan OneDrive tetap sangat tersedia dan dapat diandalkan untuk pengguna yang bergantung pada layanan lebih dari sebelumnya dalam skenario kerja jarak jauh.</span><span class="sxs-lookup"><span data-stu-id="f6285-105">During these unprecedented times, we are taking steps to ensure that SharePoint Online and OneDrive services remain highly available and reliable for your users who depend on the service more than ever in remote work scenarios.</span></span>

<span data-ttu-id="f6285-106">Untuk mendukung tujuan ini, kami telah menerapkan batas pelambatan yang lebih ketat pada aplikasi latar belakang (migrasi, DLP dan solusi cadangan) selama jam siang hari kerja.</span><span class="sxs-lookup"><span data-stu-id="f6285-106">In support of this objective, we have implemented tighter throttling limits on background apps (migration, DLP and backup solutions) during weekday daytime hours.</span></span> <span data-ttu-id="f6285-107">Anda harus mengharapkan bahwa aplikasi ini akan mencapai throughput yang sangat terbatas selama waktu ini.</span><span class="sxs-lookup"><span data-stu-id="f6285-107">You should expect that these apps will achieve very limited throughput during these times.</span></span> <span data-ttu-id="f6285-108">Namun, selama jam malam dan akhir pekan untuk wilayah ini, Layanan akan siap untuk memproses volume permintaan yang jauh lebih tinggi dari aplikasi latar belakang.</span><span class="sxs-lookup"><span data-stu-id="f6285-108">However, during evening and weekend hours for the region, the service will be ready to process a significantly higher volume of requests from background apps.</span></span>

<span data-ttu-id="f6285-109">**Masalah DLP dengan nomor kartu kredit**</span><span class="sxs-lookup"><span data-stu-id="f6285-109">**DLP issues with credit card numbers**</span></span>

<span data-ttu-id="f6285-110">Apakah Anda mengalami masalah dengan **pencegahan kehilangan data (DLP)** tidak bekerja untuk konten yang berisi **nomor kartu kredit** saat menggunakan jenis informasi sensitif DLP di O365?</span><span class="sxs-lookup"><span data-stu-id="f6285-110">Are you having problems with **Data Loss Prevention (DLP)** not working for content containing a **Credit Card Number** when using a DLP sensitive information type in O365?</span></span> <span data-ttu-id="f6285-111">Jika demikian, pastikan konten Anda berisi informasi yang diperlukan untuk memicu kebijakan DLP ketika dievaluasi.</span><span class="sxs-lookup"><span data-stu-id="f6285-111">If so, make sure your content contains the needed information to trigger the the DLP policy when it is evaluated.</span></span> <span data-ttu-id="f6285-112">Misalnya, untuk **kebijakan kartu kredit** yang dikonfigurasi dengan tingkat kepercayaan 85%, berikut dievaluasi dan harus terdeteksi untuk aturan untuk memicu:</span><span class="sxs-lookup"><span data-stu-id="f6285-112">For example, for a **Credit Card policy** configured with a confidence level of 85%, the following are evaluated and must be detected for the rule to trigger:</span></span>
  
- <span data-ttu-id="f6285-113">**[Format:](https://docs.microsoft.com/office365/securitycompliance/what-the-sensitive-information-types-look-for#format-19)** 16 digit yang dapat diformat atau belum diformat (dddddddddddddddd) dan harus lulus tes Luhn.</span><span class="sxs-lookup"><span data-stu-id="f6285-113">**[Format:](https://docs.microsoft.com/office365/securitycompliance/what-the-sensitive-information-types-look-for#format-19)** 16 digits which can be formatted or unformatted (dddddddddddddddd) and must pass the Luhn test.</span></span>

- <span data-ttu-id="f6285-114">**[Pola:](https://docs.microsoft.com/office365/securitycompliance/what-the-sensitive-information-types-look-for#pattern-19)** Pola yang sangat kompleks dan kuat yang mendeteksi kartu dari semua merek utama di seluruh dunia, termasuk Visa, MasterCard, Discover Card, JCB, American Express, kartu hadiah, dan kartu restoran.</span><span class="sxs-lookup"><span data-stu-id="f6285-114">**[Pattern:](https://docs.microsoft.com/office365/securitycompliance/what-the-sensitive-information-types-look-for#pattern-19)** Very complex and robust pattern that detects cards from all major brands worldwide, including Visa, MasterCard, Discover Card, JCB, American Express, gift cards, and diner cards.</span></span>

- <span data-ttu-id="f6285-115">**[Checksum:](https://docs.microsoft.com/office365/securitycompliance/what-the-sensitive-information-types-look-for#checksum-19)** Ya, checksum Luhn</span><span class="sxs-lookup"><span data-stu-id="f6285-115">**[Checksum:](https://docs.microsoft.com/office365/securitycompliance/what-the-sensitive-information-types-look-for#checksum-19)** Yes, the Luhn checksum</span></span>

- <span data-ttu-id="f6285-116">**[Definisi:](https://docs.microsoft.com/office365/securitycompliance/what-the-sensitive-information-types-look-for#definition-19)** Sebuah kebijakan DLP adalah 85% yakin bahwa hal itu terdeteksi jenis informasi sensitif jika, dalam kedekatan 300 karakter:</span><span class="sxs-lookup"><span data-stu-id="f6285-116">**[Definition:](https://docs.microsoft.com/office365/securitycompliance/what-the-sensitive-information-types-look-for#definition-19)** A DLP policy is 85% confident that it's detected this type of sensitive information if, within a proximity of 300 characters:</span></span>

  - <span data-ttu-id="f6285-117">Fungsi Func_credit_card menemukan konten yang sesuai dengan pola.</span><span class="sxs-lookup"><span data-stu-id="f6285-117">The function Func_credit_card finds content that matches the pattern.</span></span>

  - <span data-ttu-id="f6285-118">Salah satu dari berikut ini benar:</span><span class="sxs-lookup"><span data-stu-id="f6285-118">One of the following is true:</span></span>

  - <span data-ttu-id="f6285-119">Kata kunci dari Keyword_cc_verification ditemukan.</span><span class="sxs-lookup"><span data-stu-id="f6285-119">A keyword from Keyword_cc_verification is found.</span></span>

  - <span data-ttu-id="f6285-120">Kata kunci dari Keyword_cc_name ditemukan</span><span class="sxs-lookup"><span data-stu-id="f6285-120">A keyword from Keyword_cc_name is found</span></span>

  - <span data-ttu-id="f6285-121">Fungsi Func_expiration_date menemukan tanggal dalam format tanggal yang tepat.</span><span class="sxs-lookup"><span data-stu-id="f6285-121">The function Func_expiration_date finds a date in the right date format.</span></span>

  - <span data-ttu-id="f6285-122">Checksum lolos</span><span class="sxs-lookup"><span data-stu-id="f6285-122">The checksum passes</span></span>

    <span data-ttu-id="f6285-123">Sebagai contoh, contoh berikut akan memicu untuk kebijakan nomor kartu kredit DLP:</span><span class="sxs-lookup"><span data-stu-id="f6285-123">For example, the following sample would trigger for a DLP Credit Card Number Policy:</span></span>

  - <span data-ttu-id="f6285-124">Visa: 4485 3647 3952 7352</span><span class="sxs-lookup"><span data-stu-id="f6285-124">Visa: 4485 3647 3952 7352</span></span>
  
  - <span data-ttu-id="f6285-125">Berakhir: 2/2009</span><span class="sxs-lookup"><span data-stu-id="f6285-125">Expires: 2/2009</span></span>

<span data-ttu-id="f6285-126">Untuk informasi lebih lanjut tentang apa yang diperlukan untuk **nomor kartu kredit** akan terdeteksi untuk konten Anda, lihat bagian berikut dalam artikel ini: [apa jenis informasi sensitif mencari kartu kredit #](https://docs.microsoft.com/office365/securitycompliance/what-the-sensitive-information-types-look-for#credit-card-number)</span><span class="sxs-lookup"><span data-stu-id="f6285-126">For more information on what is required for a **Credit Card Number** to be detected for your content, see the following section in this article: [What the Sensitive Information Types look for Credit Card#](https://docs.microsoft.com/office365/securitycompliance/what-the-sensitive-information-types-look-for#credit-card-number)</span></span>
  
<span data-ttu-id="f6285-127">Menggunakan jenis informasi sensitif internal yang berbeda, lihat artikel berikut untuk informasi tentang apa yang diperlukan untuk jenis lain: [apa jenis informasi sensitif](https://docs.microsoft.com/office365/securitycompliance/what-the-sensitive-information-types-look-for) mencari</span><span class="sxs-lookup"><span data-stu-id="f6285-127">Using a different built-in sensitive information type, see the following article for information on what is required for other types: [What the Sensitive Information Types look for](https://docs.microsoft.com/office365/securitycompliance/what-the-sensitive-information-types-look-for)</span></span>
  