---
title: DLP aturan untuk SSN tidak bekerja
ms.author: cmcatee
author: cmcatee-MSFT
manager: mnirkhe
ms.date: 11/5/2018
ms.audience: ITPro
ms.topic: article
ROBOTS: NOINDEX, NOFOLLOW
localization_priority: Normal
ms.assetid: ac265ee6-c946-476e-9bf0-0ea0e8adc98a
ms.openlocfilehash: d2d21fb5546d36990d69b76e3ceb72ce2edf3d80
ms.sourcegitcommit: 9d78905c512192ffc4675468abd2efc5f2e4baf4
ms.translationtype: MT
ms.contentlocale: id-ID
ms.lasthandoff: 04/23/2019
ms.locfileid: "32404420"
---
<span data-ttu-id="c95fc-102">Apakah Anda memiliki masalah dengan **Data Rugi Pencegahan (DLP)** tidak bekerja untuk konten yang berisi **Nomor jaminan sosial (SSN)** ketika menggunakan jenis informasi sensitif di Office 365?</span><span class="sxs-lookup"><span data-stu-id="c95fc-102">Are you having problems with **Data Loss Prevention (DLP)** not working for content containing a **Social Security Number (SSN)** when using a sensitive information type in Office 365?</span></span> <span data-ttu-id="c95fc-103">Jika demikian, pastikan konten Anda berisi informasi yang dibutuhkan untuk apa kebijakan DLP Cari.</span><span class="sxs-lookup"><span data-stu-id="c95fc-103">If so, make sure your content contains the needed information for what the DLP policy is looking.</span></span> 
  
<span data-ttu-id="c95fc-104">Misalnya, untuk kebijakan SSN dikonfigurasi dengan tingkat keyakinan 85%, berikut dievaluasi dan harus terdeteksi untuk aturan untuk memicu:</span><span class="sxs-lookup"><span data-stu-id="c95fc-104">For example, for an SSN policy configured with a confidence level of 85%, the following are evaluated and must be detected for the rule to trigger:</span></span>
  
