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
ms.openlocfilehash: 0acaed476dbd06bc933bf466f9bf6116413a44bb
ms.sourcegitcommit: bc7d6f4f3c9f7060d073f5130e1ec856e248d020
ms.translationtype: MT
ms.contentlocale: id-ID
ms.lasthandoff: 06/02/2020
ms.locfileid: "44509387"
---
# <a name="setup-dkim"></a><span data-ttu-id="9f940-102">Pengaturan DKIM</span><span class="sxs-lookup"><span data-stu-id="9f940-102">Setup DKIM</span></span>

<span data-ttu-id="9f940-103">Petunjuk lengkap untuk mengonfigurasi DKIM untuk domain kustom di Microsoft 365 ada [di sini](https://docs.microsoft.com/microsoft-365/security/office-365-security/use-dkim-to-validate-outbound-email#steps-you-need-to-do-to-manually-set-up-dkim).</span><span class="sxs-lookup"><span data-stu-id="9f940-103">The complete instructions for configuring DKIM for custom domains in Microsoft 365 are [here](https://docs.microsoft.com/microsoft-365/security/office-365-security/use-dkim-to-validate-outbound-email#steps-you-need-to-do-to-manually-set-up-dkim).</span></span>

1. <span data-ttu-id="9f940-104">Untuk **setiap** domain kustom, Anda perlu membuat **dua** data CNAME DKIM di layanan hosting DNS domain (biasanya, registrar domain).</span><span class="sxs-lookup"><span data-stu-id="9f940-104">For **each** custom domain, you need to create **two** DKIM CNAME records at your domain's DNS hosting service (typically, the domain registrar).</span></span> <span data-ttu-id="9f940-105">Misalnya, contoso.com dan fourthcoffee.com memerlukan empat data CNAME DKIM: dua untuk contoso.com dan dua untuk fourthcoffee.com.</span><span class="sxs-lookup"><span data-stu-id="9f940-105">For example, contoso.com and fourthcoffee.com require four DKIM CNAME records: two for contoso.com and two for fourthcoffee.com.</span></span>

   <span data-ttu-id="9f940-106">Data CNAME DKIM untuk **setiap** domain kustom menggunakan format berikut:</span><span class="sxs-lookup"><span data-stu-id="9f940-106">The DKIM CNAME records for **each** custom domain use the following formats:</span></span>

   - <span data-ttu-id="9f940-107">**Nama host**:`selector1._domainkey.<CustomDomain>`</span><span class="sxs-lookup"><span data-stu-id="9f940-107">**Host name**: `selector1._domainkey.<CustomDomain>`</span></span>

     <span data-ttu-id="9f940-108">**Poin ke alamat atau nilai**:`selector1-<DomainGUID>._domainkey.<InitialDomain>`</span><span class="sxs-lookup"><span data-stu-id="9f940-108">**Points to address or value**: `selector1-<DomainGUID>._domainkey.<InitialDomain>`</span></span>

     <span data-ttu-id="9f940-109">**TTL**: 3600</span><span class="sxs-lookup"><span data-stu-id="9f940-109">**TTL**: 3600</span></span>

   - <span data-ttu-id="9f940-110">**Nama host**:`selector2._domainkey.<CustomDomain>`</span><span class="sxs-lookup"><span data-stu-id="9f940-110">**Host name**: `selector2._domainkey.<CustomDomain>`</span></span>

     <span data-ttu-id="9f940-111">**Poin ke alamat atau nilai**:`selector2-<DomainGUID>._domainkey.<InitialDomain>`</span><span class="sxs-lookup"><span data-stu-id="9f940-111">**Points to address or value**: `selector2-<DomainGUID>._domainkey.<InitialDomain>`</span></span>

     <span data-ttu-id="9f940-112">**TTL**: 3600</span><span class="sxs-lookup"><span data-stu-id="9f940-112">**TTL**: 3600</span></span>

   <span data-ttu-id="9f940-113">\<DomainGUID\>adalah teks di sebelah kiri `.mail.protection.outlook.com` dalam data MX yang disesuaikan untuk domain kustom (misalnya, `contoso-com` untuk domain contoso.com).</span><span class="sxs-lookup"><span data-stu-id="9f940-113">\<DomainGUID\> is the text to the left of `.mail.protection.outlook.com` in the customized MX record for the custom domain (for example, `contoso-com` for the domain contoso.com).</span></span> <span data-ttu-id="9f940-114">\<InitialDomain\>adalah domain yang Anda gunakan saat mendaftar untuk Microsoft 365 (misalnya, contoso.onmicrosoft.com).</span><span class="sxs-lookup"><span data-stu-id="9f940-114">\<InitialDomain\> is the domain you used when you signed up for Microsoft 365 (for example, contoso.onmicrosoft.com).</span></span>

2. <span data-ttu-id="9f940-115">Setelah membuat data CNAME untuk domain kustom, selesaikan petunjuk berikut:</span><span class="sxs-lookup"><span data-stu-id="9f940-115">After you've created the CNAME records for your custom domains, complete the following instructions:</span></span>

   <span data-ttu-id="9f940-116">J.</span><span class="sxs-lookup"><span data-stu-id="9f940-116">a.</span></span> <span data-ttu-id="9f940-117">[masuk ke Microsoft 365](https://support.office.microsoft.com/article/e9eb7d51-5430-4929-91ab-6157c5a050b4) dengan akun kantor atau sekolah.</span><span class="sxs-lookup"><span data-stu-id="9f940-117">[sign in to Microsoft 365](https://support.office.microsoft.com/article/e9eb7d51-5430-4929-91ab-6157c5a050b4) with your work or school account.</span></span>

   <span data-ttu-id="9f940-118">B.</span><span class="sxs-lookup"><span data-stu-id="9f940-118">b.</span></span> <span data-ttu-id="9f940-119">Pilih ikon peluncur aplikasi di kiri atas dan pilih **admin**.</span><span class="sxs-lookup"><span data-stu-id="9f940-119">Select the app launcher icon in the upper-left and choose **Admin**.</span></span>

   <span data-ttu-id="9f940-120">C.</span><span class="sxs-lookup"><span data-stu-id="9f940-120">c.</span></span> <span data-ttu-id="9f940-121">Di navigasi kiri bawah, Perluas **admin** dan pilih **Exchange**.</span><span class="sxs-lookup"><span data-stu-id="9f940-121">In the lower-left navigation, expand **Admin** and choose **Exchange**.</span></span>

   <span data-ttu-id="9f940-122">D.</span><span class="sxs-lookup"><span data-stu-id="9f940-122">d.</span></span> <span data-ttu-id="9f940-123">Pergi ke **perlindungan**  >  **DKIM**.</span><span class="sxs-lookup"><span data-stu-id="9f940-123">Go to **Protection** > **DKIM**.</span></span>

   <span data-ttu-id="9f940-124">E.</span><span class="sxs-lookup"><span data-stu-id="9f940-124">e.</span></span> <span data-ttu-id="9f940-125">Pilih domain, lalu pilih **Aktifkan** untuk **menandatangani pesan untuk domain ini dengan tanda tangan DKIM**.</span><span class="sxs-lookup"><span data-stu-id="9f940-125">Select the domain and then choose **Enable** for **Sign messages for this domain with DKIM signatures**.</span></span> <span data-ttu-id="9f940-126">Ulangi langkah ini untuk setiap domain kustom.</span><span class="sxs-lookup"><span data-stu-id="9f940-126">Repeat this step for each custom domain.</span></span>
