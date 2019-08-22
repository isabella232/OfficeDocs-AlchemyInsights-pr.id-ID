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
ms.openlocfilehash: 102c8025571f840cf64091d75295acec50661df2
ms.sourcegitcommit: 1d98db8acb9959aba3b5e308a567ade6b62da56c
ms.translationtype: MT
ms.contentlocale: id-ID
ms.lasthandoff: 08/22/2019
ms.locfileid: "36530287"
---
# <a name="dlp-not-working-as-expected"></a><span data-ttu-id="3a758-102">DLP tidak bekerja seperti yang diharapkan</span><span class="sxs-lookup"><span data-stu-id="3a758-102">DLP not working as expected</span></span>

<span data-ttu-id="3a758-103">Apakah Anda memiliki masalah dengan **Data Rugi Pencegahan (DLP)** di Office 365 tidak bekerja seperti yang diharapkan?</span><span class="sxs-lookup"><span data-stu-id="3a758-103">Are you having problems with **Data Loss Prevention (DLP)** in Office 365 not working as expected?</span></span> <span data-ttu-id="3a758-104">Jika demikian, pastikan bahwa Anda **DLP kebijakan** diatur dengan benar, dan bahwa data Anda berisi apa **kebijakan DLP** adalah mencari ketika itu sedang dievaluasi.</span><span class="sxs-lookup"><span data-stu-id="3a758-104">If so, make sure that your **DLP policy** is set up correctly, and that your data contains what the **DLP policy** is looking for when it is being evaluated.</span></span>
  
 <span data-ttu-id="3a758-105">**Menyiapkan DLP**</span><span class="sxs-lookup"><span data-stu-id="3a758-105">**Setting up DLP**</span></span>
  
<span data-ttu-id="3a758-106">DLP kebijakan memungkinkan Anda untuk mengidentifikasi dan melindungi informasi sensitif di organisasi Anda.</span><span class="sxs-lookup"><span data-stu-id="3a758-106">DLP policies allows you to identify and protect sensitive information in your organization.</span></span> <span data-ttu-id="3a758-107">Untuk setup DLP kebijakan, menggunakan informasi [di sini](https://docs.microsoft.com/office365/securitycompliance/prevent-data-loss#set-up-dlp).</span><span class="sxs-lookup"><span data-stu-id="3a758-107">To setup DLP policies, use the information [here](https://docs.microsoft.com/office365/securitycompliance/prevent-data-loss#set-up-dlp).</span></span>
  
 <span data-ttu-id="3a758-108">**Apa kebijakan DLP mencari**</span><span class="sxs-lookup"><span data-stu-id="3a758-108">**What DLP policies look for**</span></span>
  
<span data-ttu-id="3a758-109">Ketika menggunakan **jenis built-in informasi sensitif** di pusat kantor 365 keamanan dan kepatuhan, DLP kebijakan mencari pola-pola tertentu dan unsur-unsur ketika mendeteksi jenis sensitif.</span><span class="sxs-lookup"><span data-stu-id="3a758-109">When using the **built-in sensitive information types** in Office 365 Security and Compliance center, DLP policies look for specific patterns and elements when detecting these sensitive types.</span></span>
  
- <span data-ttu-id="3a758-110">**Jenis informasi sensitif built-in**</span><span class="sxs-lookup"><span data-stu-id="3a758-110">**Built-in Sensitive Information Types**</span></span>

    <span data-ttu-id="3a758-111">Untuk informasi tentang built-in tipe sensitif dan apa kebijakan DLP terlihat ketika mendeteksi jenis sensitif, lihat: [apa jenis informasi sensitif yang mencari](https://docs.microsoft.com/office365/securitycompliance/what-the-sensitive-information-types-look-for).</span><span class="sxs-lookup"><span data-stu-id="3a758-111">For information on the built-in Sensitive types and what a DLP policy looks for when detecting the Sensitive type, see: [What the sensitive information types look for](https://docs.microsoft.com/office365/securitycompliance/what-the-sensitive-information-types-look-for).</span></span>

- <span data-ttu-id="3a758-112">**Jenis informasi sensitif kustom**</span><span class="sxs-lookup"><span data-stu-id="3a758-112">**Custom Sensitive Information Types**</span></span>

    <span data-ttu-id="3a758-113">Jika Anda mencoba untuk menciptakan jenis informasi sensitif kustom, menggunakan artikel berikut untuk informasi tentang cara membuat custom jenis sensitif: [membuat sejenis kustom informasi sensitif](https://docs.microsoft.com/office365/securitycompliance/create-a-custom-sensitive-information-type).</span><span class="sxs-lookup"><span data-stu-id="3a758-113">If you are trying to create custom sensitive information types, use the following article for information on how to create a custom sensitive type: [Create a custom sensitive information type](https://docs.microsoft.com/office365/securitycompliance/create-a-custom-sensitive-information-type).</span></span>

<span data-ttu-id="3a758-114">**Menguji DLP kebijakan**</span><span class="sxs-lookup"><span data-stu-id="3a758-114">**Test a DLP policy**</span></span>

<span data-ttu-id="3a758-115">Untuk menguji data Anda dengan tipe built-in atau kustom informasi sensitif, menggunakan **jenis Test** opsi di bawah **klasifikasi** > **jenis sensitif info**.</span><span class="sxs-lookup"><span data-stu-id="3a758-115">To test your data with a built-in or custom sensitive information type, use the **Test type** option under **Classifications** > **Sensitive info types**.</span></span> <span data-ttu-id="3a758-116">Untuk selengkapnya, lihat [jenis informasi sensitif kustom tes](https://docs.microsoft.com/office365/securitycompliance/create-a-custom-sensitive-information-type#test-custom-sensitive-information-types-in-the-security--compliance-center).</span><span class="sxs-lookup"><span data-stu-id="3a758-116">For more information, see [Test custom sensitive information types](https://docs.microsoft.com/office365/securitycompliance/create-a-custom-sensitive-information-type#test-custom-sensitive-information-types-in-the-security--compliance-center).</span></span>

 <span data-ttu-id="3a758-117">**Laporan**</span><span class="sxs-lookup"><span data-stu-id="3a758-117">**Reports**</span></span>
  
- <span data-ttu-id="3a758-118">Mendapatkan data sensitif wawasan dengan [laporan DLP.](https://docs.microsoft.com/office365/securitycompliance/data-loss-prevention-policies#dlp-reports)</span><span class="sxs-lookup"><span data-stu-id="3a758-118">Get sensitive data insights with [DLP Reports.](https://docs.microsoft.com/office365/securitycompliance/data-loss-prevention-policies#dlp-reports)</span></span>

- <span data-ttu-id="3a758-119">Lihat rincian spesifik dari acara dengan [Insiden Report](https://docs.microsoft.com/office365/securitycompliance/data-loss-prevention-policies#incident-reports).</span><span class="sxs-lookup"><span data-stu-id="3a758-119">See specific details of the event with an [Incident Report](https://docs.microsoft.com/office365/securitycompliance/data-loss-prevention-policies#incident-reports).</span></span>