- <span data-ttu-id="c95fc-105">**[Format:](https://docs.microsoft.com/office365/securitycompliance/what-the-sensitive-information-types-look-for#format-80)** 9 digit, yang mungkin dalam pola diformat atau tidak diformat</span><span class="sxs-lookup"><span data-stu-id="c95fc-105">**[Format:](https://docs.microsoft.com/office365/securitycompliance/what-the-sensitive-information-types-look-for#format-80)** 9 digits, which may be in a formatted or unformatted pattern</span></span> 
    
- <span data-ttu-id="c95fc-106">**[Pola:](https://msconnect.microsoft.com/https:/docs.microsoft.com/office365/securitycompliance/what-the-sensitive-information-types-look-for#pattern-80)** Empat fungsi Cari SSNs dalam empat pola yang berbeda:</span><span class="sxs-lookup"><span data-stu-id="c95fc-106">**[Pattern:](https://msconnect.microsoft.com/https:/docs.microsoft.com/office365/securitycompliance/what-the-sensitive-information-types-look-for#pattern-80)** Four functions look for SSNs in four different patterns:</span></span> 
    
  - <span data-ttu-id="c95fc-107">Func_ssn menemukan SSNs dengan pra-2011 kuat format yang diformat dengan tanda hubung atau ruang (ddd-dd-dddd OR ddd dd dddd)</span><span class="sxs-lookup"><span data-stu-id="c95fc-107">Func_ssn finds SSNs with pre-2011 strong formatting that are formatted with dashes or spaces (ddd-dd-dddd OR ddd dd dddd)</span></span>
    
  - <span data-ttu-id="c95fc-108">Func_unformatted_ssn menemukan SSNs dengan pra-2011 kuat format yang tidak diformat sebagai sembilan angka berturut-turut (ddddddddd)</span><span class="sxs-lookup"><span data-stu-id="c95fc-108">Func_unformatted_ssn finds SSNs with pre-2011 strong formatting that are unformatted as nine consecutive digits (ddddddddd)</span></span>
    
  - <span data-ttu-id="c95fc-109">Func_randomized_formatted_ssn menemukan posting-2011 SSNs yang diformat dengan tanda hubung atau ruang (ddd-dd-dddd OR ddd dd dddd)</span><span class="sxs-lookup"><span data-stu-id="c95fc-109">Func_randomized_formatted_ssn finds post-2011 SSNs that are formatted with dashes or spaces (ddd-dd-dddd OR ddd dd dddd)</span></span>
    
  - <span data-ttu-id="c95fc-110">Func_randomized_unformatted_ssn menemukan posting-2011 SSNs yang tidak diformat sebagai sembilan angka berturut-turut (ddddddddd)</span><span class="sxs-lookup"><span data-stu-id="c95fc-110">Func_randomized_unformatted_ssn finds post-2011 SSNs that are unformatted as nine consecutive digits (ddddddddd)</span></span>
    
- <span data-ttu-id="c95fc-111">**[Checksum:](https://docs.microsoft.com/office365/securitycompliance/what-the-sensitive-information-types-look-for#checksum-79)** Tidak, adalah tidak terdapat Checksum</span><span class="sxs-lookup"><span data-stu-id="c95fc-111">**[Checksum:](https://docs.microsoft.com/office365/securitycompliance/what-the-sensitive-information-types-look-for#checksum-79)** No, there is no Checksum</span></span> 
    
- <span data-ttu-id="c95fc-112">**[Definisi:](https://docs.microsoft.com/office365/securitycompliance/what-the-sensitive-information-types-look-for#definition-80)** Kebijakan DLP adalah 85% yakin bahwa ia telah mendeteksi jenis informasi sensitif jika, dalam jarak 300 karakter:</span><span class="sxs-lookup"><span data-stu-id="c95fc-112">**[Definition:](https://docs.microsoft.com/office365/securitycompliance/what-the-sensitive-information-types-look-for#definition-80)** A DLP policy is 85% confident that it's detected this type of sensitive information if, within a proximity of 300 characters:</span></span> 
    
  - <span data-ttu-id="c95fc-113">[Fungsi Func_ssn](https://docs.microsoft.com/office365/securitycompliance/what-the-sensitive-information-types-look-for#pattern-80) menemukan konten yang cocok dengan pola.</span><span class="sxs-lookup"><span data-stu-id="c95fc-113">The [function Func_ssn](https://docs.microsoft.com/office365/securitycompliance/what-the-sensitive-information-types-look-for#pattern-80) finds content that matches the pattern.</span></span> 
    
  - <span data-ttu-id="c95fc-114">Kata kunci dari [Keyword_ssn](https://docs.microsoft.com/office365/securitycompliance/what-the-sensitive-information-types-look-for#keyword_ssn) ditemukan.</span><span class="sxs-lookup"><span data-stu-id="c95fc-114">A keyword from [Keyword_ssn](https://docs.microsoft.com/office365/securitycompliance/what-the-sensitive-information-types-look-for#keyword_ssn) is found.</span></span> <span data-ttu-id="c95fc-115">Contoh kata kunci mencakup: *jaminan sosial, Jamsostek #, Soc Sec, SSN* .</span><span class="sxs-lookup"><span data-stu-id="c95fc-115">Examples of keywords includes:  *Social Security, Social Security#, Soc Sec ,SSN*  .</span></span> <span data-ttu-id="c95fc-116">Misalnya, contoh berikut akan memicu untuk kebijakan DLP SSN: **SSN: 489-36-8350**</span><span class="sxs-lookup"><span data-stu-id="c95fc-116">For example, the following sample would trigger for the DLP SSN policy: **SSN: 489-36-8350**</span></span>
    
<span data-ttu-id="c95fc-117">Untuk informasi lebih lanjut tentang apa yang diperlukan untuk SSNs untuk dideteksi untuk konten Anda, lihat bagian berikut dalam artikel ini: [Apa the sensitif informasi jenis mencari SSNs](https://docs.microsoft.com/office365/securitycompliance/what-the-sensitive-information-types-look-for#us-social-security-number-ssn)</span><span class="sxs-lookup"><span data-stu-id="c95fc-117">For more information on what is required for SSNs to be detected for your content, see the following section in this article: [What the Sensitive Information Types look for SSNs](https://docs.microsoft.com/office365/securitycompliance/what-the-sensitive-information-types-look-for#us-social-security-number-ssn)</span></span>
  
<span data-ttu-id="c95fc-118">Menggunakan jenis informasi sensitif built-in yang berbeda, lihat artikel berikut untuk informasi apa saja diperlukan untuk jenis lainnya: [apa the sensitif informasi jenis mencari](https://docs.microsoft.com/office365/securitycompliance/what-the-sensitive-information-types-look-for)</span><span class="sxs-lookup"><span data-stu-id="c95fc-118">Using a different built-in sensitive information type, see the following article for information on what is required for other types: [What the Sensitive Information Types look for](https://docs.microsoft.com/office365/securitycompliance/what-the-sensitive-information-types-look-for)</span></span>
  

