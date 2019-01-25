---
title: Mengaktifkan kotak pesan audit
ms.author: pebaum
author: pebaum
manager: mnirkhe
ms.date: 4/5/2018
ms.audience: Admin
ms.topic: article
ROBOTS: NOINDEX, NOFOLLOW
localization_priority: Priority
ms.collection: Adm_O365
ms.custom: Adm_O365
ms.assetid: 19997b0a-394f-4943-8908-c601696a332c
ms.openlocfilehash: bd94ec10f9df2e72ec6e3d8552d2eb80212a9d78
ms.sourcegitcommit: e2864efcfb493b6e46b662b746661a61232bdba7
ms.translationtype: MT
ms.contentlocale: id-ID
ms.lasthandoff: 01/24/2019
ms.locfileid: "29500285"
---
# <a name="enable-mailbox-auditing"></a><span data-ttu-id="14769-102">Mengaktifkan kotak pesan audit</span><span class="sxs-lookup"><span data-stu-id="14769-102">Enable mailbox auditing</span></span>

<span data-ttu-id="14769-103">Aktifkan kotak pesan audit untuk pengguna tunggal atau seluruh organisasi cmdlet berikut harus dijalankan dari Remote Power Shell:</span><span class="sxs-lookup"><span data-stu-id="14769-103">To enable Mailbox Auditing for either a single user or an entire organization the following cmdlets must be run from Remote Power Shell:</span></span>
  
 <span data-ttu-id="14769-104">**Satu pengguna**</span><span class="sxs-lookup"><span data-stu-id="14769-104">**Single User**</span></span>
  
<span data-ttu-id="14769-105">Set-kotak surat - identitas "Jane Dow" - AuditEnabled $true</span><span class="sxs-lookup"><span data-stu-id="14769-105">Set-Mailbox -Identity "Jane Dow" -AuditEnabled $true</span></span>
  
 <span data-ttu-id="14769-106">Organization</span><span class="sxs-lookup"><span data-stu-id="14769-106">**Organization**</span></span>
  
<span data-ttu-id="14769-107">Get-kotak surat - ResultSize Unlimited - Filter {RecipientTypeDetails - persamaan "UserMailbox"} | Set-kotak surat - AuditEnabled $true</span><span class="sxs-lookup"><span data-stu-id="14769-107">Get-Mailbox -ResultSize Unlimited -Filter {RecipientTypeDetails -eq "UserMailbox"} | Set-Mailbox -AuditEnabled $true</span></span>
  
[<span data-ttu-id="14769-108">Pelajari lebih lanjut</span><span class="sxs-lookup"><span data-stu-id="14769-108">Learn more</span></span>](https://support.office.com/article/aaca8987-5b62-458b-9882-c28476a66918)
  

