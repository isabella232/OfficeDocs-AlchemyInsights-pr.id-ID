---
title: DLP tidak bekerja seperti yang diharapkan
ms.author: deniseb
author: denisebmsft
manager: laurawi
ms.date: 1/9/2019
ms.audience: ITPro
ms.topic: article
ms.prod: office-online-server
ROBOTS: NOINDEX, NOFOLLOW
localization_priority: Normal
ms.custom:
- "1241"
- "3200001"
ms.assetid: f6fcf5ad-55a1-4f25-af27-1f7c1ce06409
ms.openlocfilehash: 574a8a43d8264e98c6af2bfeb1bb472475e6e334
ms.sourcegitcommit: 940169c0edf638b5086d70cc275049f01dcff3cf
ms.translationtype: MT
ms.contentlocale: id-ID
ms.lasthandoff: 04/08/2020
ms.locfileid: "42977441"
---
# <a name="dlp-not-working-as-expected"></a><span data-ttu-id="5f58e-102">DLP tidak bekerja seperti yang diharapkan</span><span class="sxs-lookup"><span data-stu-id="5f58e-102">DLP not working as expected</span></span>

<span data-ttu-id="5f58e-103">**Penting**: Selama masa-masa yang berat ini, kami mengambil langkah untuk memastikan bahwa SharePoint Online dan layanan OneDrive tetap memiliki ketersediaan yang tinggi. Silakan kunjungi [Penyesuaian Fitur Sementara SharePoint Online](https://aka.ms/ODSPAdjustments) untuk informasi selengkapnya.</span><span class="sxs-lookup"><span data-stu-id="5f58e-103">**Important**: During these unprecedented times, we are taking steps to ensure that SharePoint Online and OneDrive services remain highly available – Please visit [SharePoint Online Temporary Feature Adjustments](https://aka.ms/ODSPAdjustments) for more information.</span></span>

 <span data-ttu-id="5f58e-104">**Menyiapkan DLP**</span><span class="sxs-lookup"><span data-stu-id="5f58e-104">**Setting up DLP**</span></span>

<span data-ttu-id="5f58e-105">Apakah Anda mengalami masalah dengan **pencegahan kehilangan data (DLP)** di Office 365 tidak bekerja seperti yang diharapkan?</span><span class="sxs-lookup"><span data-stu-id="5f58e-105">Are you having problems with **Data Loss Prevention (DLP)** in Office 365 not working as expected?</span></span> <span data-ttu-id="5f58e-106">Jika demikian, pastikan bahwa Anda **DLP kebijakan** diatur dengan benar, dan bahwa data Anda berisi apa **kebijakan DLP** sedang mencari ketika sedang dievaluasi.</span><span class="sxs-lookup"><span data-stu-id="5f58e-106">If so, make sure that your **DLP policy** is set up correctly, and that your data contains what the **DLP policy** is looking for when it is being evaluated.</span></span>
  
<span data-ttu-id="5f58e-107">Kebijakan DLP memungkinkan Anda mengidentifikasi dan melindungi informasi sensitif di organisasi Anda.</span><span class="sxs-lookup"><span data-stu-id="5f58e-107">DLP policies allows you to identify and protect sensitive information in your organization.</span></span> <span data-ttu-id="5f58e-108">Untuk setup DLP kebijakan, gunakan informasi [di sini](https://docs.microsoft.com/office365/securitycompliance/prevent-data-loss#set-up-dlp).</span><span class="sxs-lookup"><span data-stu-id="5f58e-108">To setup DLP policies, use the information [here](https://docs.microsoft.com/office365/securitycompliance/prevent-data-loss#set-up-dlp).</span></span>
  
 <span data-ttu-id="5f58e-109">**Apa yang dicari oleh kebijakan DLP**</span><span class="sxs-lookup"><span data-stu-id="5f58e-109">**What DLP policies look for**</span></span>
  
<span data-ttu-id="5f58e-110">Saat menggunakan **jenis informasi sensitif internal** di pusat keamanan dan kepatuhan Office 365, kebijakan DLP mencari pola dan elemen tertentu saat mendeteksi jenis sensitif ini.</span><span class="sxs-lookup"><span data-stu-id="5f58e-110">When using the **built-in sensitive information types** in Office 365 Security and Compliance center, DLP policies look for specific patterns and elements when detecting these sensitive types.</span></span>
  
- <span data-ttu-id="5f58e-111">**Jenis informasi sensitif internal**</span><span class="sxs-lookup"><span data-stu-id="5f58e-111">**Built-in Sensitive Information Types**</span></span>

    <span data-ttu-id="5f58e-112">Untuk informasi tentang jenis sensitif internal dan apa yang dicari oleh kebijakan DLP saat mendeteksi jenis sensitif, lihat: [apa jenis informasi sensitif Cari](https://docs.microsoft.com/office365/securitycompliance/what-the-sensitive-information-types-look-for).</span><span class="sxs-lookup"><span data-stu-id="5f58e-112">For information on the built-in Sensitive types and what a DLP policy looks for when detecting the Sensitive type, see: [What the sensitive information types look for](https://docs.microsoft.com/office365/securitycompliance/what-the-sensitive-information-types-look-for).</span></span>

- <span data-ttu-id="5f58e-113">**Jenis informasi sensitif khusus**</span><span class="sxs-lookup"><span data-stu-id="5f58e-113">**Custom Sensitive Information Types**</span></span>

    <span data-ttu-id="5f58e-114">Jika Anda mencoba untuk membuat jenis informasi sensitif kustom, gunakan artikel berikut ini untuk informasi tentang cara membuat jenis sensitif kustom: [membuat jenis informasi sensitif kustom](https://docs.microsoft.com/office365/securitycompliance/create-a-custom-sensitive-information-type).</span><span class="sxs-lookup"><span data-stu-id="5f58e-114">If you are trying to create custom sensitive information types, use the following article for information on how to create a custom sensitive type: [Create a custom sensitive information type](https://docs.microsoft.com/office365/securitycompliance/create-a-custom-sensitive-information-type).</span></span>

<span data-ttu-id="5f58e-115">**Menguji kebijakan DLP**</span><span class="sxs-lookup"><span data-stu-id="5f58e-115">**Test a DLP policy**</span></span>

<span data-ttu-id="5f58e-116">Untuk menguji data Anda dengan jenis informasi sensitif internal atau kustom, gunakan opsi **jenis uji** di bawah **klasifikasi** > **jenis Info sensitif**.</span><span class="sxs-lookup"><span data-stu-id="5f58e-116">To test your data with a built-in or custom sensitive information type, use the **Test type** option under **Classifications** > **Sensitive info types**.</span></span> <span data-ttu-id="5f58e-117">Untuk informasi selengkapnya, lihat [menguji jenis informasi sensitif kustom](https://docs.microsoft.com/office365/securitycompliance/create-a-custom-sensitive-information-type#test-custom-sensitive-information-types-in-the-security--compliance-center).</span><span class="sxs-lookup"><span data-stu-id="5f58e-117">For more information, see [Test custom sensitive information types](https://docs.microsoft.com/office365/securitycompliance/create-a-custom-sensitive-information-type#test-custom-sensitive-information-types-in-the-security--compliance-center).</span></span>

 <span data-ttu-id="5f58e-118">**Laporan**</span><span class="sxs-lookup"><span data-stu-id="5f58e-118">**Reports**</span></span>
  
- <span data-ttu-id="5f58e-119">Dapatkan wawasan data sensitif dengan [laporan DLP.](https://docs.microsoft.com/office365/securitycompliance/data-loss-prevention-policies#dlp-reports)</span><span class="sxs-lookup"><span data-stu-id="5f58e-119">Get sensitive data insights with [DLP Reports.](https://docs.microsoft.com/office365/securitycompliance/data-loss-prevention-policies#dlp-reports)</span></span>

- <span data-ttu-id="5f58e-120">Lihat detail spesifik acara dengan [laporan insiden](https://docs.microsoft.com/office365/securitycompliance/data-loss-prevention-policies#incident-reports).</span><span class="sxs-lookup"><span data-stu-id="5f58e-120">See specific details of the event with an [Incident Report](https://docs.microsoft.com/office365/securitycompliance/data-loss-prevention-policies#incident-reports).</span></span>
