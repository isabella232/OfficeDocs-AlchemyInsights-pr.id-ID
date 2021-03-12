---
title: Memperbaiki kebijakan penyewa (menimpa tindakan)
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
ms.openlocfilehash: bc7ad8acd86c9d5b2f99ffdc6fe8a8b53e1fcb8b
ms.sourcegitcommit: 6312ee31561db36104f32282d019d069ede69174
ms.translationtype: MT
ms.contentlocale: id-ID
ms.lasthandoff: 03/11/2021
ms.locfileid: "50745881"
---
# <a name="fix-tenant-policy-action-override"></a><span data-ttu-id="b451a-102">Memperbaiki kebijakan penyewa (menimpa tindakan)</span><span class="sxs-lookup"><span data-stu-id="b451a-102">Fix Tenant policy (action override)</span></span>

<span data-ttu-id="b451a-103">Kebijakan anti spam di penyewa Anda mempengaruhi pesan ini.</span><span class="sxs-lookup"><span data-stu-id="b451a-103">An anti-spam policy in your tenant affected this message.</span></span> <span data-ttu-id="b451a-104">Untuk meninjau kebijakan, lakukan hal berikut:</span><span class="sxs-lookup"><span data-stu-id="b451a-104">To review the policy, do the following:</span></span>

1. <span data-ttu-id="b451a-105">Masuk ke [pusat kepatuhan & keamanan Office 365](https://go.microsoft.com/fwlink/p/?linkid=2077143), lalu masuk ke kebijakan **manajemen ancaman**  >    >  [anti-spam](https://go.microsoft.com/fwlink/?linkid=2101518).</span><span class="sxs-lookup"><span data-stu-id="b451a-105">Go to the [Office 365 Security & Compliance Center](https://go.microsoft.com/fwlink/p/?linkid=2077143), and then go to **Threat management** > **Policy** > [Anti-spam](https://go.microsoft.com/fwlink/?linkid=2101518).</span></span>
2. <span data-ttu-id="b451a-106">Periksa untuk melihat apakah **sumber kebijakan** menunjukkan hal berikut:  **Add-Xheader/Modifysubject/redirect/Delete/No Action/Bcc message**</span><span class="sxs-lookup"><span data-stu-id="b451a-106">Check to see if **Policy source** indicates the following:  **Add-Xheader/ModifySubject/Redirect/Delete/No action/ BCC message**</span></span>

    <span data-ttu-id="b451a-107">Jika demikian, pada tab **kustom** , periksa pengaturan kebijakan yang mempengaruhi pesan.</span><span class="sxs-lookup"><span data-stu-id="b451a-107">If so, on the **Custom** tab, check the settings of the policy that affected the message.</span></span> <span data-ttu-id="b451a-108">Ada kemungkinan bahwa **pengaturan standar** yang diterapkan ke semua pelanggan Exchange Online Protection mempengaruhi pesan tersebut.</span><span class="sxs-lookup"><span data-stu-id="b451a-108">It's possible that the **Standard settings** applied to all Exchange Online Protection customers affected the message.</span></span>

<span data-ttu-id="b451a-109">Untuk informasi selengkapnya tentang mengonfigurasi kebijakan filter spam, lihat [mengonfigurasi kebijakan filter spam Anda](https://go.microsoft.com/fwlink/?linkid=2101431).</span><span class="sxs-lookup"><span data-stu-id="b451a-109">For more information on configuring spam filter policies, see [Configure your spam filter policies](https://go.microsoft.com/fwlink/?linkid=2101431).</span></span>
