---
title: Menggunakan PowerShell untuk berbagi kebijakan dan relasi organisasi
ms.author: pebaum
author: pebaum
manager: mnirkhe
ms.audience: Admin
ms.topic: article
ROBOTS: NOINDEX, NOFOLLOW
localization_priority: Priority
ms.collection: Adm_O365
ms.custom:
- "3800014"
- "898"
ms.openlocfilehash: 717cdd6827e243ac6bf375209a911937c97088d2
ms.sourcegitcommit: 722e9a0ed058cb1eab2dd053be2418b60f7d4aac
ms.translationtype: MT
ms.contentlocale: id-ID
ms.lasthandoff: 06/23/2020
ms.locfileid: "44862089"
---
# <a name="use-powershell-for-sharing-policies-and-organization-relationships"></a><span data-ttu-id="b0ba2-102">Menggunakan PowerShell untuk berbagi kebijakan dan relasi organisasi</span><span class="sxs-lookup"><span data-stu-id="b0ba2-102">Use PowerShell for Sharing policies and Organization relationships</span></span>


<span data-ttu-id="b0ba2-103">Untuk hubungan organisasi silakan Tinjau informasi rinci sintaks dan parameter untuk: [Get-FederationInformation](https://docs.microsoft.com/powershell/module/exchange/get-federationinformation), [New-OrganizationRelationship](https://docs.microsoft.com/powershell/module/exchange/new-organizationrelationship), [set-OrganizationRelationship](https://docs.microsoft.com/powershell/module/exchange/set-organizationrelationship) dan [Hapus-OrganizationRelationship](https://docs.microsoft.com/powershell/module/exchange/remove-organizationrelationship).</span><span class="sxs-lookup"><span data-stu-id="b0ba2-103">For Organization relationships please review the detailed syntax and parameter information for : [Get-FederationInformation](https://docs.microsoft.com/powershell/module/exchange/get-federationinformation), [New-OrganizationRelationship](https://docs.microsoft.com/powershell/module/exchange/new-organizationrelationship), [Set-OrganizationRelationship](https://docs.microsoft.com/powershell/module/exchange/set-organizationrelationship)  AND  [Remove-OrganizationRelationship](https://docs.microsoft.com/powershell/module/exchange/remove-organizationrelationship).</span></span>

<span data-ttu-id="b0ba2-104">Untuk membuat kebijakan berbagi menggunakan [baru-SharingPolicy](https://docs.microsoft.com/powershell/module/exchange/new-sharingpolicy).</span><span class="sxs-lookup"><span data-stu-id="b0ba2-104">To create sharing policy use [New-SharingPolicy](https://docs.microsoft.com/powershell/module/exchange/new-sharingpolicy).</span></span> <span data-ttu-id="b0ba2-105">Untuk [menerapkan kebijakan berbagi ke kotak pesan atau pengguna](https://docs.microsoft.com/exchange/sharing/sharing-policies/apply-a-sharing-policy%23use-exchange-online-powershell-to-apply-a-sharing-policy-to-one-or-more-mailboxes) , Anda harus menggunakan kombinasi [Set-Mailbox](https://docs.microsoft.com/powershell/module/exchange/set-mailbox) dan [Get-kotak surat](https://docs.microsoft.com/powershell/module/exchange/get-mailbox) dengan kebijakan yang baru dibuat.</span><span class="sxs-lookup"><span data-stu-id="b0ba2-105">To  [apply a sharing policy to a mailbox or user](https://docs.microsoft.com/exchange/sharing/sharing-policies/apply-a-sharing-policy%23use-exchange-online-powershell-to-apply-a-sharing-policy-to-one-or-more-mailboxes)  you need to use a combination of  [Set-Mailbox](https://docs.microsoft.com/powershell/module/exchange/set-mailbox) and [Get-Mailbox](https://docs.microsoft.com/powershell/module/exchange/get-mailbox) with the newly created policy.</span></span> <span data-ttu-id="b0ba2-106">Untuk [mengubah, menonaktifkan atau menghapus kebijakan berbagi](https://docs.microsoft.com/exchange/sharing/sharing-policies/modify-a-sharing-policy) Anda perlu menggunakan [set-sharingpolicy](https://docs.microsoft.com/powershell/module/exchange/set-sharingpolicy) dan [Hapus-sharingpolicy](https://docs.microsoft.com/powershell/module/exchange/remove-sharingpolicy).</span><span class="sxs-lookup"><span data-stu-id="b0ba2-106">To  [modify, disable or remove a sharing policy](https://docs.microsoft.com/exchange/sharing/sharing-policies/modify-a-sharing-policy)  you need to use  [Set-SharingPolicy](https://docs.microsoft.com/powershell/module/exchange/set-sharingpolicy) and [Remove-SharingPolicy](https://docs.microsoft.com/powershell/module/exchange/remove-sharingpolicy).</span></span>

<span data-ttu-id="b0ba2-107">**Untuk pemahaman penuh tentang topik ini silahkan baca:**</span><span class="sxs-lookup"><span data-stu-id="b0ba2-107">**For full understanding of this topic please read:**</span></span>

[<span data-ttu-id="b0ba2-108">Berbagi di Exchange Online</span><span class="sxs-lookup"><span data-stu-id="b0ba2-108">Sharing in Exchange Online</span></span>](https://docs.microsoft.com/exchange/sharing/sharing)