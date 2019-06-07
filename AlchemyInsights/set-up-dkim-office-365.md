---
title: Setup DKIM di Office 365
ms.author: chrisda
author: chrisda
manager: dansimp
ms.date: ''
ms.audience: ITPro
ms.topic: article
ROBOTS: NOINDEX, NOFOLLOW
localization_priority: Normal
ms.custom: 1388
ms.assetid: ''
ms.openlocfilehash: 0f81fe02135f3d0901ffe5a26d7aa3dad70c3770
ms.sourcegitcommit: 4b7e478ce700c0b781efec3857ac4dce5bdf00c6
ms.translationtype: MT
ms.contentlocale: id-ID
ms.lasthandoff: 06/07/2019
ms.locfileid: "34765165"
---
# <a name="setup-dkim-in-office-365"></a><span data-ttu-id="867fd-102">Setup DKIM di Office 365</span><span class="sxs-lookup"><span data-stu-id="867fd-102">Setup DKIM in Office 365</span></span>

<span data-ttu-id="867fd-103">Petunjuk lengkap untuk mengkonfigurasi DKIM untuk custom domain di Office 365 [di sini](https://docs.microsoft.com/office365/SecurityCompliance/use-dkim-to-validate-outbound-email#what-you-need-to-do-to-manually-set-up-dkim-in-office-365).</span><span class="sxs-lookup"><span data-stu-id="867fd-103">The complete instructions for configuring DKIM for custom domains in Office 365 are [here](https://docs.microsoft.com/office365/SecurityCompliance/use-dkim-to-validate-outbound-email#what-you-need-to-do-to-manually-set-up-dkim-in-office-365).</span></span>

1. <span data-ttu-id="867fd-104">Untuk **setiap** domain kustom, Anda perlu membuat **dua** DKIM CNAME records di layanan hosting DNS domain Anda (biasanya, registrar domain).</span><span class="sxs-lookup"><span data-stu-id="867fd-104">For **each** custom domain, you need to create **two** DKIM CNAME records at your domain's DNS hosting service (typically, the domain registrar).</span></span> <span data-ttu-id="867fd-105">Misalnya, contoso.com dan fourthcoffee.com memerlukan empat DKIM CNAME records: dua untuk contoso.com dan dua untuk fourthcoffee.com.</span><span class="sxs-lookup"><span data-stu-id="867fd-105">For example, contoso.com and fourthcoffee.com require four DKIM CNAME records: two for contoso.com and two for fourthcoffee.com.</span></span>

   <span data-ttu-id="867fd-106">DKIM CNAME records untuk **setiap** domain kustom menggunakan format berikut:</span><span class="sxs-lookup"><span data-stu-id="867fd-106">The DKIM CNAME records for **each** custom domain use the following formats:</span></span>

   - <span data-ttu-id="867fd-107">**Nama host**:`selector1._domainkey.<CustomDomain>`</span><span class="sxs-lookup"><span data-stu-id="867fd-107">**Host name**: `selector1._domainkey.<CustomDomain>`</span></span>

     <span data-ttu-id="867fd-108">**Poin ke alamat atau nilai**:`selector1-<DomainGUID>._domainkey.<InitialDomain>`</span><span class="sxs-lookup"><span data-stu-id="867fd-108">**Points to address or value**: `selector1-<DomainGUID>._domainkey.<InitialDomain>`</span></span>

     <span data-ttu-id="867fd-109">**TTL**: 3600</span><span class="sxs-lookup"><span data-stu-id="867fd-109">**TTL**: 3600</span></span>

   - <span data-ttu-id="867fd-110">**Nama host**:`selector2._domainkey.<CustomDomain>`</span><span class="sxs-lookup"><span data-stu-id="867fd-110">**Host name**: `selector2._domainkey.<CustomDomain>`</span></span>

     <span data-ttu-id="867fd-111">**Poin ke alamat atau nilai**:`selector2-<DomainGUID>._domainkey.<InitialDomain>`</span><span class="sxs-lookup"><span data-stu-id="867fd-111">**Points to address or value**: `selector2-<DomainGUID>._domainkey.<InitialDomain>`</span></span>

     <span data-ttu-id="867fd-112">**TTL**: 3600</span><span class="sxs-lookup"><span data-stu-id="867fd-112">**TTL**: 3600</span></span>

   <span data-ttu-id="867fd-113">\<DomainGUID\> adalah teks di sebelah kiri `.mail.protection.outlook.com` dalam data MX disesuaikan untuk custom domain (misalnya, `contoso-com` untuk domain contoso.com).</span><span class="sxs-lookup"><span data-stu-id="867fd-113">\<DomainGUID\> is the text to the left of `.mail.protection.outlook.com` in the customized MX record for the custom domain (for example, `contoso-com` for the domain contoso.com).</span></span> <span data-ttu-id="867fd-114">\<InitialDomain\> adalah domain yang digunakan saat mendaftar ke Office 365 (misalnya, contoso.onmicrosoft.com).</span><span class="sxs-lookup"><span data-stu-id="867fd-114">\<InitialDomain\> is the domain you used when you signed up for Office 365 (for example, contoso.onmicrosoft.com).</span></span>

2. <span data-ttu-id="867fd-115">Setelah membuat data CNAME untuk domain kustom, lengkap petunjuk berikut:</span><span class="sxs-lookup"><span data-stu-id="867fd-115">After you've created the CNAME records for your custom domains, complete the following instructions:</span></span>

   <span data-ttu-id="867fd-116">a.</span><span class="sxs-lookup"><span data-stu-id="867fd-116">a.</span></span> <span data-ttu-id="867fd-117">[Masuk ke kantor 365](https://support.office.microsoft.com/article/e9eb7d51-5430-4929-91ab-6157c5a050b4) dengan akun kantor atau sekolah.</span><span class="sxs-lookup"><span data-stu-id="867fd-117">[Sign in to Office 365](https://support.office.microsoft.com/article/e9eb7d51-5430-4929-91ab-6157c5a050b4) with your work or school account.</span></span>

   <span data-ttu-id="867fd-118">b.</span><span class="sxs-lookup"><span data-stu-id="867fd-118">b.</span></span> <span data-ttu-id="867fd-119">Pilih ikon peluncur app di kiri dan pilih **Admin**.</span><span class="sxs-lookup"><span data-stu-id="867fd-119">Select the app launcher icon in the upper-left and choose **Admin**.</span></span>

   <span data-ttu-id="867fd-120">c.</span><span class="sxs-lookup"><span data-stu-id="867fd-120">c.</span></span> <span data-ttu-id="867fd-121">Pada navigasi kiri, memperluas **Admin** dan memilih **asing**.</span><span class="sxs-lookup"><span data-stu-id="867fd-121">In the lower-left navigation, expand **Admin** and choose **Exchange**.</span></span>

   <span data-ttu-id="867fd-122">d.</span><span class="sxs-lookup"><span data-stu-id="867fd-122">d.</span></span> <span data-ttu-id="867fd-123">Pergi ke **perlindungan** > **DKIM**.</span><span class="sxs-lookup"><span data-stu-id="867fd-123">Go to **Protection** > **DKIM**.</span></span>

   <span data-ttu-id="867fd-124">e.</span><span class="sxs-lookup"><span data-stu-id="867fd-124">e.</span></span> <span data-ttu-id="867fd-125">Pilih domain, dan kemudian memilih **mengaktifkan** **tanda**pesan untuk domain ini dengan DKIM tanda tangan.</span><span class="sxs-lookup"><span data-stu-id="867fd-125">Select the domain and then choose **Enable** for **Sign messages for this domain with DKIM signatures**.</span></span> <span data-ttu-id="867fd-126">Ulangi langkah ini untuk setiap domain kustom.</span><span class="sxs-lookup"><span data-stu-id="867fd-126">Repeat this step for each custom domain.</span></span>
