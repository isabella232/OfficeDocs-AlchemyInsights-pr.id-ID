---
title: Aturan DLP untuk US/Inggris paspor nomor tidak bekerja
ms.author: deniseb
author: denisebmsft
manager: laurawi
ms.date: 11/5/2018
ms.audience: ITPro
ms.topic: article
ROBOTS: NOINDEX, NOFOLLOW
localization_priority: Normal
ms.custom:
- "1319"
- "3200001"
ms.assetid: fc178b8b-943b-4346-a2bd-a75c6af6f80f
ms.openlocfilehash: 534e258c31a9a71c618765511487487c53f455b5
ms.sourcegitcommit: d108a2da2f5dab05246e30b5108cca5173e09051
ms.translationtype: MT
ms.contentlocale: id-ID
ms.lasthandoff: 03/26/2020
ms.locfileid: "42977109"
---
# <a name="problems-with-dlp---usuk-passport-numbers"></a><span data-ttu-id="2153f-102">Masalah dengan DLP-US/Inggris nomor paspor</span><span class="sxs-lookup"><span data-stu-id="2153f-102">Problems with DLP - US/UK passport numbers</span></span>

<span data-ttu-id="2153f-103">**Penting**: selama waktu yang belum pernah terjadi sebelumnya, kami mengambil langkah untuk memastikan bahwa Layanan SharePoint online dan OneDrive tetap sangat tersedia-silakan kunjungi [penyesuaian fitur sementara SharePoint online](https://aka.ms/ODSPAdjustments) untuk informasi lebih lanjut.</span><span class="sxs-lookup"><span data-stu-id="2153f-103">**Important**: During these unprecedented times, we are taking steps to ensure that SharePoint Online and OneDrive services remain highly available – Please visit [SharePoint Online Temporary Feature Adjustments](https://aka.ms/ODSPAdjustments) for more information.</span></span>

<span data-ttu-id="2153f-104">**Masalah DLP dengan nomor paspor AS/Inggris**</span><span class="sxs-lookup"><span data-stu-id="2153f-104">**DLP issues with US/UK passport numbers**</span></span>

<span data-ttu-id="2153f-105">Apakah Anda mengalami masalah dengan **pencegahan kehilangan data (DLP)** yang tidak bekerja untuk konten yang berisi **nomor paspor AS/Inggris** saat menggunakan jenis informasi sensitif DLP di O365?</span><span class="sxs-lookup"><span data-stu-id="2153f-105">Are you having problems with **Data Loss Prevention (DLP)** not working for content containing a **US/UK passport number** when using a DLP sensitive information type in O365?</span></span> <span data-ttu-id="2153f-106">Jika demikian, pastikan konten Anda berisi informasi yang diperlukan untuk apa kebijakan DLP Cari ketika dievaluasi.</span><span class="sxs-lookup"><span data-stu-id="2153f-106">If so, make sure your content contains the needed information for what the DLP policy is looking for when it is evaluated.</span></span>
  
<span data-ttu-id="2153f-107">Misalnya, untuk kebijakan **nomor paspor AS/Inggris** yang dikonfigurasi dengan tingkat kepercayaan 75%, berikut dievaluasi dan harus terdeteksi untuk aturan untuk memicu</span><span class="sxs-lookup"><span data-stu-id="2153f-107">For example, for a **US/UK passport number** policy configured with a confidence level of 75%, the following are evaluated and must be detected for the rule to trigger</span></span>
  
- <span data-ttu-id="2153f-108">**[Format:](https://docs.microsoft.com/office365/securitycompliance/what-the-sensitive-information-types-look-for#format-77)** Sembilan digit</span><span class="sxs-lookup"><span data-stu-id="2153f-108">**[Format:](https://docs.microsoft.com/office365/securitycompliance/what-the-sensitive-information-types-look-for#format-77)** Nine digits</span></span>

- <span data-ttu-id="2153f-109">**[Pola:](https://docs.microsoft.com/office365/securitycompliance/what-the-sensitive-information-types-look-for#pattern-77)** Sembilan digit berturut-turut</span><span class="sxs-lookup"><span data-stu-id="2153f-109">**[Pattern:](https://docs.microsoft.com/office365/securitycompliance/what-the-sensitive-information-types-look-for#pattern-77)** Nine consecutive digits</span></span>

- <span data-ttu-id="2153f-110">**[Checksum:](https://docs.microsoft.com/office365/securitycompliance/what-the-sensitive-information-types-look-for#checksum-76)** Tidak, tidak ada checksum</span><span class="sxs-lookup"><span data-stu-id="2153f-110">**[Checksum:](https://docs.microsoft.com/office365/securitycompliance/what-the-sensitive-information-types-look-for#checksum-76)** No, there is no Checksum</span></span>

- <span data-ttu-id="2153f-111">**[Definisi:](https://docs.microsoft.com/office365/securitycompliance/what-the-sensitive-information-types-look-for#definition-77)** Sebuah kebijakan DLP adalah 75% yakin bahwa hal itu terdeteksi jenis informasi sensitif jika, dalam kedekatan 300 karakter:</span><span class="sxs-lookup"><span data-stu-id="2153f-111">**[Definition:](https://docs.microsoft.com/office365/securitycompliance/what-the-sensitive-information-types-look-for#definition-77)** A DLP policy is 75% confident that it's detected this type of sensitive information if, within a proximity of 300 characters:</span></span>

  - <span data-ttu-id="2153f-112">Fungsi Func_usa_uk_passport menemukan konten yang sesuai dengan pola.</span><span class="sxs-lookup"><span data-stu-id="2153f-112">The function Func_usa_uk_passport finds content that matches the pattern.</span></span>

  - <span data-ttu-id="2153f-113">Kata kunci dari Keyword_passport ditemukan.</span><span class="sxs-lookup"><span data-stu-id="2153f-113">A keyword from Keyword_passport is found.</span></span>

    <span data-ttu-id="2153f-114">Sebagai contoh, contoh berikut akan memicu untuk kebijakan **nomor paspor AS/Inggris** : nomor paspor AS 123456789</span><span class="sxs-lookup"><span data-stu-id="2153f-114">For example, the following sample would trigger for the **US/UK passport number** policy: U.S. Passport number 123456789</span></span>

<span data-ttu-id="2153f-115">Untuk informasi lebih lanjut tentang apa yang diperlukan untuk nomor paspor AS/Inggris yang akan terdeteksi untuk konten Anda, lihat bagian berikut dalam artikel ini: [apa jenis informasi sensitif mencari US/Inggris nomor paspor](https://docs.microsoft.com/office365/securitycompliance/what-the-sensitive-information-types-look-for#us--uk-passport-number)</span><span class="sxs-lookup"><span data-stu-id="2153f-115">For more information on what is required for a US/UK Passport Number to be detected for your content, see the following section in this article: [What the Sensitive Information Types look for US/UK Passport Number](https://docs.microsoft.com/office365/securitycompliance/what-the-sensitive-information-types-look-for#us--uk-passport-number)</span></span>
  
<span data-ttu-id="2153f-116">Menggunakan jenis informasi sensitif internal yang berbeda, lihat artikel berikut untuk informasi tentang apa yang diperlukan untuk jenis lain: [apa jenis informasi sensitif](https://docs.microsoft.com/office365/securitycompliance/what-the-sensitive-information-types-look-for) mencari</span><span class="sxs-lookup"><span data-stu-id="2153f-116">Using a different built-in sensitive information type, see the following article for information on what is required for other types: [What the Sensitive Information Types look for](https://docs.microsoft.com/office365/securitycompliance/what-the-sensitive-information-types-look-for)</span></span>
  