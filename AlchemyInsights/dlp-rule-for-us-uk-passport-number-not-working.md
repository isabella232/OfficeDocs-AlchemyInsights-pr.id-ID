---
title: DLP aturan untuk US / nomor paspor Inggris tidak bekerja
ms.author: cmcatee
author: cmcatee-MSFT
manager: mnirkhe
ms.date: 11/5/2018
ms.audience: ITPro
ms.topic: article
ROBOTS: NOINDEX, NOFOLLOW
localization_priority: Normal
ms.assetid: fc178b8b-943b-4346-a2bd-a75c6af6f80f
ms.openlocfilehash: bb80ef07364a575f6032bb105cff83cd8f95bd63
ms.sourcegitcommit: dd43cc0a9470f98b8ef2a3787c823801d674c666
ms.translationtype: MT
ms.contentlocale: id-ID
ms.lasthandoff: 02/12/2019
ms.locfileid: "29912102"
---
# <a name="problems-with-dlp---usuk-passport-numbers"></a><span data-ttu-id="47520-102">Masalah dengan DLP - U.S. / nomor paspor Inggris</span><span class="sxs-lookup"><span data-stu-id="47520-102">Problems with DLP - US/UK Passport Numbers</span></span>

<span data-ttu-id="47520-p101">Apakah Anda mengalami masalah dengan **Data Rugi Pencegahan (DLP)** tidak bekerja karena mengandung konten **U.S. / nomor paspor Inggris** ketika menggunakan jenis informasi sensitif DLP di O365? Jika demikian, pastikan konten Anda berisi informasi yang dibutuhkan untuk apa kebijakan DLP dicari ketika itu dievaluasi.</span><span class="sxs-lookup"><span data-stu-id="47520-p101">Are you having problems with **Data Loss Prevention (DLP)** not working for content containing a **US/UK Passport Number** when using a DLP sensitive information type in O365? If so, make sure your content contains the needed information for what the DLP policy is looking for when it is evaluated.</span></span> 
  
<span data-ttu-id="47520-105">Misalnya, untuk **U.S. / nomor paspor Inggris** kebijakan dikonfigurasi dengan tingkat keyakinan 75%, berikut dievaluasi dan harus terdeteksi untuk aturan untuk memicu</span><span class="sxs-lookup"><span data-stu-id="47520-105">For example, for a **US/UK Passport Number** policy configured with a confidence level of 75%, the following are evaluated and must be detected for the rule to trigger</span></span> 
  
- <span data-ttu-id="47520-106">**[Format:](https://docs.microsoft.com/office365/securitycompliance/what-the-sensitive-information-types-look-for#format-77)** Sembilan angka</span><span class="sxs-lookup"><span data-stu-id="47520-106">**[Format:](https://docs.microsoft.com/office365/securitycompliance/what-the-sensitive-information-types-look-for#format-77)** Nine digits</span></span> 
    
- <span data-ttu-id="47520-107">**[Pola:](https://docs.microsoft.com/office365/securitycompliance/what-the-sensitive-information-types-look-for#pattern-77)** Sembilan angka berturut-turut</span><span class="sxs-lookup"><span data-stu-id="47520-107">**[Pattern:](https://docs.microsoft.com/office365/securitycompliance/what-the-sensitive-information-types-look-for#pattern-77)** Nine consecutive digits</span></span> 
    
- <span data-ttu-id="47520-108">**[Checksum:](https://docs.microsoft.com/office365/securitycompliance/what-the-sensitive-information-types-look-for#checksum-76)** Tidak, adalah tidak terdapat Checksum</span><span class="sxs-lookup"><span data-stu-id="47520-108">**[Checksum:](https://docs.microsoft.com/office365/securitycompliance/what-the-sensitive-information-types-look-for#checksum-76)** No, there is no Checksum</span></span> 
    
- <span data-ttu-id="47520-109">**[Definisi:](https://docs.microsoft.com/office365/securitycompliance/what-the-sensitive-information-types-look-for#definition-77)** Kebijakan DLP adalah 75% yakin bahwa ia telah mendeteksi jenis informasi sensitif jika, dalam jarak 300 karakter:</span><span class="sxs-lookup"><span data-stu-id="47520-109">**[Definition:](https://docs.microsoft.com/office365/securitycompliance/what-the-sensitive-information-types-look-for#definition-77)** A DLP policy is 75% confident that it's detected this type of sensitive information if, within a proximity of 300 characters:</span></span> 
    
  - <span data-ttu-id="47520-110">Fungsi Func_usa_uk_passport menemukan konten yang cocok dengan pola.</span><span class="sxs-lookup"><span data-stu-id="47520-110">The function Func_usa_uk_passport finds content that matches the pattern.</span></span>
    
  - <span data-ttu-id="47520-111">Kata kunci dari Keyword_passport ditemukan.</span><span class="sxs-lookup"><span data-stu-id="47520-111">A keyword from Keyword_passport is found.</span></span>
    
    <span data-ttu-id="47520-112">Misalnya, contoh berikut akan memicu untuk **U.S. / nomor paspor Inggris** kebijakan: nomor paspor AS 123456789</span><span class="sxs-lookup"><span data-stu-id="47520-112">For example, the following sample would trigger for the **US/UK Passport Number** policy: U.S. Passport number 123456789</span></span> 
    
<span data-ttu-id="47520-113">Untuk informasi lebih lanjut tentang apa saja diperlukan untuk US / nomor paspor Inggris untuk terdeteksi untuk konten Anda, lihat bagian berikut dalam artikel ini: [apa the sensitif informasi jenis tampilan untuk US / nomor paspor Inggris](https://docs.microsoft.com/office365/securitycompliance/what-the-sensitive-information-types-look-for#us--uk-passport-number)</span><span class="sxs-lookup"><span data-stu-id="47520-113">For more information on what is required for a US/UK Passport Number to be detected for your content, see the following section in this article: [What the Sensitive Information Types look for US/UK Passport Number](https://docs.microsoft.com/office365/securitycompliance/what-the-sensitive-information-types-look-for#us--uk-passport-number)</span></span>
  
<span data-ttu-id="47520-114">Menggunakan jenis informasi sensitif built-in yang berbeda, lihat artikel berikut untuk informasi apa saja diperlukan untuk jenis lainnya: [apa the sensitif informasi jenis mencari](https://docs.microsoft.com/office365/securitycompliance/what-the-sensitive-information-types-look-for)</span><span class="sxs-lookup"><span data-stu-id="47520-114">Using a different built-in sensitive information type, see the following article for information on what is required for other types: [What the Sensitive Information Types look for](https://docs.microsoft.com/office365/securitycompliance/what-the-sensitive-information-types-look-for)</span></span>
  

