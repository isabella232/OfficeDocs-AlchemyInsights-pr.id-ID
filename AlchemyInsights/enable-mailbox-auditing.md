---
title: Mengaktifkan audit kotak pesan
ms.author: pebaum
author: pebaum
manager: mnirkhe
ms.date: 04/21/2020
ms.audience: Admin
ms.topic: article
ROBOTS: NOINDEX, NOFOLLOW
localization_priority: Normal
ms.collection: Adm_O365
ms.custom: ''
ms.assetid: 19997b0a-394f-4943-8908-c601696a332c
ms.openlocfilehash: ae11d6be0789a5662d202b85268480a3d42922c4
ms.sourcegitcommit: 55eff703a17e500681d8fa6a87eb067019ade3cc
ms.translationtype: MT
ms.contentlocale: id-ID
ms.lasthandoff: 04/22/2020
ms.locfileid: "43703574"
---
# <a name="enable-mailbox-auditing"></a><span data-ttu-id="1643c-102">Mengaktifkan audit kotak pesan</span><span class="sxs-lookup"><span data-stu-id="1643c-102">Enable mailbox auditing</span></span>

<span data-ttu-id="1643c-103">Untuk mengaktifkan audit kotak surat untuk salah satu pengguna atau seluruh organisasi cmdlet berikut harus dijalankan dari remote Power Shell:</span><span class="sxs-lookup"><span data-stu-id="1643c-103">To enable Mailbox Auditing for either a single user or an entire organization the following cmdlets must be run from Remote Power Shell:</span></span>
  
 <span data-ttu-id="1643c-104">**Pengguna tunggal**</span><span class="sxs-lookup"><span data-stu-id="1643c-104">**Single User**</span></span>
  
<span data-ttu-id="1643c-105">Set-kotak surat-identitas "Jane Dow"-AuditEnabled $true</span><span class="sxs-lookup"><span data-stu-id="1643c-105">Set-Mailbox -Identity "Jane Dow" -AuditEnabled $true</span></span>
  
 <span data-ttu-id="1643c-106">**Organisasi**</span><span class="sxs-lookup"><span data-stu-id="1643c-106">**Organization**</span></span>
  
<span data-ttu-id="1643c-107">Get-kotak surat-ResultSize terbatas-filter {RecipientTypeDetails-EQ "UserMailbox"} | Set-kotak surat-AuditEnabled $true</span><span class="sxs-lookup"><span data-stu-id="1643c-107">Get-Mailbox -ResultSize Unlimited -Filter {RecipientTypeDetails -eq "UserMailbox"} | Set-Mailbox -AuditEnabled $true</span></span>
  
[<span data-ttu-id="1643c-108">Pelajari lebih lanjut</span><span class="sxs-lookup"><span data-stu-id="1643c-108">Learn more</span></span>](https://docs.microsoft.com/office365/securitycompliance/enable-mailbox-auditing)
  

