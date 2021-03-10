---
title: Memperbaiki kebijakan koneksi
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
ms.openlocfilehash: 0b6286350e706e493f6d30b7978aacedc02daff5
ms.sourcegitcommit: bd6a9cb5d357baee5134c0dea430afc2a035c810
ms.translationtype: MT
ms.contentlocale: id-ID
ms.lasthandoff: 03/09/2021
ms.locfileid: "50694168"
---
# <a name="fix-connection-policy"></a><span data-ttu-id="3ef93-102">Memperbaiki kebijakan koneksi</span><span class="sxs-lookup"><span data-stu-id="3ef93-102">Fix connection policy</span></span>

<span data-ttu-id="3ef93-103">Email ditandai aman dan dikirim ke kotak masuk pengguna karena alamat IP pengirim ditandai aman di kebijakan filter koneksi.</span><span class="sxs-lookup"><span data-stu-id="3ef93-103">The email was marked safe and delivered to the user's inbox because the sending IP address was marked safe in the Connection Filter policy.</span></span> <span data-ttu-id="3ef93-104">Untuk meninjau kebijakan, lakukan hal berikut:</span><span class="sxs-lookup"><span data-stu-id="3ef93-104">To review the policy, do the following:</span></span>

1. <span data-ttu-id="3ef93-105">Masuk ke [pusat kepatuhan & keamanan Office 365](https://go.microsoft.com/fwlink/p/?linkid=2077143), lalu masuk ke kebijakan **manajemen ancaman**  >    >  [anti-spam](https://go.microsoft.com/fwlink/?linkid=2101518).</span><span class="sxs-lookup"><span data-stu-id="3ef93-105">Go to the [Office 365 Security & Compliance Center](https://go.microsoft.com/fwlink/p/?linkid=2077143), and then go to **Threat management** > **Policy** > [Anti-spam](https://go.microsoft.com/fwlink/?linkid=2101518).</span></span>
2. <span data-ttu-id="3ef93-106">Pada tab **kustom** , pilih **kebijakan filter koneksi**, lalu pilih **Edit kebijakan**.</span><span class="sxs-lookup"><span data-stu-id="3ef93-106">On the **Custom** tab, select the **Connection filter policy**, and then select **Edit policy**.</span></span>
3. <span data-ttu-id="3ef93-107">Tinjau daftar **Perbolehkan IP** .</span><span class="sxs-lookup"><span data-stu-id="3ef93-107">Review the **IP Allow** list.</span></span> <span data-ttu-id="3ef93-108">Lihat apakah **daftar aman** diaktifkan.</span><span class="sxs-lookup"><span data-stu-id="3ef93-108">See if **Safe list** is enabled.</span></span>

    > [!NOTE]
    > <span data-ttu-id="3ef93-109">Microsoft berlangganan ke sumber pihak ketiga pengirim tepercaya.</span><span class="sxs-lookup"><span data-stu-id="3ef93-109">Microsoft subscribes to third-party sources of trusted senders.</span></span> <span data-ttu-id="3ef93-110">Jika **daftar aman** diaktifkan, pengirim tepercaya ini tidak secara keliru ditandai sebagai spam.</span><span class="sxs-lookup"><span data-stu-id="3ef93-110">If **Safe list** is enabled, these trusted senders aren't mistakenly marked as spam.</span></span> <span data-ttu-id="3ef93-111">Saya merekomendasikan memilih opsi ini, karena akan mengurangi jumlah positif palsu (baik email yang diklasifikasikan sebagai spam) yang Anda terima.</span><span class="sxs-lookup"><span data-stu-id="3ef93-111">I recommend selecting this option, because it will reduce the number of false positives (good mail that's classified as spam) that you receive.</span></span>
