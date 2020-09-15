---
title: Aturan DLP untuk nomor paspor AS/Inggris tidak berfungsi
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
- "1319"
- "3200001"
ms.assetid: fc178b8b-943b-4346-a2bd-a75c6af6f80f
ms.openlocfilehash: c6c7191f380f264113e2042f2869d9767922b2cc
ms.sourcegitcommit: c6692ce0fa1358ec3529e59ca0ecdfdea4cdc759
ms.translationtype: MT
ms.contentlocale: id-ID
ms.lasthandoff: 09/14/2020
ms.locfileid: "47679227"
---
# <a name="problems-with-dlp---usuk-passport-numbers"></a><span data-ttu-id="8ed54-102">Masalah dengan DLP-nomor paspor AS/Inggris</span><span class="sxs-lookup"><span data-stu-id="8ed54-102">Problems with DLP - US/UK passport numbers</span></span>

<span data-ttu-id="8ed54-103">**Penting**: Selama masa-masa yang berat ini, kami mengambil langkah untuk memastikan bahwa SharePoint Online dan layanan OneDrive tetap memiliki ketersediaan yang tinggi. Silakan kunjungi [Penyesuaian Fitur Sementara SharePoint Online](https://aka.ms/ODSPAdjustments) untuk informasi selengkapnya.</span><span class="sxs-lookup"><span data-stu-id="8ed54-103">**Important**: During these unprecedented times, we are taking steps to ensure that SharePoint Online and OneDrive services remain highly available – Please visit [SharePoint Online Temporary Feature Adjustments](https://aka.ms/ODSPAdjustments) for more information.</span></span>

<span data-ttu-id="8ed54-104">**Masalah DLP dengan nomor paspor AS/Inggris**</span><span class="sxs-lookup"><span data-stu-id="8ed54-104">**DLP issues with US/UK passport numbers**</span></span>

<span data-ttu-id="8ed54-105">Apakah Anda mengalami masalah dengan **pencegahan kehilangan data (DLP)** tidak berfungsi untuk konten yang berisi **nomor paspor AS/Inggris** saat menggunakan tipe informasi sensitif DLP di O365?</span><span class="sxs-lookup"><span data-stu-id="8ed54-105">Are you having problems with **Data Loss Prevention (DLP)** not working for content containing a **US/UK passport number** when using a DLP sensitive information type in O365?</span></span> <span data-ttu-id="8ed54-106">Jika demikian, pastikan konten Anda berisi informasi yang diperlukan tentang apa yang dicari kebijakan DLP saat dievaluasi.</span><span class="sxs-lookup"><span data-stu-id="8ed54-106">If so, make sure your content contains the needed information for what the DLP policy is looking for when it is evaluated.</span></span>
  
<span data-ttu-id="8ed54-107">Misalnya, untuk kebijakan **nomor paspor AS/Inggris** yang dikonfigurasikan dengan tingkat kepercayaan 75%, hal berikut dievaluasi dan harus dideteksi agar aturan dapat dipicu</span><span class="sxs-lookup"><span data-stu-id="8ed54-107">For example, for a **US/UK passport number** policy configured with a confidence level of 75%, the following are evaluated and must be detected for the rule to trigger</span></span>
  
- <span data-ttu-id="8ed54-108">**[Format:](https://docs.microsoft.com/microsoft-365/compliance/sensitive-information-type-entity-definitions#format-77)** Sembilan digit</span><span class="sxs-lookup"><span data-stu-id="8ed54-108">**[Format:](https://docs.microsoft.com/microsoft-365/compliance/sensitive-information-type-entity-definitions#format-77)** Nine digits</span></span>

- <span data-ttu-id="8ed54-109">**[Pola:](https://docs.microsoft.com/microsoft-365/compliance/sensitive-information-type-entity-definitions#pattern-77)** Sembilan digit berurutan</span><span class="sxs-lookup"><span data-stu-id="8ed54-109">**[Pattern:](https://docs.microsoft.com/microsoft-365/compliance/sensitive-information-type-entity-definitions#pattern-77)** Nine consecutive digits</span></span>

- <span data-ttu-id="8ed54-110">**[Checksum:](https://docs.microsoft.com/microsoft-365/compliance/sensitive-information-type-entity-definitions#checksum-76)** Tidak, tidak ada checksum</span><span class="sxs-lookup"><span data-stu-id="8ed54-110">**[Checksum:](https://docs.microsoft.com/microsoft-365/compliance/sensitive-information-type-entity-definitions#checksum-76)** No, there is no Checksum</span></span>

- <span data-ttu-id="8ed54-111">**[Definisi:](https://docs.microsoft.com/microsoft-365/compliance/sensitive-information-type-entity-definitions#definition-77)** Kebijakan DLP adalah 75% yakin bahwa kebijakan ini mendeteksi tipe informasi sensitif ini jika, dalam kedekatan karakter 300:</span><span class="sxs-lookup"><span data-stu-id="8ed54-111">**[Definition:](https://docs.microsoft.com/microsoft-365/compliance/sensitive-information-type-entity-definitions#definition-77)** A DLP policy is 75% confident that it's detected this type of sensitive information if, within a proximity of 300 characters:</span></span>

  - <span data-ttu-id="8ed54-112">Fungsi Func_usa_uk_passport menemukan konten yang cocok dengan pola.</span><span class="sxs-lookup"><span data-stu-id="8ed54-112">The function Func_usa_uk_passport finds content that matches the pattern.</span></span>

  - <span data-ttu-id="8ed54-113">Kata kunci dari Keyword_passport ditemukan.</span><span class="sxs-lookup"><span data-stu-id="8ed54-113">A keyword from Keyword_passport is found.</span></span>

    <span data-ttu-id="8ed54-114">Misalnya, contoh berikut ini akan memicu kebijakan **nomor paspor AS/Inggris** : nomor paspor AS 123456789</span><span class="sxs-lookup"><span data-stu-id="8ed54-114">For example, the following sample would trigger for the **US/UK passport number** policy: U.S. Passport number 123456789</span></span>

<span data-ttu-id="8ed54-115">Untuk informasi selengkapnya tentang apa yang diperlukan untuk nomor paspor AS/Inggris yang akan terdeteksi untuk konten Anda, lihat bagian berikut ini di artikel ini: [apa tipe informasi sensitif Cari nomor paspor AS/UK](https://docs.microsoft.com/microsoft-365/compliance/sensitive-information-type-entity-definitions#us--uk-passport-number)</span><span class="sxs-lookup"><span data-stu-id="8ed54-115">For more information on what is required for a US/UK Passport Number to be detected for your content, see the following section in this article: [What the Sensitive Information Types look for US/UK Passport Number](https://docs.microsoft.com/microsoft-365/compliance/sensitive-information-type-entity-definitions#us--uk-passport-number)</span></span>
  
<span data-ttu-id="8ed54-116">Menggunakan tipe informasi sensitif bawaan yang berbeda, lihat artikel berikut ini untuk informasi tentang apa yang diperlukan untuk tipe lainnya: [apa yang dicari tipe informasi sensitif](https://docs.microsoft.com/microsoft-365/compliance/sensitive-information-type-entity-definitions)</span><span class="sxs-lookup"><span data-stu-id="8ed54-116">Using a different built-in sensitive information type, see the following article for information on what is required for other types: [What the Sensitive Information Types look for](https://docs.microsoft.com/microsoft-365/compliance/sensitive-information-type-entity-definitions)</span></span>
  