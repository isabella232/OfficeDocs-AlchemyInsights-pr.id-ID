---
title: DLP aturan untuk SSN tidak bekerja
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
ms.openlocfilehash: 757136c39700f12f40f839b29277a59b0e436f03
ms.sourcegitcommit: 1d98db8acb9959aba3b5e308a567ade6b62da56c
ms.translationtype: MT
ms.contentlocale: id-ID
ms.lasthandoff: 08/22/2019
ms.locfileid: "36529860"
---
# <a name="dlp-issues-with-social-security-numbers"></a><span data-ttu-id="0bd75-102">DLP masalah dengan nomor jaminan sosial</span><span class="sxs-lookup"><span data-stu-id="0bd75-102">DLP issues with Social Security Numbers</span></span>

<span data-ttu-id="0bd75-103">Apakah Anda memiliki masalah dengan **Data Rugi Pencegahan (DLP)** tidak bekerja untuk konten yang berisi **Nomor jaminan sosial (SSN)** ketika menggunakan jenis informasi sensitif di Office 365?</span><span class="sxs-lookup"><span data-stu-id="0bd75-103">Are you having problems with **Data Loss Prevention (DLP)** not working for content containing a **Social Security Number (SSN)** when using a sensitive information type in Office 365?</span></span> <span data-ttu-id="0bd75-104">Jika demikian, pastikan konten Anda berisi informasi yang dibutuhkan untuk apa kebijakan DLP Cari.</span><span class="sxs-lookup"><span data-stu-id="0bd75-104">If so, make sure your content contains the needed information for what the DLP policy is looking.</span></span> 
  
<span data-ttu-id="0bd75-105">Misalnya, untuk kebijakan SSN dikonfigurasi dengan tingkat keyakinan 85%, berikut dievaluasi dan harus terdeteksi untuk aturan untuk memicu:</span><span class="sxs-lookup"><span data-stu-id="0bd75-105">For example, for an SSN policy configured with a confidence level of 85%, the following are evaluated and must be detected for the rule to trigger:</span></span>
  
