---
title: DLP aturan untuk nomor kartu kredit tidak bekerja
ms.author: cmcatee
author: cmcatee-MSFT
manager: mnirkhe
ms.date: 11/5/2018
ms.audience: ITPro
ms.topic: article
ROBOTS: NOINDEX, NOFOLLOW
localization_priority: Normal
ms.assetid: 30496c79-c8b4-4337-a46d-abed12864209
ms.openlocfilehash: e1d60c493a27efb7f724d57051e21fad5bd0242f
ms.sourcegitcommit: 9d78905c512192ffc4675468abd2efc5f2e4baf4
ms.translationtype: MT
ms.contentlocale: id-ID
ms.lasthandoff: 04/23/2019
ms.locfileid: "32404503"
---
<span data-ttu-id="e051c-102">Apakah Anda memiliki masalah dengan **Data Rugi Pencegahan (DLP)** tidak bekerja untuk konten yang berisi **Nomor kartu kredit** ketika menggunakan jenis informasi sensitif DLP di O365?</span><span class="sxs-lookup"><span data-stu-id="e051c-102">Are you having problems with **Data Loss Prevention (DLP)** not working for content containing a **Credit Card Number** when using a DLP sensitive information type in O365?</span></span> <span data-ttu-id="e051c-103">Jika demikian, pastikan konten Anda berisi informasi yang diperlukan untuk memicu kebijakan DLP ketika itu dievaluasi.</span><span class="sxs-lookup"><span data-stu-id="e051c-103">If so, make sure your content contains the needed information to trigger the the DLP policy when it is evaluated.</span></span> <span data-ttu-id="e051c-104">Misalnya, **kartu kredit kebijakan** dikonfigurasi dengan tingkat keyakinan 85%, berikut dievaluasi dan harus terdeteksi untuk aturan untuk memicu:</span><span class="sxs-lookup"><span data-stu-id="e051c-104">For example, for a **Credit Card policy** configured with a confidence level of 85%, the following are evaluated and must be detected for the rule to trigger:</span></span> 
  
