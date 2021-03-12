---
title: Memperbaiki pengaturan kebijakan pengguna/kotak surat
ms.author: v-jmathew
author: v-jmathew
manager: dansimp
audience: Admin
ms.topic: article
ms.service: o365-administration
ROBOTS: NOINDEX, NOFOLLOW
localization_priority: Normal
ms.collection: Adm_O365
ms.custom:
- "9000760"
- "7391"
ms.openlocfilehash: ca998c453fcb0905b122436f0eea384a9b8a9992
ms.sourcegitcommit: 6312ee31561db36104f32282d019d069ede69174
ms.translationtype: MT
ms.contentlocale: id-ID
ms.lasthandoff: 03/11/2021
ms.locfileid: "50746730"
---
# <a name="fix-user-policymailbox-settings"></a><span data-ttu-id="5d602-102">Memperbaiki pengaturan kebijakan pengguna/kotak surat</span><span class="sxs-lookup"><span data-stu-id="5d602-102">Fix user policy/mailbox settings</span></span>

<span data-ttu-id="5d602-103">Pengaturan email sampah pada kotak surat terpengaruh pesan ini.</span><span class="sxs-lookup"><span data-stu-id="5d602-103">The junk mail settings on the mailbox affected this message.</span></span> <span data-ttu-id="5d602-104">Untuk meninjau pengaturan, lakukan hal berikut:</span><span class="sxs-lookup"><span data-stu-id="5d602-104">To review the settings, do the following:</span></span>

1. <span data-ttu-id="5d602-105">Luncurkan Exchange Management Shell.</span><span class="sxs-lookup"><span data-stu-id="5d602-105">Launch Exchange Management Shell.</span></span> <span data-ttu-id="5d602-106">Untuk informasi selengkapnya, lihat [membuka Exchange Management Shell](https://go.microsoft.com/fwlink/?linkid=2101432).</span><span class="sxs-lookup"><span data-stu-id="5d602-106">For more information, see [Open the Exchange Management Shell](https://go.microsoft.com/fwlink/?linkid=2101432).</span></span>
2. <span data-ttu-id="5d602-107">Jalankan perintah ini (menggunakan alamat email pengguna):  **Get-mailboxjunkmailconfiguration-Identity "user@domain.com"**</span><span class="sxs-lookup"><span data-stu-id="5d602-107">Run this command (using the user's email address):  **get-mailboxjunkmailconfiguration -identity "user@domain.com"**</span></span>
3. <span data-ttu-id="5d602-108">Periksa apakah alamat email pengirim adalah bagian dari **Trustedsendersanddomains** atau **blockedsendersanddomains**.</span><span class="sxs-lookup"><span data-stu-id="5d602-108">Check if the sender's email address is part of **TrustedSendersAndDomains** or **BlockedSendersAndDomains**.</span></span> <span data-ttu-id="5d602-109">Jika alamat email berada dalam salah satu daftar, Anda mungkin harus menghapusnya.</span><span class="sxs-lookup"><span data-stu-id="5d602-109">If the email address is in one of the lists, you may have to remove it.</span></span> <span data-ttu-id="5d602-110">Untuk mempelajari selengkapnya, lihat [set-MailboxJunkEmailConfiguration](https://go.microsoft.com/fwlink/?linkid=2101047).</span><span class="sxs-lookup"><span data-stu-id="5d602-110">To learn more, see [Set-MailboxJunkEmailConfiguration](https://go.microsoft.com/fwlink/?linkid=2101047).</span></span>
