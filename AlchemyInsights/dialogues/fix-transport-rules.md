---
title: Memperbaiki aturan transpor
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
ms.openlocfilehash: 635009ed4b78d2b05b0eef1f3298765b10f86ede
ms.sourcegitcommit: bd6a9cb5d357baee5134c0dea430afc2a035c810
ms.translationtype: MT
ms.contentlocale: id-ID
ms.lasthandoff: 03/09/2021
ms.locfileid: "50694154"
---
# <a name="fix-transport-rules"></a><span data-ttu-id="02584-102">Memperbaiki aturan transpor</span><span class="sxs-lookup"><span data-stu-id="02584-102">Fix transport rules</span></span>

<span data-ttu-id="02584-103">Aturan aliran email kustom terpengaruh pesan ini.</span><span class="sxs-lookup"><span data-stu-id="02584-103">A custom mail flow rule affected this message.</span></span> <span data-ttu-id="02584-104">Untuk meninjau aturan yang tepat, lakukan hal berikut:</span><span class="sxs-lookup"><span data-stu-id="02584-104">To review the exact rule, do the following:</span></span>

1. <span data-ttu-id="02584-105">Dalam hasil pengiriman, di bawah **informasi tambahan**, perhatikan **GUID** atau **nama kebijakan**.</span><span class="sxs-lookup"><span data-stu-id="02584-105">In the submission results, under **Additional information**, note the **GUID** or the **Policy Name**.</span></span>
2. <span data-ttu-id="02584-106">Luncurkan Exchange Management Shell.</span><span class="sxs-lookup"><span data-stu-id="02584-106">Launch Exchange Management Shell.</span></span> <span data-ttu-id="02584-107">Untuk informasi selengkapnya, lihat [membuka Exchange Management Shell](https://go.microsoft.com/fwlink/?linkid=2101432).</span><span class="sxs-lookup"><span data-stu-id="02584-107">For more information, see [Open the Exchange Management Shell](https://go.microsoft.com/fwlink/?linkid=2101432).</span></span>
3. <span data-ttu-id="02584-108">Jalankan perintah ini (menggunakan GUID dari pengiriman Anda):  **Get-TransportRule-identitas "GUID" | FL \* Deskripsi**\*</span><span class="sxs-lookup"><span data-stu-id="02584-108">Run this command (using the GUID from your submission):  **Get-TransportRule -identity "GUID" | fl \* Description**\*</span></span>
4. <span data-ttu-id="02584-109">Tinjau Deskripsi untuk melihat kondisi yang dikonfigurasi yang mempengaruhi pesan tersebut.</span><span class="sxs-lookup"><span data-stu-id="02584-109">Review the description to see the configured conditions that affected the message.</span></span>

<span data-ttu-id="02584-110">Untuk mempelajari selengkapnya, lihat [Get-TransportRule](https://go.microsoft.com/fwlink/?linkid=2101523).</span><span class="sxs-lookup"><span data-stu-id="02584-110">To learn more, see [Get-TransportRule](https://go.microsoft.com/fwlink/?linkid=2101523).</span></span>