- <span data-ttu-id="e051c-105">**[Format:](https://docs.microsoft.com/office365/securitycompliance/what-the-sensitive-information-types-look-for#format-19)** 16 digit yang dapat diformat atau tidak diformat (dddddddddddddddd) dan harus lulus tes Luhn.</span><span class="sxs-lookup"><span data-stu-id="e051c-105">**[Format:](https://docs.microsoft.com/office365/securitycompliance/what-the-sensitive-information-types-look-for#format-19)** 16 digits which can be formatted or unformatted (dddddddddddddddd) and must pass the Luhn test.</span></span> 
    
- <span data-ttu-id="e051c-106">**[Pola:](https://docs.microsoft.com/office365/securitycompliance/what-the-sensitive-information-types-look-for#pattern-19)** Sangat kompleks dan kuat pola yang mendeteksi kartu dari semua merek utama di seluruh dunia, termasuk Visa, Mastercard, Discover Card, JCB, kartu American Express, kartu hadiah, dan restoran.</span><span class="sxs-lookup"><span data-stu-id="e051c-106">**[Pattern:](https://docs.microsoft.com/office365/securitycompliance/what-the-sensitive-information-types-look-for#pattern-19)** Very complex and robust pattern that detects cards from all major brands worldwide, including Visa, MasterCard, Discover Card, JCB, American Express, gift cards, and diner cards.</span></span> 
    
- <span data-ttu-id="e051c-107">**[Checksum:](https://docs.microsoft.com/office365/securitycompliance/what-the-sensitive-information-types-look-for#checksum-19)** Ya, Luhn checksum</span><span class="sxs-lookup"><span data-stu-id="e051c-107">**[Checksum:](https://docs.microsoft.com/office365/securitycompliance/what-the-sensitive-information-types-look-for#checksum-19)** Yes, the Luhn checksum</span></span> 
    
- <span data-ttu-id="e051c-108">**[Definisi:](https://docs.microsoft.com/office365/securitycompliance/what-the-sensitive-information-types-look-for#definition-19)** Kebijakan DLP adalah 85% yakin bahwa ia telah mendeteksi jenis informasi sensitif jika, dalam jarak 300 karakter:</span><span class="sxs-lookup"><span data-stu-id="e051c-108">**[Definition:](https://docs.microsoft.com/office365/securitycompliance/what-the-sensitive-information-types-look-for#definition-19)** A DLP policy is 85% confident that it's detected this type of sensitive information if, within a proximity of 300 characters:</span></span> 
    
  - <span data-ttu-id="e051c-109">Fungsi Func_credit_card menemukan konten yang cocok dengan pola.</span><span class="sxs-lookup"><span data-stu-id="e051c-109">The function Func_credit_card finds content that matches the pattern.</span></span>
    
  - <span data-ttu-id="e051c-110">Salah satu dari berikut ini benar:</span><span class="sxs-lookup"><span data-stu-id="e051c-110">One of the following is true:</span></span> 
    
  - <span data-ttu-id="e051c-111">Kata kunci dari Keyword_cc_verification ditemukan.</span><span class="sxs-lookup"><span data-stu-id="e051c-111">A keyword from Keyword_cc_verification is found.</span></span>
    
  - <span data-ttu-id="e051c-112">Kata kunci dari Keyword_cc_name ditemukan</span><span class="sxs-lookup"><span data-stu-id="e051c-112">A keyword from Keyword_cc_name is found</span></span>
    
  - <span data-ttu-id="e051c-113">Fungsi Func_expiration_date menemukan tanggal dalam format tanggal yang tepat.</span><span class="sxs-lookup"><span data-stu-id="e051c-113">The function Func_expiration_date finds a date in the right date format.</span></span>
    
  - <span data-ttu-id="e051c-114">Checksum melewati</span><span class="sxs-lookup"><span data-stu-id="e051c-114">The checksum passes</span></span>
    
    <span data-ttu-id="e051c-115">Misalnya, contoh berikut akan memicu DLP kartu kredit nomor kebijakan:</span><span class="sxs-lookup"><span data-stu-id="e051c-115">For example, the following sample would trigger for a DLP Credit Card Number Policy:</span></span>
    
  - <span data-ttu-id="e051c-116">Visa: 4485 3647 3952 7352</span><span class="sxs-lookup"><span data-stu-id="e051c-116">Visa: 4485 3647 3952 7352</span></span> 
    
  - <span data-ttu-id="e051c-117">Berakhir: 2/2009</span><span class="sxs-lookup"><span data-stu-id="e051c-117">Expires: 2/2009</span></span>
    
<span data-ttu-id="e051c-118">Untuk informasi lebih lanjut tentang apa saja diperlukan untuk **Nomor kartu kredit** untuk terdeteksi untuk konten Anda, lihat bagian berikut dalam artikel ini: [Apa the sensitif informasi jenis mencari kartu kredit #](https://docs.microsoft.com/office365/securitycompliance/what-the-sensitive-information-types-look-for#credit-card-number)</span><span class="sxs-lookup"><span data-stu-id="e051c-118">For more information on what is required for a **Credit Card Number** to be detected for your content, see the following section in this article: [What the Sensitive Information Types look for Credit Card#](https://docs.microsoft.com/office365/securitycompliance/what-the-sensitive-information-types-look-for#credit-card-number)</span></span>
  
<span data-ttu-id="e051c-119">Menggunakan jenis informasi sensitif built-in yang berbeda, lihat artikel berikut untuk informasi apa saja diperlukan untuk jenis lainnya: [apa the sensitif informasi jenis mencari](https://docs.microsoft.com/office365/securitycompliance/what-the-sensitive-information-types-look-for)</span><span class="sxs-lookup"><span data-stu-id="e051c-119">Using a different built-in sensitive information type, see the following article for information on what is required for other types: [What the Sensitive Information Types look for](https://docs.microsoft.com/office365/securitycompliance/what-the-sensitive-information-types-look-for)</span></span>
  

