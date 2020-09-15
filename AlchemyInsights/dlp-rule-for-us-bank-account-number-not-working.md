---
title: Aturan DLP untuk nomor rekening bank AS tidak berfungsi
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
- "1287"
- "3200001"
ms.assetid: 80b40145-8376-4c3a-8d22-6efb9f9cb271
ms.openlocfilehash: eb399e4b23de32a757562833ed32d97daa6a1247
ms.sourcegitcommit: c6692ce0fa1358ec3529e59ca0ecdfdea4cdc759
ms.translationtype: MT
ms.contentlocale: id-ID
ms.lasthandoff: 09/14/2020
ms.locfileid: "47679299"
---
# <a name="dlp-issues-with-us-bank-account-numbers"></a><span data-ttu-id="725bd-102">Masalah DLP dengan nomor rekening bank AS</span><span class="sxs-lookup"><span data-stu-id="725bd-102">DLP issues with US bank account numbers</span></span>

<span data-ttu-id="725bd-103">**Penting**: Selama masa-masa yang berat ini, kami mengambil langkah untuk memastikan bahwa SharePoint Online dan layanan OneDrive tetap memiliki ketersediaan yang tinggi. Silakan kunjungi [Penyesuaian Fitur Sementara SharePoint Online](https://aka.ms/ODSPAdjustments) untuk informasi selengkapnya.</span><span class="sxs-lookup"><span data-stu-id="725bd-103">**Important**: During these unprecedented times, we are taking steps to ensure that SharePoint Online and OneDrive services remain highly available – Please visit [SharePoint Online Temporary Feature Adjustments](https://aka.ms/ODSPAdjustments) for more information.</span></span>

<span data-ttu-id="725bd-104">**Masalah DLP dengan nomor rekening bank AS**</span><span class="sxs-lookup"><span data-stu-id="725bd-104">**DLP issues with US bank account numbers**</span></span>

<span data-ttu-id="725bd-105">Apakah Anda mengalami masalah dengan **pencegahan kehilangan data (DLP)** tidak berfungsi untuk konten yang berisi **nomor rekening bank AS** saat menggunakan tipe informasi sensitif DLP di O365?</span><span class="sxs-lookup"><span data-stu-id="725bd-105">Are you having problems with **Data Loss Prevention (DLP)** not working for content containing a **US Bank Account Number** when using a DLP sensitive information type in O365?</span></span> <span data-ttu-id="725bd-106">Jika demikian, pastikan konten Anda berisi informasi yang diperlukan tentang apa yang dicari kebijakan DLP saat dievaluasi.</span><span class="sxs-lookup"><span data-stu-id="725bd-106">If so, make sure your content contains the needed information for what the DLP policy is looking for when it is evaluated.</span></span>
  
<span data-ttu-id="725bd-107">Misalnya, untuk kebijakan **nomor rekening bank AS** yang dikonfigurasi dengan tingkat kepercayaan 85%, hal berikut dievaluasi dan harus dideteksi agar aturan dipicu:</span><span class="sxs-lookup"><span data-stu-id="725bd-107">For example, for a **US Bank Account Number** policy configured with a confidence level of 85%, the following are evaluated and must be detected for the rule to trigger:</span></span>
  
- <span data-ttu-id="725bd-108">**[Format:](https://docs.microsoft.com/microsoft-365/compliance/sensitive-information-type-entity-definitions#format-77)** 8-17 digit</span><span class="sxs-lookup"><span data-stu-id="725bd-108">**[Format:](https://docs.microsoft.com/microsoft-365/compliance/sensitive-information-type-entity-definitions#format-77)** 8-17 digits</span></span>

- <span data-ttu-id="725bd-109">**[Pola:](https://docs.microsoft.com/microsoft-365/compliance/sensitive-information-type-entity-definitions#pattern-77)** 8-17 digit berturut-turut.</span><span class="sxs-lookup"><span data-stu-id="725bd-109">**[Pattern:](https://docs.microsoft.com/microsoft-365/compliance/sensitive-information-type-entity-definitions#pattern-77)** 8-17 consecutive digits.</span></span>

- <span data-ttu-id="725bd-110">**[Checksum:](https://docs.microsoft.com/microsoft-365/compliance/sensitive-information-type-entity-definitions#checksum-76)** Tidak, tidak ada checksum</span><span class="sxs-lookup"><span data-stu-id="725bd-110">**[Checksum:](https://docs.microsoft.com/microsoft-365/compliance/sensitive-information-type-entity-definitions#checksum-76)** No, there is no Checksum</span></span>

- <span data-ttu-id="725bd-111">**[Definisi:](https://docs.microsoft.com/microsoft-365/compliance/sensitive-information-type-entity-definitions)** Kebijakan DLP adalah 75% yakin bahwa kebijakan ini mendeteksi tipe informasi sensitif ini jika, dalam kedekatan karakter 300:</span><span class="sxs-lookup"><span data-stu-id="725bd-111">**[Definition:](https://docs.microsoft.com/microsoft-365/compliance/sensitive-information-type-entity-definitions)** A DLP policy is 75% confident that it's detected this type of sensitive information if, within a proximity of 300 characters:</span></span>

  - <span data-ttu-id="725bd-112">Ekspresi reguler Regex_usa_bank_account_number menemukan konten yang cocok dengan pola</span><span class="sxs-lookup"><span data-stu-id="725bd-112">The regular expression Regex_usa_bank_account_number finds content that matches the pattern</span></span>

  - <span data-ttu-id="725bd-113">Kata kunci dari Keyword_usa_Bank_Account ditemukan.</span><span class="sxs-lookup"><span data-stu-id="725bd-113">A keyword from Keyword_usa_Bank_Account is found.</span></span>

    <span data-ttu-id="725bd-114">Misalnya, contoh berikut ini akan memicu kebijakan **nomor rekening bank AS** : memeriksa akun 78344011</span><span class="sxs-lookup"><span data-stu-id="725bd-114">For example, the following sample would trigger for the **US Bank Account Number** policy: Checking Account 78344011</span></span>

<span data-ttu-id="725bd-115">Untuk informasi selengkapnya tentang apa yang diperlukan untuk **nomor rekening bank AS** yang akan terdeteksi untuk konten Anda, lihat bagian berikut ini di artikel ini: [apa tipe informasi sensitif Cari nomor rekening bank AS](https://docs.microsoft.com/microsoft-365/compliance/sensitive-information-type-entity-definitions#us-bank-account-number)</span><span class="sxs-lookup"><span data-stu-id="725bd-115">For more information on what is required for a **US Bank Account Number** to be detected for your content, see the following section in this article: [What the Sensitive Information Types look for US Bank Account Number](https://docs.microsoft.com/microsoft-365/compliance/sensitive-information-type-entity-definitions#us-bank-account-number)</span></span>
  
<span data-ttu-id="725bd-116">Menggunakan tipe informasi sensitif bawaan yang berbeda, lihat artikel berikut ini untuk informasi tentang apa yang diperlukan untuk tipe lainnya: [apa yang dicari tipe informasi sensitif](https://docs.microsoft.com/microsoft-365/compliance/sensitive-information-type-entity-definitions)</span><span class="sxs-lookup"><span data-stu-id="725bd-116">Using a different built-in sensitive information type, see the following article for information on what is required for other types: [What the Sensitive Information Types look for](https://docs.microsoft.com/microsoft-365/compliance/sensitive-information-type-entity-definitions)</span></span>
  