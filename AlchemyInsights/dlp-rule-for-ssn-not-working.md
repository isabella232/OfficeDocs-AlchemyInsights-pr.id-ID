---
title: Aturan DLP untuk SSN tidak berfungsi
ms.author: deniseb
author: denisebmsft
manager: laurawi
ms.date: 04/21/2020
ms.audience: ITPro
ms.topic: article
ms.service: o365-administration
ROBOTS: NOINDEX, NOFOLLOW
localization_priority: Normal
ms.custom:
- "1242"
- "3200001"
ms.assetid: ac265ee6-c946-476e-9bf0-0ea0e8adc98a
ms.openlocfilehash: b221e66862ca01074f380fbb8433f8f9cac044cb
ms.sourcegitcommit: c6692ce0fa1358ec3529e59ca0ecdfdea4cdc759
ms.translationtype: MT
ms.contentlocale: id-ID
ms.lasthandoff: 09/14/2020
ms.locfileid: "47679372"
---
# <a name="dlp-issues-with-social-security-numbers"></a><span data-ttu-id="9e935-102">Masalah DLP dengan nomor jaminan sosial</span><span class="sxs-lookup"><span data-stu-id="9e935-102">DLP issues with Social Security Numbers</span></span>

<span data-ttu-id="9e935-103">**Penting**: Selama masa-masa yang berat ini, kami mengambil langkah untuk memastikan bahwa SharePoint Online dan layanan OneDrive tetap memiliki ketersediaan yang tinggi. Silakan kunjungi [Penyesuaian Fitur Sementara SharePoint Online](https://aka.ms/ODSPAdjustments) untuk informasi selengkapnya.</span><span class="sxs-lookup"><span data-stu-id="9e935-103">**Important**: During these unprecedented times, we are taking steps to ensure that SharePoint Online and OneDrive services remain highly available – Please visit [SharePoint Online Temporary Feature Adjustments](https://aka.ms/ODSPAdjustments) for more information.</span></span>

<span data-ttu-id="9e935-104">**Masalah DLP dengan SSNs**</span><span class="sxs-lookup"><span data-stu-id="9e935-104">**DLP issues with SSNs**</span></span>

<span data-ttu-id="9e935-105">Apakah Anda mengalami masalah dengan **pencegahan kehilangan data (DLP)** tidak berfungsi untuk konten yang berisi **nomor jaminan sosial (SSN)** saat menggunakan tipe informasi sensitif di Microsoft 365?</span><span class="sxs-lookup"><span data-stu-id="9e935-105">Are you having problems with **Data Loss Prevention (DLP)** not working for content containing a **Social Security Number (SSN)** when using a sensitive information type in Microsoft 365?</span></span> <span data-ttu-id="9e935-106">Jika demikian, pastikan konten Anda berisi informasi yang diperlukan untuk apa yang dicari kebijakan DLP.</span><span class="sxs-lookup"><span data-stu-id="9e935-106">If so, make sure your content contains the needed information for what the DLP policy is looking.</span></span> 
  
<span data-ttu-id="9e935-107">Misalnya, untuk kebijakan SSN yang dikonfigurasi dengan tingkat kepercayaan 85%, berikut ini dievaluasi dan harus dideteksi agar aturan dipicu:</span><span class="sxs-lookup"><span data-stu-id="9e935-107">For example, for an SSN policy configured with a confidence level of 85%, the following are evaluated and must be detected for the rule to trigger:</span></span>
  
- <span data-ttu-id="9e935-108">**[Format:](https://docs.microsoft.com/microsoft-365/compliance/sensitive-information-type-entity-definitions#format-80)** 9 digit, yang mungkin dalam pola yang diformat atau tidak diformat</span><span class="sxs-lookup"><span data-stu-id="9e935-108">**[Format:](https://docs.microsoft.com/microsoft-365/compliance/sensitive-information-type-entity-definitions#format-80)** 9 digits, which may be in a formatted or unformatted pattern</span></span>

- <span data-ttu-id="9e935-109">**[Pola:](https://msconnect.microsoft.com/https:/docs.microsoft.com/office365/securitycompliance/what-the-sensitive-information-types-look-for#pattern-80)** Empat fungsi mencari SSNs dalam empat pola yang berbeda:</span><span class="sxs-lookup"><span data-stu-id="9e935-109">**[Pattern:](https://msconnect.microsoft.com/https:/docs.microsoft.com/office365/securitycompliance/what-the-sensitive-information-types-look-for#pattern-80)** Four functions look for SSNs in four different patterns:</span></span>

  - <span data-ttu-id="9e935-110">Func_ssn menemukan SSNs dengan pemformatan pra-2011 kuat yang diformat dengan garis putus-putus atau spasi (DDD-DD-DDDD atau DDD DD DDDD)</span><span class="sxs-lookup"><span data-stu-id="9e935-110">Func_ssn finds SSNs with pre-2011 strong formatting that are formatted with dashes or spaces (ddd-dd-dddd OR ddd dd dddd)</span></span>

  - <span data-ttu-id="9e935-111">Func_unformatted_ssn menemukan SSNs dengan pemformatan pra-2011 yang kuat yang tidak diformat sebagai sembilan digit berturut-turut (ddddddddd)</span><span class="sxs-lookup"><span data-stu-id="9e935-111">Func_unformatted_ssn finds SSNs with pre-2011 strong formatting that are unformatted as nine consecutive digits (ddddddddd)</span></span>

  - <span data-ttu-id="9e935-112">Func_randomized_formatted_ssn menemukan SSNs Post-2011 yang diformat dengan garis putus-putus atau spasi (DDD-DD-DDDD atau DDD DD DDDD)</span><span class="sxs-lookup"><span data-stu-id="9e935-112">Func_randomized_formatted_ssn finds post-2011 SSNs that are formatted with dashes or spaces (ddd-dd-dddd OR ddd dd dddd)</span></span>

  - <span data-ttu-id="9e935-113">Func_randomized_unformatted_ssn menemukan SSNs Post-2011 yang tidak diformat sebagai sembilan digit berturut-turut (ddddddddd)</span><span class="sxs-lookup"><span data-stu-id="9e935-113">Func_randomized_unformatted_ssn finds post-2011 SSNs that are unformatted as nine consecutive digits (ddddddddd)</span></span>

- <span data-ttu-id="9e935-114">**[Checksum:](https://docs.microsoft.com/microsoft-365/compliance/sensitive-information-type-entity-definitions#checksum-79)** Tidak, tidak ada checksum</span><span class="sxs-lookup"><span data-stu-id="9e935-114">**[Checksum:](https://docs.microsoft.com/microsoft-365/compliance/sensitive-information-type-entity-definitions#checksum-79)** No, there is no Checksum</span></span>

- <span data-ttu-id="9e935-115">**[Definisi:](https://docs.microsoft.com/microsoft-365/compliance/sensitive-information-type-entity-definitions#definition-80)** Kebijakan DLP adalah 85% yakin bahwa kebijakan ini mendeteksi tipe informasi sensitif ini jika, dalam kedekatan karakter 300:</span><span class="sxs-lookup"><span data-stu-id="9e935-115">**[Definition:](https://docs.microsoft.com/microsoft-365/compliance/sensitive-information-type-entity-definitions#definition-80)** A DLP policy is 85% confident that it's detected this type of sensitive information if, within a proximity of 300 characters:</span></span>

  - <span data-ttu-id="9e935-116">[Fungsi Func_ssn](https://docs.microsoft.com/microsoft-365/compliance/sensitive-information-type-entity-definitions#pattern-80) menemukan konten yang cocok dengan pola.</span><span class="sxs-lookup"><span data-stu-id="9e935-116">The [function Func_ssn](https://docs.microsoft.com/microsoft-365/compliance/sensitive-information-type-entity-definitions#pattern-80) finds content that matches the pattern.</span></span>

  - <span data-ttu-id="9e935-117">Kata kunci dari [Keyword_ssn](https://docs.microsoft.com/microsoft-365/compliance/sensitive-information-type-entity-definitions#keyword_ssn) ditemukan.</span><span class="sxs-lookup"><span data-stu-id="9e935-117">A keyword from [Keyword_ssn](https://docs.microsoft.com/microsoft-365/compliance/sensitive-information-type-entity-definitions#keyword_ssn) is found.</span></span> <span data-ttu-id="9e935-118">Contoh kata kunci meliputi: Jamsostek  *, Jamsostek #, SOC SEC, SSN*  .</span><span class="sxs-lookup"><span data-stu-id="9e935-118">Examples of keywords includes:  *Social Security, Social Security#, Soc Sec ,SSN*  .</span></span> <span data-ttu-id="9e935-119">Misalnya, contoh berikut ini akan memicu kebijakan SSN DLP: **SSN: 489-36-8350**</span><span class="sxs-lookup"><span data-stu-id="9e935-119">For example, the following sample would trigger for the DLP SSN policy: **SSN: 489-36-8350**</span></span>
  
<span data-ttu-id="9e935-120">Untuk informasi lebih lanjut tentang apa yang diperlukan untuk SSNs yang akan terdeteksi untuk konten Anda, lihat bagian berikut ini di artikel ini: [apa tipe informasi sensitif Cari SSNs](https://docs.microsoft.com/microsoft-365/compliance/sensitive-information-type-entity-definitions#us-social-security-number-ssn)</span><span class="sxs-lookup"><span data-stu-id="9e935-120">For more information on what is required for SSNs to be detected for your content, see the following section in this article: [What the Sensitive Information Types look for SSNs](https://docs.microsoft.com/microsoft-365/compliance/sensitive-information-type-entity-definitions#us-social-security-number-ssn)</span></span>
  
<span data-ttu-id="9e935-121">Menggunakan tipe informasi sensitif bawaan yang berbeda, lihat artikel berikut ini untuk informasi tentang apa yang diperlukan untuk tipe lainnya: [apa yang dicari tipe informasi sensitif](https://docs.microsoft.com/microsoft-365/compliance/sensitive-information-type-entity-definitions)</span><span class="sxs-lookup"><span data-stu-id="9e935-121">Using a different built-in sensitive information type, see the following article for information on what is required for other types: [What the Sensitive Information Types look for](https://docs.microsoft.com/microsoft-365/compliance/sensitive-information-type-entity-definitions)</span></span>
  