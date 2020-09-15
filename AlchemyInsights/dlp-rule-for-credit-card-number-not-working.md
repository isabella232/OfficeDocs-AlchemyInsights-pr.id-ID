---
title: Aturan DLP untuk nomor kartu kredit tidak berfungsi
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
- "1270"
- "3200001"
ms.assetid: 30496c79-c8b4-4337-a46d-abed12864209
ms.openlocfilehash: d5dd6354e7a1bcbb7f2fb917952ddbee5077e88d
ms.sourcegitcommit: c6692ce0fa1358ec3529e59ca0ecdfdea4cdc759
ms.translationtype: MT
ms.contentlocale: id-ID
ms.lasthandoff: 09/14/2020
ms.locfileid: "47679444"
---
# <a name="dlp-issues-with-credit-card-numbers"></a><span data-ttu-id="956aa-102">Masalah DLP dengan nomor kartu kredit</span><span class="sxs-lookup"><span data-stu-id="956aa-102">DLP issues with credit card numbers</span></span>

<span data-ttu-id="956aa-103">**Penting**: Selama masa-masa yang berat ini, kami mengambil langkah untuk memastikan bahwa SharePoint Online dan layanan OneDrive tetap memiliki ketersediaan yang tinggi. Silakan kunjungi [Penyesuaian Fitur Sementara SharePoint Online](https://aka.ms/ODSPAdjustments) untuk informasi selengkapnya.</span><span class="sxs-lookup"><span data-stu-id="956aa-103">**Important**: During these unprecedented times, we are taking steps to ensure that SharePoint Online and OneDrive services remain highly available – Please visit [SharePoint Online Temporary Feature Adjustments](https://aka.ms/ODSPAdjustments) for more information.</span></span>

<span data-ttu-id="956aa-104">**Masalah DLP dengan nomor kartu kredit**</span><span class="sxs-lookup"><span data-stu-id="956aa-104">**DLP issues with credit card numbers**</span></span>

<span data-ttu-id="956aa-105">Apakah Anda mengalami masalah dengan **pencegahan kehilangan data (DLP)** tidak berfungsi untuk konten yang berisi **nomor kartu kredit** ketika menggunakan tipe informasi sensitif DLP di O365?</span><span class="sxs-lookup"><span data-stu-id="956aa-105">Are you having problems with **Data Loss Prevention (DLP)** not working for content containing a **Credit Card Number** when using a DLP sensitive information type in O365?</span></span> <span data-ttu-id="956aa-106">Jika demikian, pastikan konten Anda berisi informasi yang diperlukan untuk memicu kebijakan DLP saat dievaluasi.</span><span class="sxs-lookup"><span data-stu-id="956aa-106">If so, make sure your content contains the needed information to trigger the the DLP policy when it is evaluated.</span></span> <span data-ttu-id="956aa-107">Misalnya, untuk **kebijakan kartu kredit** yang dikonfigurasikan dengan tingkat kepercayaan 85%, hal berikut dievaluasi dan harus dideteksi agar aturan dipicu:</span><span class="sxs-lookup"><span data-stu-id="956aa-107">For example, for a **Credit Card policy** configured with a confidence level of 85%, the following are evaluated and must be detected for the rule to trigger:</span></span>
  
- <span data-ttu-id="956aa-108">**[Format:](https://docs.microsoft.com/microsoft-365/compliance/sensitive-information-type-entity-definitions#format-19)** 16 digit yang bisa diformat atau tidak diformat (dddddddddddddddd) dan harus lulus uji Luhn.</span><span class="sxs-lookup"><span data-stu-id="956aa-108">**[Format:](https://docs.microsoft.com/microsoft-365/compliance/sensitive-information-type-entity-definitions#format-19)** 16 digits which can be formatted or unformatted (dddddddddddddddd) and must pass the Luhn test.</span></span>

- <span data-ttu-id="956aa-109">**[Pola:](https://docs.microsoft.com/microsoft-365/compliance/sensitive-information-type-entity-definitions#pattern-19)** Pola yang sangat kompleks dan kuat yang mendeteksi kartu dari semua merek utama di seluruh dunia, termasuk Visa, MasterCard, Kartu Discover, JCB, kartu American Express, Gift Cards, dan Diner.</span><span class="sxs-lookup"><span data-stu-id="956aa-109">**[Pattern:](https://docs.microsoft.com/microsoft-365/compliance/sensitive-information-type-entity-definitions#pattern-19)** Very complex and robust pattern that detects cards from all major brands worldwide, including Visa, MasterCard, Discover Card, JCB, American Express, gift cards, and diner cards.</span></span>

- <span data-ttu-id="956aa-110">**[Checksum:](https://docs.microsoft.com/microsoft-365/compliance/sensitive-information-type-entity-definitions#checksum-19)** Ya, checksum Luhn</span><span class="sxs-lookup"><span data-stu-id="956aa-110">**[Checksum:](https://docs.microsoft.com/microsoft-365/compliance/sensitive-information-type-entity-definitions#checksum-19)** Yes, the Luhn checksum</span></span>

- <span data-ttu-id="956aa-111">**[Definisi:](https://docs.microsoft.com/microsoft-365/compliance/sensitive-information-type-entity-definitions#definition-19)** Kebijakan DLP adalah 85% yakin bahwa kebijakan ini mendeteksi tipe informasi sensitif ini jika, dalam kedekatan karakter 300:</span><span class="sxs-lookup"><span data-stu-id="956aa-111">**[Definition:](https://docs.microsoft.com/microsoft-365/compliance/sensitive-information-type-entity-definitions#definition-19)** A DLP policy is 85% confident that it's detected this type of sensitive information if, within a proximity of 300 characters:</span></span>

  - <span data-ttu-id="956aa-112">Fungsi Func_credit_card menemukan konten yang cocok dengan pola.</span><span class="sxs-lookup"><span data-stu-id="956aa-112">The function Func_credit_card finds content that matches the pattern.</span></span>

  - <span data-ttu-id="956aa-113">Salah satu hal berikut ini benar:</span><span class="sxs-lookup"><span data-stu-id="956aa-113">One of the following is true:</span></span>

  - <span data-ttu-id="956aa-114">Kata kunci dari Keyword_cc_verification ditemukan.</span><span class="sxs-lookup"><span data-stu-id="956aa-114">A keyword from Keyword_cc_verification is found.</span></span>

  - <span data-ttu-id="956aa-115">Kata kunci dari Keyword_cc_name ditemukan</span><span class="sxs-lookup"><span data-stu-id="956aa-115">A keyword from Keyword_cc_name is found</span></span>

  - <span data-ttu-id="956aa-116">Fungsi Func_expiration_date menemukan tanggal dalam format tanggal yang tepat.</span><span class="sxs-lookup"><span data-stu-id="956aa-116">The function Func_expiration_date finds a date in the right date format.</span></span>

  - <span data-ttu-id="956aa-117">Tanda titik lewat</span><span class="sxs-lookup"><span data-stu-id="956aa-117">The checksum passes</span></span>

    <span data-ttu-id="956aa-118">Misalnya, sampel berikut ini akan memicu kebijakan nomor kartu kredit DLP:</span><span class="sxs-lookup"><span data-stu-id="956aa-118">For example, the following sample would trigger for a DLP Credit Card Number Policy:</span></span>

  - <span data-ttu-id="956aa-119">Visa: 4485 3647 3952 7352</span><span class="sxs-lookup"><span data-stu-id="956aa-119">Visa: 4485 3647 3952 7352</span></span>
  
  - <span data-ttu-id="956aa-120">Berakhir: 2/2009</span><span class="sxs-lookup"><span data-stu-id="956aa-120">Expires: 2/2009</span></span>

<span data-ttu-id="956aa-121">Untuk informasi selengkapnya tentang apa yang diperlukan untuk **nomor kartu kredit** yang akan terdeteksi untuk konten Anda, lihat bagian berikut ini di artikel ini: [apa tipe informasi sensitif Cari kartu kredit #](https://docs.microsoft.com/microsoft-365/compliance/sensitive-information-type-entity-definitions#credit-card-number)</span><span class="sxs-lookup"><span data-stu-id="956aa-121">For more information on what is required for a **Credit Card Number** to be detected for your content, see the following section in this article: [What the Sensitive Information Types look for Credit Card#](https://docs.microsoft.com/microsoft-365/compliance/sensitive-information-type-entity-definitions#credit-card-number)</span></span>
  
<span data-ttu-id="956aa-122">Menggunakan tipe informasi sensitif bawaan yang berbeda, lihat artikel berikut ini untuk informasi tentang apa yang diperlukan untuk tipe lainnya: [apa yang dicari tipe informasi sensitif](https://docs.microsoft.com/microsoft-365/compliance/sensitive-information-type-entity-definitions)</span><span class="sxs-lookup"><span data-stu-id="956aa-122">Using a different built-in sensitive information type, see the following article for information on what is required for other types: [What the Sensitive Information Types look for](https://docs.microsoft.com/microsoft-365/compliance/sensitive-information-type-entity-definitions)</span></span>
  