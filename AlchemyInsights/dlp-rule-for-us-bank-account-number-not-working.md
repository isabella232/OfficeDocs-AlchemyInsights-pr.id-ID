---
title: Aturan DLP untuk nomor rekening bank AS tidak berfungsi
ms.author: deniseb
author: denisebmsft
manager: laurawi
ms.date: 04/21/2020
ms.audience: ITPro
ms.topic: article
ROBOTS: NOINDEX, NOFOLLOW
localization_priority: Normal
ms.custom:
- "1287"
- "3200001"
ms.assetid: 80b40145-8376-4c3a-8d22-6efb9f9cb271
ms.openlocfilehash: b032a7c80e8b387114aeda95c4f6af7e57225517
ms.sourcegitcommit: bc7d6f4f3c9f7060d073f5130e1ec856e248d020
ms.translationtype: MT
ms.contentlocale: id-ID
ms.lasthandoff: 06/02/2020
ms.locfileid: "44507337"
---
# <a name="dlp-issues-with-us-bank-account-numbers"></a><span data-ttu-id="e0c30-102">Masalah DLP dengan nomor rekening bank AS</span><span class="sxs-lookup"><span data-stu-id="e0c30-102">DLP issues with US bank account numbers</span></span>

<span data-ttu-id="e0c30-103">**Penting**: Selama masa-masa yang berat ini, kami mengambil langkah untuk memastikan bahwa SharePoint Online dan layanan OneDrive tetap memiliki ketersediaan yang tinggi. Silakan kunjungi [Penyesuaian Fitur Sementara SharePoint Online](https://aka.ms/ODSPAdjustments) untuk informasi selengkapnya.</span><span class="sxs-lookup"><span data-stu-id="e0c30-103">**Important**: During these unprecedented times, we are taking steps to ensure that SharePoint Online and OneDrive services remain highly available – Please visit [SharePoint Online Temporary Feature Adjustments](https://aka.ms/ODSPAdjustments) for more information.</span></span>

<span data-ttu-id="e0c30-104">**Masalah DLP dengan nomor rekening bank AS**</span><span class="sxs-lookup"><span data-stu-id="e0c30-104">**DLP issues with US bank account numbers**</span></span>

<span data-ttu-id="e0c30-105">Apakah Anda mengalami masalah dengan **pencegahan kehilangan data (DLP)** yang tidak berfungsi untuk konten yang berisi **nomor rekening bank AS** saat menggunakan jenis informasi sensitif DLP di O365?</span><span class="sxs-lookup"><span data-stu-id="e0c30-105">Are you having problems with **Data Loss Prevention (DLP)** not working for content containing a **US Bank Account Number** when using a DLP sensitive information type in O365?</span></span> <span data-ttu-id="e0c30-106">Jika demikian, pastikan konten Anda berisi informasi yang diperlukan untuk apa kebijakan DLP Cari ketika dievaluasi.</span><span class="sxs-lookup"><span data-stu-id="e0c30-106">If so, make sure your content contains the needed information for what the DLP policy is looking for when it is evaluated.</span></span>
  
<span data-ttu-id="e0c30-107">Misalnya, untuk kebijakan **nomor rekening bank AS** yang dikonfigurasi dengan tingkat kepercayaan 85%, berikut dievaluasi dan harus terdeteksi aturan untuk memicu:</span><span class="sxs-lookup"><span data-stu-id="e0c30-107">For example, for a **US Bank Account Number** policy configured with a confidence level of 85%, the following are evaluated and must be detected for the rule to trigger:</span></span>
  
- <span data-ttu-id="e0c30-108">**[Format:](https://docs.microsoft.com/microsoft-365/compliance/sensitive-information-type-entity-definitions#format-77)** 8-17 digit</span><span class="sxs-lookup"><span data-stu-id="e0c30-108">**[Format:](https://docs.microsoft.com/microsoft-365/compliance/sensitive-information-type-entity-definitions#format-77)** 8-17 digits</span></span>

- <span data-ttu-id="e0c30-109">**[Pattern:](https://docs.microsoft.com/microsoft-365/compliance/sensitive-information-type-entity-definitions#pattern-77)** 8-17 digit berturut-turut.</span><span class="sxs-lookup"><span data-stu-id="e0c30-109">**[Pattern:](https://docs.microsoft.com/microsoft-365/compliance/sensitive-information-type-entity-definitions#pattern-77)** 8-17 consecutive digits.</span></span>

- <span data-ttu-id="e0c30-110">**[Checksum:](https://docs.microsoft.com/microsoft-365/compliance/sensitive-information-type-entity-definitions#checksum-76)** Tidak, tidak ada checksum</span><span class="sxs-lookup"><span data-stu-id="e0c30-110">**[Checksum:](https://docs.microsoft.com/microsoft-365/compliance/sensitive-information-type-entity-definitions#checksum-76)** No, there is no Checksum</span></span>

- <span data-ttu-id="e0c30-111">**[Definisi:](https://docs.microsoft.com/microsoft-365/compliance/sensitive-information-type-entity-definitions)** Sebuah kebijakan DLP adalah 75% yakin bahwa hal itu terdeteksi jenis informasi sensitif jika, dalam kedekatan 300 karakter:</span><span class="sxs-lookup"><span data-stu-id="e0c30-111">**[Definition:](https://docs.microsoft.com/microsoft-365/compliance/sensitive-information-type-entity-definitions)** A DLP policy is 75% confident that it's detected this type of sensitive information if, within a proximity of 300 characters:</span></span>

  - <span data-ttu-id="e0c30-112">Ekspresi reguler Regex_usa_bank_account_number menemukan konten yang sesuai dengan pola</span><span class="sxs-lookup"><span data-stu-id="e0c30-112">The regular expression Regex_usa_bank_account_number finds content that matches the pattern</span></span>

  - <span data-ttu-id="e0c30-113">Kata kunci dari Keyword_usa_Bank_Account ditemukan.</span><span class="sxs-lookup"><span data-stu-id="e0c30-113">A keyword from Keyword_usa_Bank_Account is found.</span></span>

    <span data-ttu-id="e0c30-114">Sebagai contoh, contoh berikut akan memicu untuk kebijakan **nomor rekening bank AS** : memeriksa akun 78344011</span><span class="sxs-lookup"><span data-stu-id="e0c30-114">For example, the following sample would trigger for the **US Bank Account Number** policy: Checking Account 78344011</span></span>

<span data-ttu-id="e0c30-115">Untuk informasi lebih lanjut tentang apa yang diperlukan untuk **nomor rekening bank AS** untuk terdeteksi untuk konten Anda, lihat bagian berikut dalam artikel ini: [apa jenis informasi sensitif mencari nomor rekening bank AS](https://docs.microsoft.com/microsoft-365/compliance/sensitive-information-type-entity-definitions#us-bank-account-number)</span><span class="sxs-lookup"><span data-stu-id="e0c30-115">For more information on what is required for a **US Bank Account Number** to be detected for your content, see the following section in this article: [What the Sensitive Information Types look for US Bank Account Number](https://docs.microsoft.com/microsoft-365/compliance/sensitive-information-type-entity-definitions#us-bank-account-number)</span></span>
  
<span data-ttu-id="e0c30-116">Menggunakan jenis informasi sensitif internal yang berbeda, lihat artikel berikut untuk informasi tentang apa yang diperlukan untuk jenis lain: [apa jenis informasi sensitif](https://docs.microsoft.com/microsoft-365/compliance/sensitive-information-type-entity-definitions) mencari</span><span class="sxs-lookup"><span data-stu-id="e0c30-116">Using a different built-in sensitive information type, see the following article for information on what is required for other types: [What the Sensitive Information Types look for](https://docs.microsoft.com/microsoft-365/compliance/sensitive-information-type-entity-definitions)</span></span>
  