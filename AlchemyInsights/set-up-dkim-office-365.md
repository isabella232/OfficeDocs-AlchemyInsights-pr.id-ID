---
title: Pengaturan DKIM
ms.author: chrisda
author: chrisda
manager: dansimp
ms.audience: ITPro
ms.topic: article
ROBOTS: NOINDEX, NOFOLLOW
localization_priority: Normal
ms.custom: 1388
ms.assetid: ''
ms.openlocfilehash: d23a816d4eef065f800eaee60829d57dc1e7177f
ms.sourcegitcommit: 6bf1d945b4fd6a1fe37d00c5ea99adea7eef9910
ms.translationtype: MT
ms.contentlocale: id-ID
ms.lasthandoff: 04/21/2020
ms.locfileid: "43645675"
---
# <a name="setup-dkim"></a><span data-ttu-id="43d7b-102">Pengaturan DKIM</span><span class="sxs-lookup"><span data-stu-id="43d7b-102">Setup DKIM</span></span>

<span data-ttu-id="43d7b-103">Petunjuk lengkap untuk mengonfigurasi DKIM untuk domain kustom di Microsoft 365 ada [di sini](https://docs.microsoft.com/office365/SecurityCompliance/use-dkim-to-validate-outbound-email#what-you-need-to-do-to-manually-set-up-dkim-in-office-365).</span><span class="sxs-lookup"><span data-stu-id="43d7b-103">The complete instructions for configuring DKIM for custom domains in Microsoft 365 are [here](https://docs.microsoft.com/office365/SecurityCompliance/use-dkim-to-validate-outbound-email#what-you-need-to-do-to-manually-set-up-dkim-in-office-365).</span></span>

1. <span data-ttu-id="43d7b-104">Untuk **setiap** domain kustom, Anda perlu membuat **dua** data CNAME DKIM di layanan hosting DNS domain (biasanya, registrar domain).</span><span class="sxs-lookup"><span data-stu-id="43d7b-104">For **each** custom domain, you need to create **two** DKIM CNAME records at your domain's DNS hosting service (typically, the domain registrar).</span></span> <span data-ttu-id="43d7b-105">Misalnya, contoso.com dan fourthcoffee.com memerlukan empat data CNAME DKIM: dua untuk contoso.com dan dua untuk fourthcoffee.com.</span><span class="sxs-lookup"><span data-stu-id="43d7b-105">For example, contoso.com and fourthcoffee.com require four DKIM CNAME records: two for contoso.com and two for fourthcoffee.com.</span></span>

   <span data-ttu-id="43d7b-106">Data CNAME DKIM untuk **setiap** domain kustom menggunakan format berikut:</span><span class="sxs-lookup"><span data-stu-id="43d7b-106">The DKIM CNAME records for **each** custom domain use the following formats:</span></span>

   - <span data-ttu-id="43d7b-107">**Nama host**:`selector1._domainkey.<CustomDomain>`</span><span class="sxs-lookup"><span data-stu-id="43d7b-107">**Host name**: `selector1._domainkey.<CustomDomain>`</span></span>

     <span data-ttu-id="43d7b-108">**Poin ke alamat atau nilai**:`selector1-<DomainGUID>._domainkey.<InitialDomain>`</span><span class="sxs-lookup"><span data-stu-id="43d7b-108">**Points to address or value**: `selector1-<DomainGUID>._domainkey.<InitialDomain>`</span></span>

     <span data-ttu-id="43d7b-109">**TTL**: 3600</span><span class="sxs-lookup"><span data-stu-id="43d7b-109">**TTL**: 3600</span></span>

   - <span data-ttu-id="43d7b-110">**Nama host**:`selector2._domainkey.<CustomDomain>`</span><span class="sxs-lookup"><span data-stu-id="43d7b-110">**Host name**: `selector2._domainkey.<CustomDomain>`</span></span>

     <span data-ttu-id="43d7b-111">**Poin ke alamat atau nilai**:`selector2-<DomainGUID>._domainkey.<InitialDomain>`</span><span class="sxs-lookup"><span data-stu-id="43d7b-111">**Points to address or value**: `selector2-<DomainGUID>._domainkey.<InitialDomain>`</span></span>

     <span data-ttu-id="43d7b-112">**TTL**: 3600</span><span class="sxs-lookup"><span data-stu-id="43d7b-112">**TTL**: 3600</span></span>

   <span data-ttu-id="43d7b-113">\<DomainGUID\> adalah teks `.mail.protection.outlook.com` di sebelah kiri dalam data MX yang disesuaikan untuk domain kustom (misalnya, `contoso-com` untuk domain contoso.com).</span><span class="sxs-lookup"><span data-stu-id="43d7b-113">\<DomainGUID\> is the text to the left of `.mail.protection.outlook.com` in the customized MX record for the custom domain (for example, `contoso-com` for the domain contoso.com).</span></span> <span data-ttu-id="43d7b-114">\<InitialDomain\> adalah domain yang Anda gunakan ketika Anda mendaftar untuk Microsoft 365 (misalnya, contoso.onmicrosoft.com).</span><span class="sxs-lookup"><span data-stu-id="43d7b-114">\<InitialDomain\> is the domain you used when you signed up for Microsoft 365 (for example, contoso.onmicrosoft.com).</span></span>

2. <span data-ttu-id="43d7b-115">Setelah membuat data CNAME untuk domain kustom, selesaikan petunjuk berikut:</span><span class="sxs-lookup"><span data-stu-id="43d7b-115">After you've created the CNAME records for your custom domains, complete the following instructions:</span></span>

   <span data-ttu-id="43d7b-116">J.</span><span class="sxs-lookup"><span data-stu-id="43d7b-116">a.</span></span> <span data-ttu-id="43d7b-117">[masuk ke Microsoft 365](https://support.office.microsoft.com/article/e9eb7d51-5430-4929-91ab-6157c5a050b4) dengan akun kantor atau sekolah.</span><span class="sxs-lookup"><span data-stu-id="43d7b-117">[sign in to Microsoft 365](https://support.office.microsoft.com/article/e9eb7d51-5430-4929-91ab-6157c5a050b4) with your work or school account.</span></span>

   <span data-ttu-id="43d7b-118">B.</span><span class="sxs-lookup"><span data-stu-id="43d7b-118">b.</span></span> <span data-ttu-id="43d7b-119">Pilih ikon peluncur aplikasi di kiri atas dan pilih **admin**.</span><span class="sxs-lookup"><span data-stu-id="43d7b-119">Select the app launcher icon in the upper-left and choose **Admin**.</span></span>

   <span data-ttu-id="43d7b-120">C.</span><span class="sxs-lookup"><span data-stu-id="43d7b-120">c.</span></span> <span data-ttu-id="43d7b-121">Di navigasi kiri bawah, Perluas **admin** dan pilih **Exchange**.</span><span class="sxs-lookup"><span data-stu-id="43d7b-121">In the lower-left navigation, expand **Admin** and choose **Exchange**.</span></span>

   <span data-ttu-id="43d7b-122">D.</span><span class="sxs-lookup"><span data-stu-id="43d7b-122">d.</span></span> <span data-ttu-id="43d7b-123">Pergi ke **perlindungan** > **DKIM**.</span><span class="sxs-lookup"><span data-stu-id="43d7b-123">Go to **Protection** > **DKIM**.</span></span>

   <span data-ttu-id="43d7b-124">E.</span><span class="sxs-lookup"><span data-stu-id="43d7b-124">e.</span></span> <span data-ttu-id="43d7b-125">Pilih domain, lalu pilih **Aktifkan** untuk **menandatangani pesan untuk domain ini dengan tanda tangan DKIM**.</span><span class="sxs-lookup"><span data-stu-id="43d7b-125">Select the domain and then choose **Enable** for **Sign messages for this domain with DKIM signatures**.</span></span> <span data-ttu-id="43d7b-126">Ulangi langkah ini untuk setiap domain kustom.</span><span class="sxs-lookup"><span data-stu-id="43d7b-126">Repeat this step for each custom domain.</span></span>
