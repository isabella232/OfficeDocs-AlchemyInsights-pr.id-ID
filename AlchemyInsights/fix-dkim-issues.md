---
title: Memperbaiki masalah pengaturan DKIM
ms.author: chrisda
author: chrisda
manager: dansimp
ms.date: ''
ms.audience: ITPro
ms.topic: article
ROBOTS: NOINDEX, NOFOLLOW
localization_priority: Normal
ms.custom: 1389
ms.assetid: ''
ms.openlocfilehash: 4d6dadbcbf71fe6e9ea56d6a82a7d8ababdd38ef
ms.sourcegitcommit: 4b7e478ce700c0b781efec3857ac4dce5bdf00c6
ms.translationtype: MT
ms.contentlocale: id-ID
ms.lasthandoff: 06/07/2019
ms.locfileid: "34765153"
---
# <a name="fix-dkim-setup-issues"></a><span data-ttu-id="7de87-102">Memperbaiki masalah pengaturan DKIM</span><span class="sxs-lookup"><span data-stu-id="7de87-102">Fix DKIM setup issues</span></span>

<span data-ttu-id="7de87-103">Jika Anda mengalami masalah yang memungkinkan DKIM untuk domain kustom, gunakan langkah-langkah berikut:</span><span class="sxs-lookup"><span data-stu-id="7de87-103">If you experience issues enabling DKIM for your custom domain, use the following steps:</span></span>

- <span data-ttu-id="7de87-104">Sebagian besar masalah pengaturan DKIM yang terkait dengan data DNS yang salah.</span><span class="sxs-lookup"><span data-stu-id="7de87-104">Most DKIM setup issues are related to incorrect DNS records.</span></span> <span data-ttu-id="7de87-105">Pastikan DKIM data CNAME (**bukan** data TXT) diformat dengan benar.</span><span class="sxs-lookup"><span data-stu-id="7de87-105">Verify the DKIM CNAME record (**not** a TXT record) is formatted correctly.</span></span> <span data-ttu-id="7de87-106">Untuk selengkapnya, lihat [topik](https://docs.microsoft.com/office365/SecurityCompliance/use-dkim-to-validate-outbound-email#what-you-need-to-do-to-manually-set-up-dkim-in-office-365)ini.</span><span class="sxs-lookup"><span data-stu-id="7de87-106">For more information, see this [topic](https://docs.microsoft.com/office365/SecurityCompliance/use-dkim-to-validate-outbound-email#what-you-need-to-do-to-manually-set-up-dkim-in-office-365).</span></span>

- <span data-ttu-id="7de87-107">Setelah membuat atau memperbarui data DKIM dengan DNS pada layanan hosting DNS untuk domain Anda (biasanya, registrar domain), menunggu data DNS untuk menyebarkan.</span><span class="sxs-lookup"><span data-stu-id="7de87-107">After you create or update your DKIM DNS records at the DNS hosting service for your domain (typically, your domain registrar), wait for the DNS records to propagate.</span></span>

- <span data-ttu-id="7de87-108">Jika Anda tidak dapat membuat data DKIM DNS di pusat admin, Anda dapat mengganti \<CustomDomain\> dengan domain kustom (misalnya, contoso.com) dan menjalankan perintah ini di [PowerShell Online asing](https://docs.microsoft.com/powershell/exchange/exchange-online/connect-to-exchange-online-powershell/connect-to-exchange-online-powershell): `New-DkimSigningConfig -DomainName <CustomDomain> -Enabled $true`.</span><span class="sxs-lookup"><span data-stu-id="7de87-108">If you can't create the DKIM DNS records in the admin center, you can replace \<CustomDomain\> with your custom domain (for example, contoso.com) and run this command in [Exchange Online PowerShell](https://docs.microsoft.com/powershell/exchange/exchange-online/connect-to-exchange-online-powershell/connect-to-exchange-online-powershell): `New-DkimSigningConfig -DomainName <CustomDomain> -Enabled $true`.</span></span>
