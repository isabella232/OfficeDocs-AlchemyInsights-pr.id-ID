---
title: Memperbaiki masalah penyiapan DKIM
ms.author: chrisda
author: chrisda
manager: dansimp
ms.date: 04/21/2020
ms.audience: ITPro
ms.topic: article
ROBOTS: NOINDEX, NOFOLLOW
localization_priority: Normal
ms.custom: 1389
ms.assetid: ''
ms.openlocfilehash: 8195b0e3fada6da033b2d95b1fc6600e7fa3341e
ms.sourcegitcommit: bc7d6f4f3c9f7060d073f5130e1ec856e248d020
ms.translationtype: MT
ms.contentlocale: id-ID
ms.lasthandoff: 06/02/2020
ms.locfileid: "44506777"
---
# <a name="fix-dkim-setup-issues"></a><span data-ttu-id="68f1f-102">Memperbaiki masalah penyiapan DKIM</span><span class="sxs-lookup"><span data-stu-id="68f1f-102">Fix DKIM setup issues</span></span>

<span data-ttu-id="68f1f-103">Jika Anda mengalami masalah saat mengaktifkan DKIM untuk domain kustom, gunakan langkah berikut:</span><span class="sxs-lookup"><span data-stu-id="68f1f-103">If you experience issues enabling DKIM for your custom domain, use the following steps:</span></span>

- <span data-ttu-id="68f1f-104">Sebagian besar masalah penyiapan DKIM terkait dengan data DNS yang salah.</span><span class="sxs-lookup"><span data-stu-id="68f1f-104">Most DKIM setup issues are related to incorrect DNS records.</span></span> <span data-ttu-id="68f1f-105">Verifikasi data CNAME DKIM (**bukan** data TXT) diformat dengan benar.</span><span class="sxs-lookup"><span data-stu-id="68f1f-105">Verify the DKIM CNAME record (**not** a TXT record) is formatted correctly.</span></span> <span data-ttu-id="68f1f-106">Untuk informasi lebih lanjut, lihat [topik](https://docs.microsoft.com/microsoft-365/security/office-365-security/use-dkim-to-validate-outbound-email#steps-you-need-to-do-to-manually-set-up-dkim)ini.</span><span class="sxs-lookup"><span data-stu-id="68f1f-106">For more information, see this [topic](https://docs.microsoft.com/microsoft-365/security/office-365-security/use-dkim-to-validate-outbound-email#steps-you-need-to-do-to-manually-set-up-dkim).</span></span>

- <span data-ttu-id="68f1f-107">Setelah membuat atau memperbarui data DNS DKIM di layanan hosting DNS untuk domain (biasanya, registrar domain), tunggu hingga data DNS diterapkan.</span><span class="sxs-lookup"><span data-stu-id="68f1f-107">After you create or update your DKIM DNS records at the DNS hosting service for your domain (typically, your domain registrar), wait for the DNS records to propagate.</span></span>

- <span data-ttu-id="68f1f-108">Jika Anda tidak dapat membuat data DNS DKIM di pusat admin, Anda dapat mengganti \<CustomDomain\> dengan domain kustom (misalnya, contoso.com) dan menjalankan perintah ini di [Exchange Online PowerShell](https://docs.microsoft.com/powershell/exchange/exchange-online/connect-to-exchange-online-powershell/connect-to-exchange-online-powershell): `New-DkimSigningConfig -DomainName <CustomDomain> -Enabled $true` .</span><span class="sxs-lookup"><span data-stu-id="68f1f-108">If you can't create the DKIM DNS records in the admin center, you can replace \<CustomDomain\> with your custom domain (for example, contoso.com) and run this command in [Exchange Online PowerShell](https://docs.microsoft.com/powershell/exchange/exchange-online/connect-to-exchange-online-powershell/connect-to-exchange-online-powershell): `New-DkimSigningConfig -DomainName <CustomDomain> -Enabled $true`.</span></span>
