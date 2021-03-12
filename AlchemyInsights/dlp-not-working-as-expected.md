---
title: DLP tidak berfungsi seperti yang diharapkan
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
- "1241"
- "3200001"
ms.assetid: f6fcf5ad-55a1-4f25-af27-1f7c1ce06409
ms.openlocfilehash: 0f07e64c95675a4f6a0aeb6df110fe4e6a21d72f
ms.sourcegitcommit: 0eb4f9bde53395b5fd4b5cd4ffc56ca96db91298
ms.translationtype: MT
ms.contentlocale: id-ID
ms.lasthandoff: 03/10/2021
ms.locfileid: "50707813"
---
# <a name="dlp-not-working-as-expected"></a><span data-ttu-id="93261-102">DLP tidak berfungsi seperti yang diharapkan</span><span class="sxs-lookup"><span data-stu-id="93261-102">DLP not working as expected</span></span>

<span data-ttu-id="93261-103">**Penting**: Selama masa-masa yang berat ini, kami mengambil langkah untuk memastikan bahwa SharePoint Online dan layanan OneDrive tetap memiliki ketersediaan yang tinggi. Silakan kunjungi [Penyesuaian Fitur Sementara SharePoint Online](https://aka.ms/ODSPAdjustments) untuk informasi selengkapnya.</span><span class="sxs-lookup"><span data-stu-id="93261-103">**Important**: During these unprecedented times, we are taking steps to ensure that SharePoint Online and OneDrive services remain highly available – Please visit [SharePoint Online Temporary Feature Adjustments](https://aka.ms/ODSPAdjustments) for more information.</span></span>

 <span data-ttu-id="93261-104">**Menyiapkan DLP**</span><span class="sxs-lookup"><span data-stu-id="93261-104">**Setting up DLP**</span></span>

<span data-ttu-id="93261-105">Apakah Anda mengalami masalah dengan **pencegahan kehilangan data (DLP)** di Office 365 tidak berfungsi seperti yang diharapkan?</span><span class="sxs-lookup"><span data-stu-id="93261-105">Are you having problems with **Data Loss Prevention (DLP)** in Office 365 not working as expected?</span></span> <span data-ttu-id="93261-106">Jika demikian, pastikan bahwa **kebijakan DLP** Anda disetel dengan benar, dan bahwa data Anda berisi apa yang dicari **kebijakan DLP** saat dievaluasi.</span><span class="sxs-lookup"><span data-stu-id="93261-106">If so, make sure that your **DLP policy** is set up correctly, and that your data contains what the **DLP policy** is looking for when it is being evaluated.</span></span>
  
<span data-ttu-id="93261-107">Kebijakan DLP memungkinkan Anda mengidentifikasi dan melindungi informasi sensitif di organisasi Anda.</span><span class="sxs-lookup"><span data-stu-id="93261-107">DLP policies allows you to identify and protect sensitive information in your organization.</span></span> <span data-ttu-id="93261-108">Untuk menyetel kebijakan DLP, gunakan informasi [di sini](https://docs.microsoft.com/microsoft-365/compliance/create-a-dlp-policy-from-a-template).</span><span class="sxs-lookup"><span data-stu-id="93261-108">To setup DLP policies, use the information [here](https://docs.microsoft.com/microsoft-365/compliance/create-a-dlp-policy-from-a-template).</span></span>
  
 <span data-ttu-id="93261-109">**Apa yang dicari kebijakan DLP**</span><span class="sxs-lookup"><span data-stu-id="93261-109">**What DLP policies look for**</span></span>
  
<span data-ttu-id="93261-110">Saat menggunakan **tipe informasi sensitif bawaan** di pusat keamanan dan kepatuhan, kebijakan DLP mencari pola dan elemen tertentu saat mendeteksi tipe sensitif ini.</span><span class="sxs-lookup"><span data-stu-id="93261-110">When using the **built-in sensitive information types** in the Security and Compliance centers, DLP policies look for specific patterns and elements when detecting these sensitive types.</span></span>
  
- <span data-ttu-id="93261-111">**Tipe informasi sensitif bawaan**</span><span class="sxs-lookup"><span data-stu-id="93261-111">**Built-in Sensitive Information Types**</span></span>

    <span data-ttu-id="93261-112">Untuk informasi tentang tipe sensitif bawaan dan apa yang dicari kebijakan DLP saat mendeteksi tipe sensitif, lihat: [seperti apa tipe informasi sensitif tersebut](https://docs.microsoft.com/microsoft-365/compliance/sensitive-information-type-entity-definitions).</span><span class="sxs-lookup"><span data-stu-id="93261-112">For information on the built-in Sensitive types and what a DLP policy looks for when detecting the Sensitive type, see: [What the sensitive information types look for](https://docs.microsoft.com/microsoft-365/compliance/sensitive-information-type-entity-definitions).</span></span>

- <span data-ttu-id="93261-113">**Tipe informasi sensitif kustom**</span><span class="sxs-lookup"><span data-stu-id="93261-113">**Custom Sensitive Information Types**</span></span>

    <span data-ttu-id="93261-114">Jika Anda mencoba membuat tipe informasi sensitif kustom, gunakan artikel berikut ini untuk informasi tentang cara membuat tipe sensitif kustom: [membuat tipe informasi sensitif kustom](https://docs.microsoft.com/microsoft-365/compliance/create-a-custom-sensitive-information-type).</span><span class="sxs-lookup"><span data-stu-id="93261-114">If you are trying to create custom sensitive information types, use the following article for information on how to create a custom sensitive type: [Create a custom sensitive information type](https://docs.microsoft.com/microsoft-365/compliance/create-a-custom-sensitive-information-type).</span></span>

<span data-ttu-id="93261-115">**Menguji kebijakan DLP**</span><span class="sxs-lookup"><span data-stu-id="93261-115">**Test a DLP policy**</span></span>

<span data-ttu-id="93261-116">Untuk menguji data Anda dengan tipe informasi sensitif bawaan atau kustom, gunakan opsi **tipe uji** di bawah tipe informasi sensitif **klasifikasi**  >  .</span><span class="sxs-lookup"><span data-stu-id="93261-116">To test your data with a built-in or custom sensitive information type, use the **Test type** option under **Classifications** > **Sensitive info types**.</span></span> <span data-ttu-id="93261-117">Untuk informasi selengkapnya, lihat [menguji tipe informasi sensitif kustom](https://docs.microsoft.com/microsoft-365/compliance/create-a-custom-sensitive-information-type#create-custom-sensitive-information-types-in-the-security--compliance-center).</span><span class="sxs-lookup"><span data-stu-id="93261-117">For more information, see [Test custom sensitive information types](https://docs.microsoft.com/microsoft-365/compliance/create-a-custom-sensitive-information-type#create-custom-sensitive-information-types-in-the-security--compliance-center).</span></span>

 <span data-ttu-id="93261-118">**Melaporkan**</span><span class="sxs-lookup"><span data-stu-id="93261-118">**Reports**</span></span>
  
- <span data-ttu-id="93261-119">Dapatkan wawasan data sensitif dengan [laporan DLP.](https://docs.microsoft.com/microsoft-365/compliance/data-loss-prevention-policies#dlp-reports)</span><span class="sxs-lookup"><span data-stu-id="93261-119">Get sensitive data insights with [DLP Reports.](https://docs.microsoft.com/microsoft-365/compliance/data-loss-prevention-policies#dlp-reports)</span></span>

- <span data-ttu-id="93261-120">Lihat detail acara tertentu dengan [laporan insiden](https://docs.microsoft.com/microsoft-365/compliance/data-loss-prevention-policies#incident-reports).</span><span class="sxs-lookup"><span data-stu-id="93261-120">See specific details of the event with an [Incident Report](https://docs.microsoft.com/microsoft-365/compliance/data-loss-prevention-policies#incident-reports).</span></span>
