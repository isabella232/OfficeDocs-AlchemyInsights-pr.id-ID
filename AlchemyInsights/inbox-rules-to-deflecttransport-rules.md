---
title: 929 aturan kotak masuk untuk aturan deflectTransport
ms.author: chrisda
author: chrisda
manager: dansimp
ms.date: 04/21/2020
ms.audience: ITPro
ms.topic: article
ROBOTS: NOINDEX, NOFOLLOW
localization_priority: Normal
ms.custom:
- "929"
- "1800021"
ms.assetid: 9733ef4e-db8d-4345-a072-c251480875a1
ms.openlocfilehash: 6b6e64c0332a579e8f6132b08f2f89b15eb4de27
ms.sourcegitcommit: 55eff703a17e500681d8fa6a87eb067019ade3cc
ms.translationtype: MT
ms.contentlocale: id-ID
ms.lasthandoff: 04/22/2020
ms.locfileid: "43724595"
---
# <a name="mail-flow-rules-also-known-as-transport-rules"></a><span data-ttu-id="22e55-102">Aturan aliran e-mail (juga dikenal sebagai aturan transport)</span><span class="sxs-lookup"><span data-stu-id="22e55-102">Mail flow rules (also known as transport rules)</span></span>

- <span data-ttu-id="22e55-103">Ikhtisar umum aturan aliran surat: [aturan aliran surat (aturan transpor) di Exchange Online](https://technet.microsoft.com/library/jj919238.aspx)</span><span class="sxs-lookup"><span data-stu-id="22e55-103">General overview of mail flow rules: [Mail flow rules (transport rules) in Exchange Online](https://technet.microsoft.com/library/jj919238.aspx)</span></span>

- <span data-ttu-id="22e55-104">Aturan alur e-mail penyiapan: [prosedur aturan alur e-mail di Exchange Online](https://technet.microsoft.com/library/dn600436.aspx)</span><span class="sxs-lookup"><span data-stu-id="22e55-104">Setup mail flow rules: [Mail flow rule procedures in Exchange Online](https://technet.microsoft.com/library/dn600436.aspx)</span></span>

- <span data-ttu-id="22e55-105">Membuat, mengubah, dan menghapus aturan aliran e-mail: [mengelola aturan aliran e-mail](https://technet.microsoft.com/library/jj657505.aspx)</span><span class="sxs-lookup"><span data-stu-id="22e55-105">Create, modify, and delete mail flow rules: [Manage mail flow rules](https://technet.microsoft.com/library/jj657505.aspx)</span></span>

<span data-ttu-id="22e55-106">Anda juga dapat mengelola aturan aliran e-mail di Exchange Online PowerShell.</span><span class="sxs-lookup"><span data-stu-id="22e55-106">You can also manage mail flow rules in Exchange Online PowerShell.</span></span> <span data-ttu-id="22e55-107">Untuk informasi selengkapnya, lihat [Get-TransportRule](https://docs.microsoft.com/powershell/module/exchange/policy-and-compliance/get-transportrule) (tampilan), [baru-TransportRule](https://docs.microsoft.com/powershell/module/exchange/policy-and-compliance/new-transportrule) (membuat), [Hapus-TransportRule](https://docs.microsoft.com/powershell/module/exchange/policy-and-compliance/remove-transportrule) (Hapus), [set-TransportRule](https://docs.microsoft.com/powershell/module/exchange/policy-and-compliance/set-transportrule) (mengubah ada), [menonaktifkan-TransportRule](https://docs.microsoft.com/powershell/module/exchange/policy-and-compliance/disable-transportrule) (menonaktifkan ada), dan [mengaktifkan-TransportRule](https://docs.microsoft.com/powershell/module/exchange/policy-and-compliance/enable-transportrule) (mengaktifkan ada).</span><span class="sxs-lookup"><span data-stu-id="22e55-107">For more information, see [Get-TransportRule](https://docs.microsoft.com/powershell/module/exchange/policy-and-compliance/get-transportrule) (view), [New-TransportRule](https://docs.microsoft.com/powershell/module/exchange/policy-and-compliance/new-transportrule) (create), [Remove-TransportRule](https://docs.microsoft.com/powershell/module/exchange/policy-and-compliance/remove-transportrule) (delete), [Set-TransportRule](https://docs.microsoft.com/powershell/module/exchange/policy-and-compliance/set-transportrule) (modify existing), [Disable-TransportRule](https://docs.microsoft.com/powershell/module/exchange/policy-and-compliance/disable-transportrule) (disable existing), and [Enable-TransportRule](https://docs.microsoft.com/powershell/module/exchange/policy-and-compliance/enable-transportrule) (enable existing).</span></span>

<span data-ttu-id="22e55-108">Cmdlet aturan aliran surat tambahan: [Get-TransportRuleAction](https://docs.microsoft.com/powershell/module/exchange/policy-and-compliance/get-transportruleaction) (daftar tindakan yang tersedia), [Get-TransportRulePredicate](https://docs.microsoft.com/powershell/module/exchange/policy-and-compliance/get-transportrulepredicate) (daftar tersedia kondisi dan pengecualian), [transportrulecollection ekspor](https://docs.microsoft.com/powershell/module/exchange/policy-and-compliance/export-transportrulecollection) (ekspor aturan), dan [transportrulecollection impor](https://docs.microsoft.com/powershell/module/exchange/policy-and-compliance/import-transportrulecollection) (impor aturan).</span><span class="sxs-lookup"><span data-stu-id="22e55-108">Additional mail flow rule cmdlets: [Get-TransportRuleAction](https://docs.microsoft.com/powershell/module/exchange/policy-and-compliance/get-transportruleaction) (list available actions), [Get-TransportRulePredicate](https://docs.microsoft.com/powershell/module/exchange/policy-and-compliance/get-transportrulepredicate) (list available conditions and exceptions), [Export-TransportRuleCollection](https://docs.microsoft.com/powershell/module/exchange/policy-and-compliance/export-transportrulecollection) (export rules), and [Import-TransportRuleCollection](https://docs.microsoft.com/powershell/module/exchange/policy-and-compliance/import-transportrulecollection) (import rules).</span></span>