- <span data-ttu-id="0bd75-106">**[Format:](https://docs.microsoft.com/office365/securitycompliance/what-the-sensitive-information-types-look-for#format-80)** 9 digit, yang mungkin dalam pola diformat atau tidak diformat</span><span class="sxs-lookup"><span data-stu-id="0bd75-106">**[Format:](https://docs.microsoft.com/office365/securitycompliance/what-the-sensitive-information-types-look-for#format-80)** 9 digits, which may be in a formatted or unformatted pattern</span></span>

- <span data-ttu-id="0bd75-107">**[Pola:](https://msconnect.microsoft.com/https:/docs.microsoft.com/office365/securitycompliance/what-the-sensitive-information-types-look-for#pattern-80)** Empat fungsi Cari SSNs dalam empat pola yang berbeda:</span><span class="sxs-lookup"><span data-stu-id="0bd75-107">**[Pattern:](https://msconnect.microsoft.com/https:/docs.microsoft.com/office365/securitycompliance/what-the-sensitive-information-types-look-for#pattern-80)** Four functions look for SSNs in four different patterns:</span></span>

  - <span data-ttu-id="0bd75-108">Func_ssn menemukan SSNs dengan pra-2011 kuat format yang diformat dengan tanda hubung atau ruang (ddd-dd-dddd OR ddd dd dddd)</span><span class="sxs-lookup"><span data-stu-id="0bd75-108">Func_ssn finds SSNs with pre-2011 strong formatting that are formatted with dashes or spaces (ddd-dd-dddd OR ddd dd dddd)</span></span>

  - <span data-ttu-id="0bd75-109">Func_unformatted_ssn menemukan SSNs dengan pra-2011 kuat format yang tidak diformat sebagai sembilan angka berturut-turut (ddddddddd)</span><span class="sxs-lookup"><span data-stu-id="0bd75-109">Func_unformatted_ssn finds SSNs with pre-2011 strong formatting that are unformatted as nine consecutive digits (ddddddddd)</span></span>

  - <span data-ttu-id="0bd75-110">Func_randomized_formatted_ssn menemukan posting-2011 SSNs yang diformat dengan tanda hubung atau ruang (ddd-dd-dddd OR ddd dd dddd)</span><span class="sxs-lookup"><span data-stu-id="0bd75-110">Func_randomized_formatted_ssn finds post-2011 SSNs that are formatted with dashes or spaces (ddd-dd-dddd OR ddd dd dddd)</span></span>

  - <span data-ttu-id="0bd75-111">Func_randomized_unformatted_ssn menemukan posting-2011 SSNs yang tidak diformat sebagai sembilan angka berturut-turut (ddddddddd)</span><span class="sxs-lookup"><span data-stu-id="0bd75-111">Func_randomized_unformatted_ssn finds post-2011 SSNs that are unformatted as nine consecutive digits (ddddddddd)</span></span>

- <span data-ttu-id="0bd75-112">**[Checksum:](https://docs.microsoft.com/office365/securitycompliance/what-the-sensitive-information-types-look-for#checksum-79)** Tidak, adalah tidak terdapat Checksum</span><span class="sxs-lookup"><span data-stu-id="0bd75-112">**[Checksum:](https://docs.microsoft.com/office365/securitycompliance/what-the-sensitive-information-types-look-for#checksum-79)** No, there is no Checksum</span></span>

- <span data-ttu-id="0bd75-113">**[Definisi:](https://docs.microsoft.com/office365/securitycompliance/what-the-sensitive-information-types-look-for#definition-80)** Kebijakan DLP adalah 85% yakin bahwa ia telah mendeteksi jenis informasi sensitif jika, dalam jarak 300 karakter:</span><span class="sxs-lookup"><span data-stu-id="0bd75-113">**[Definition:](https://docs.microsoft.com/office365/securitycompliance/what-the-sensitive-information-types-look-for#definition-80)** A DLP policy is 85% confident that it's detected this type of sensitive information if, within a proximity of 300 characters:</span></span>

  - <span data-ttu-id="0bd75-114">[Fungsi Func_ssn](https://docs.microsoft.com/office365/securitycompliance/what-the-sensitive-information-types-look-for#pattern-80) menemukan konten yang cocok dengan pola.</span><span class="sxs-lookup"><span data-stu-id="0bd75-114">The [function Func_ssn](https://docs.microsoft.com/office365/securitycompliance/what-the-sensitive-information-types-look-for#pattern-80) finds content that matches the pattern.</span></span>

  - <span data-ttu-id="0bd75-115">Kata kunci dari [Keyword_ssn](https://docs.microsoft.com/office365/securitycompliance/what-the-sensitive-information-types-look-for#keyword_ssn) ditemukan.</span><span class="sxs-lookup"><span data-stu-id="0bd75-115">A keyword from [Keyword_ssn](https://docs.microsoft.com/office365/securitycompliance/what-the-sensitive-information-types-look-for#keyword_ssn) is found.</span></span> <span data-ttu-id="0bd75-116">Contoh kata kunci mencakup: *jaminan sosial, Jamsostek #, Soc Sec, SSN* .</span><span class="sxs-lookup"><span data-stu-id="0bd75-116">Examples of keywords includes:  *Social Security, Social Security#, Soc Sec ,SSN*  .</span></span> <span data-ttu-id="0bd75-117">Misalnya, contoh berikut akan memicu untuk kebijakan DLP SSN: **SSN: 489-36-8350**</span><span class="sxs-lookup"><span data-stu-id="0bd75-117">For example, the following sample would trigger for the DLP SSN policy: **SSN: 489-36-8350**</span></span>
  
<span data-ttu-id="0bd75-118">Untuk informasi lebih lanjut tentang apa yang diperlukan untuk SSNs untuk dideteksi untuk konten Anda, lihat bagian berikut dalam artikel ini: [Apa the sensitif informasi jenis mencari SSNs](https://docs.microsoft.com/office365/securitycompliance/what-the-sensitive-information-types-look-for#us-social-security-number-ssn)</span><span class="sxs-lookup"><span data-stu-id="0bd75-118">For more information on what is required for SSNs to be detected for your content, see the following section in this article: [What the Sensitive Information Types look for SSNs](https://docs.microsoft.com/office365/securitycompliance/what-the-sensitive-information-types-look-for#us-social-security-number-ssn)</span></span>
  
<span data-ttu-id="0bd75-119">Menggunakan jenis informasi sensitif built-in yang berbeda, lihat artikel berikut untuk informasi apa saja diperlukan untuk jenis lainnya: [apa the sensitif informasi jenis mencari](https://docs.microsoft.com/office365/securitycompliance/what-the-sensitive-information-types-look-for)</span><span class="sxs-lookup"><span data-stu-id="0bd75-119">Using a different built-in sensitive information type, see the following article for information on what is required for other types: [What the Sensitive Information Types look for](https://docs.microsoft.com/office365/securitycompliance/what-the-sensitive-information-types-look-for)</span></span>
  