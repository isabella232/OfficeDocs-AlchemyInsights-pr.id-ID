---
title: Memperbaiki masalah penyetelan DKIM
ms.author: chrisda
author: chrisda
manager: dansimp
ms.date: 04/21/2020
ms.audience: ITPro
ms.topic: article
ms.service: o365-administration
ROBOTS: NOINDEX, NOFOLLOW
localization_priority: Normal
ms.custom: 1389
ms.assetid: ''
ms.openlocfilehash: 35e8023d26fe26211e27521ceb8751d2d7fc7a21
ms.sourcegitcommit: c6692ce0fa1358ec3529e59ca0ecdfdea4cdc759
ms.translationtype: MT
ms.contentlocale: id-ID
ms.lasthandoff: 09/14/2020
ms.locfileid: "47744953"
---
# <a name="fix-dkim-setup-issues"></a><span data-ttu-id="05090-102">Memperbaiki masalah penyetelan DKIM</span><span class="sxs-lookup"><span data-stu-id="05090-102">Fix DKIM setup issues</span></span>

<span data-ttu-id="05090-103">Jika Anda mengalami masalah dalam mengaktifkan DKIM untuk domain kustom Anda, gunakan langkah-langkah berikut:</span><span class="sxs-lookup"><span data-stu-id="05090-103">If you experience issues enabling DKIM for your custom domain, use the following steps:</span></span>

- <span data-ttu-id="05090-104">Sebagian besar masalah penyetelan DKIM terkait dengan catatan DNS yang salah.</span><span class="sxs-lookup"><span data-stu-id="05090-104">Most DKIM setup issues are related to incorrect DNS records.</span></span> <span data-ttu-id="05090-105">Verifikasi catatan CNAME DKIM (**bukan** rekaman txt) diformat dengan benar.</span><span class="sxs-lookup"><span data-stu-id="05090-105">Verify the DKIM CNAME record (**not** a TXT record) is formatted correctly.</span></span> <span data-ttu-id="05090-106">Untuk informasi selengkapnya, lihat [topik](https://docs.microsoft.com/microsoft-365/security/office-365-security/use-dkim-to-validate-outbound-email#steps-you-need-to-do-to-manually-set-up-dkim)ini.</span><span class="sxs-lookup"><span data-stu-id="05090-106">For more information, see this [topic](https://docs.microsoft.com/microsoft-365/security/office-365-security/use-dkim-to-validate-outbound-email#steps-you-need-to-do-to-manually-set-up-dkim).</span></span>

- <span data-ttu-id="05090-107">Setelah Anda membuat atau memperbarui catatan DNS DKIM Anda di layanan hosting DNS untuk domain Anda (biasanya, pencatat domain Anda), tunggulah catatan DNS untuk disebarkan.</span><span class="sxs-lookup"><span data-stu-id="05090-107">After you create or update your DKIM DNS records at the DNS hosting service for your domain (typically, your domain registrar), wait for the DNS records to propagate.</span></span>

- <span data-ttu-id="05090-108">Jika Anda tidak dapat membuat catatan DNS DKIM di pusat admin, Anda bisa mengganti \<CustomDomain\> dengan domain kustom Anda (misalnya, contoso.com) dan menjalankan perintah ini di [Exchange Online PowerShell](https://docs.microsoft.com/powershell/exchange/exchange-online/connect-to-exchange-online-powershell/connect-to-exchange-online-powershell): `New-DkimSigningConfig -DomainName <CustomDomain> -Enabled $true` .</span><span class="sxs-lookup"><span data-stu-id="05090-108">If you can't create the DKIM DNS records in the admin center, you can replace \<CustomDomain\> with your custom domain (for example, contoso.com) and run this command in [Exchange Online PowerShell](https://docs.microsoft.com/powershell/exchange/exchange-online/connect-to-exchange-online-powershell/connect-to-exchange-online-powershell): `New-DkimSigningConfig -DomainName <CustomDomain> -Enabled $true`.</span></span>
