---
title: Penyetelan DKIM
ms.author: chrisda
author: chrisda
manager: dansimp
ms.audience: ITPro
ms.topic: article
ms.service: o365-administration
ROBOTS: NOINDEX, NOFOLLOW
localization_priority: Normal
ms.custom: 1388
ms.assetid: ''
ms.openlocfilehash: b34bfdafcab6229a4dd2e9d9f23103fa13556482
ms.sourcegitcommit: c6692ce0fa1358ec3529e59ca0ecdfdea4cdc759
ms.translationtype: MT
ms.contentlocale: id-ID
ms.lasthandoff: 09/15/2020
ms.locfileid: "47808710"
---
# <a name="setup-dkim"></a><span data-ttu-id="52689-102">Penyetelan DKIM</span><span class="sxs-lookup"><span data-stu-id="52689-102">Setup DKIM</span></span>

<span data-ttu-id="52689-103">Instruksi lengkap untuk mengonfigurasi DKIM untuk domain kustom di Microsoft 365 ada [di sini](https://docs.microsoft.com/microsoft-365/security/office-365-security/use-dkim-to-validate-outbound-email#steps-you-need-to-do-to-manually-set-up-dkim).</span><span class="sxs-lookup"><span data-stu-id="52689-103">The complete instructions for configuring DKIM for custom domains in Microsoft 365 are [here](https://docs.microsoft.com/microsoft-365/security/office-365-security/use-dkim-to-validate-outbound-email#steps-you-need-to-do-to-manually-set-up-dkim).</span></span>

1. <span data-ttu-id="52689-104">Untuk **setiap** domain kustom, Anda perlu membuat **dua** catatan CNAME DKIM di layanan hosting DNS domain Anda (biasanya, pencatat domain).</span><span class="sxs-lookup"><span data-stu-id="52689-104">For **each** custom domain, you need to create **two** DKIM CNAME records at your domain's DNS hosting service (typically, the domain registrar).</span></span> <span data-ttu-id="52689-105">Misalnya, contoso.com dan fourthcoffee.com memerlukan empat catatan CNAME DKIM: dua untuk contoso.com dan dua untuk fourthcoffee.com.</span><span class="sxs-lookup"><span data-stu-id="52689-105">For example, contoso.com and fourthcoffee.com require four DKIM CNAME records: two for contoso.com and two for fourthcoffee.com.</span></span>

   <span data-ttu-id="52689-106">Catatan CNAME DKIM untuk **setiap** domain kustom menggunakan format berikut:</span><span class="sxs-lookup"><span data-stu-id="52689-106">The DKIM CNAME records for **each** custom domain use the following formats:</span></span>

   - <span data-ttu-id="52689-107">**Nama host**: `selector1._domainkey.<CustomDomain>`</span><span class="sxs-lookup"><span data-stu-id="52689-107">**Host name**: `selector1._domainkey.<CustomDomain>`</span></span>

     <span data-ttu-id="52689-108">**Mengarahkan ke alamat atau nilai**: `selector1-<DomainGUID>._domainkey.<InitialDomain>`</span><span class="sxs-lookup"><span data-stu-id="52689-108">**Points to address or value**: `selector1-<DomainGUID>._domainkey.<InitialDomain>`</span></span>

     <span data-ttu-id="52689-109">**TTL**: 3600</span><span class="sxs-lookup"><span data-stu-id="52689-109">**TTL**: 3600</span></span>

   - <span data-ttu-id="52689-110">**Nama host**: `selector2._domainkey.<CustomDomain>`</span><span class="sxs-lookup"><span data-stu-id="52689-110">**Host name**: `selector2._domainkey.<CustomDomain>`</span></span>

     <span data-ttu-id="52689-111">**Mengarahkan ke alamat atau nilai**: `selector2-<DomainGUID>._domainkey.<InitialDomain>`</span><span class="sxs-lookup"><span data-stu-id="52689-111">**Points to address or value**: `selector2-<DomainGUID>._domainkey.<InitialDomain>`</span></span>

     <span data-ttu-id="52689-112">**TTL**: 3600</span><span class="sxs-lookup"><span data-stu-id="52689-112">**TTL**: 3600</span></span>

   <span data-ttu-id="52689-113">\<DomainGUID\> adalah teks di sebelah kiri `.mail.protection.outlook.com` catatan MX yang dikustomisasi untuk domain kustom (misalnya, `contoso-com` untuk domain contoso.com).</span><span class="sxs-lookup"><span data-stu-id="52689-113">\<DomainGUID\> is the text to the left of `.mail.protection.outlook.com` in the customized MX record for the custom domain (for example, `contoso-com` for the domain contoso.com).</span></span> <span data-ttu-id="52689-114">\<InitialDomain\> adalah domain yang Anda gunakan saat mendaftar untuk Microsoft 365 (misalnya, contoso.onmicrosoft.com).</span><span class="sxs-lookup"><span data-stu-id="52689-114">\<InitialDomain\> is the domain you used when you signed up for Microsoft 365 (for example, contoso.onmicrosoft.com).</span></span>

2. <span data-ttu-id="52689-115">Setelah Anda membuat catatan CNAME untuk domain kustom Anda, selesaikan instruksi berikut:</span><span class="sxs-lookup"><span data-stu-id="52689-115">After you've created the CNAME records for your custom domains, complete the following instructions:</span></span>

   <span data-ttu-id="52689-116">untuk.</span><span class="sxs-lookup"><span data-stu-id="52689-116">a.</span></span> <span data-ttu-id="52689-117">[masuk ke Microsoft 365](https://support.office.microsoft.com/article/e9eb7d51-5430-4929-91ab-6157c5a050b4) dengan akun kantor atau sekolah Anda.</span><span class="sxs-lookup"><span data-stu-id="52689-117">[sign in to Microsoft 365](https://support.office.microsoft.com/article/e9eb7d51-5430-4929-91ab-6157c5a050b4) with your work or school account.</span></span>

   <span data-ttu-id="52689-118">b.</span><span class="sxs-lookup"><span data-stu-id="52689-118">b.</span></span> <span data-ttu-id="52689-119">Pilih ikon peluncur aplikasi di kiri atas dan pilih **admin**.</span><span class="sxs-lookup"><span data-stu-id="52689-119">Select the app launcher icon in the upper-left and choose **Admin**.</span></span>

   <span data-ttu-id="52689-120">'s.</span><span class="sxs-lookup"><span data-stu-id="52689-120">c.</span></span> <span data-ttu-id="52689-121">Di navigasi kiri bawah, Perluas **admin** dan pilih **Exchange**.</span><span class="sxs-lookup"><span data-stu-id="52689-121">In the lower-left navigation, expand **Admin** and choose **Exchange**.</span></span>

   <span data-ttu-id="52689-122">dih.</span><span class="sxs-lookup"><span data-stu-id="52689-122">d.</span></span> <span data-ttu-id="52689-123">Buka **proteksi**  >  **DKIM**.</span><span class="sxs-lookup"><span data-stu-id="52689-123">Go to **Protection** > **DKIM**.</span></span>

   <span data-ttu-id="52689-124">e.</span><span class="sxs-lookup"><span data-stu-id="52689-124">e.</span></span> <span data-ttu-id="52689-125">Pilih domain, lalu pilih **Aktifkan** untuk **tanda tangani pesan untuk domain ini dengan tanda tangan DKIM**.</span><span class="sxs-lookup"><span data-stu-id="52689-125">Select the domain and then choose **Enable** for **Sign messages for this domain with DKIM signatures**.</span></span> <span data-ttu-id="52689-126">Ulangi langkah ini untuk setiap domain kustom.</span><span class="sxs-lookup"><span data-stu-id="52689-126">Repeat this step for each custom domain.</span></span>
