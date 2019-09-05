---
title: Mengaktifkan audit kotak pesan
ms.author: pebaum
author: pebaum
manager: mnirkhe
ms.date: 4/5/2018
ms.audience: Admin
ms.topic: article
ROBOTS: NOINDEX, NOFOLLOW
localization_priority: Normal
ms.collection: Adm_O365
ms.custom: ''
ms.assetid: 19997b0a-394f-4943-8908-c601696a332c
ms.openlocfilehash: 73517f46935a67a4a8a3e4770090ac897fe67979
ms.sourcegitcommit: a256e8680379c006287ae30996763051c4d9ff85
ms.translationtype: MT
ms.contentlocale: id-ID
ms.lasthandoff: 09/04/2019
ms.locfileid: "36736256"
---
# <a name="enable-mailbox-auditing"></a><span data-ttu-id="bc338-102">Mengaktifkan audit kotak pesan</span><span class="sxs-lookup"><span data-stu-id="bc338-102">Enable mailbox auditing</span></span>

<span data-ttu-id="bc338-103">Untuk mengaktifkan audit kotak surat untuk salah satu pengguna atau seluruh organisasi cmdlet berikut harus dijalankan dari remote Power Shell:</span><span class="sxs-lookup"><span data-stu-id="bc338-103">To enable Mailbox Auditing for either a single user or an entire organization the following cmdlets must be run from Remote Power Shell:</span></span>
  
 <span data-ttu-id="bc338-104">**Pengguna tunggal**</span><span class="sxs-lookup"><span data-stu-id="bc338-104">**Single User**</span></span>
  
<span data-ttu-id="bc338-105">Set-kotak surat-identitas "Jane Dow"-AuditEnabled $true</span><span class="sxs-lookup"><span data-stu-id="bc338-105">Set-Mailbox -Identity "Jane Dow" -AuditEnabled $true</span></span>
  
 <span data-ttu-id="bc338-106">**Organisasi**</span><span class="sxs-lookup"><span data-stu-id="bc338-106">**Organization**</span></span>
  
<span data-ttu-id="bc338-107">Get-kotak surat-ResultSize terbatas-filter {RecipientTypeDetails-EQ "UserMailbox"} | Set-kotak surat-AuditEnabled $true</span><span class="sxs-lookup"><span data-stu-id="bc338-107">Get-Mailbox -ResultSize Unlimited -Filter {RecipientTypeDetails -eq "UserMailbox"} | Set-Mailbox -AuditEnabled $true</span></span>
  
[<span data-ttu-id="bc338-108">Pelajari lebih lanjut</span><span class="sxs-lookup"><span data-stu-id="bc338-108">Learn more</span></span>](https://docs.microsoft.com/office365/securitycompliance/enable-mailbox-auditing)
  

