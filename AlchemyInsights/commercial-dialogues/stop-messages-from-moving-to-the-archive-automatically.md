---
title: Menghentikan pesan agar tidak berpindah ke arsip secara otomatis
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
- "3100008"
- "7217"
ms.openlocfilehash: 2cb3e29dfd4f422e946b7887d4d44f373ff03794
ms.sourcegitcommit: 6312ee31561db36104f32282d019d069ede69174
ms.translationtype: MT
ms.contentlocale: id-ID
ms.lasthandoff: 03/11/2021
ms.locfileid: "50746329"
---
# <a name="stop-messages-from-moving-to-the-archive-automatically"></a><span data-ttu-id="50ab2-102">Menghentikan pesan agar tidak berpindah ke arsip secara otomatis</span><span class="sxs-lookup"><span data-stu-id="50ab2-102">Stop messages from moving to the archive automatically</span></span>

<span data-ttu-id="50ab2-103">Jika Anda menggunakan kebijakan penyimpanan, Anda bisa mengubah usia penyimpanan dalam kebijakan tersebut untuk menghentikan pengarsipan pesan secara otomatis.</span><span class="sxs-lookup"><span data-stu-id="50ab2-103">If you are using a retention policy, you can change the retention age in that policy to stop messages from archiving automatically.</span></span> <span data-ttu-id="50ab2-104">Berikut caranya:</span><span class="sxs-lookup"><span data-stu-id="50ab2-104">Here's how:</span></span>

1. <span data-ttu-id="50ab2-105">Di [Pusat admin Exchange](https://go.microsoft.com/fwlink/?linkid=2059104), pilih   >  **tag penyimpanan** manajemen kepatuhan.</span><span class="sxs-lookup"><span data-stu-id="50ab2-105">In the [Exchange admin center](https://go.microsoft.com/fwlink/?linkid=2059104), choose **compliance management** > **retention tags**.</span></span> <span data-ttu-id="50ab2-106">Temukan tag penyimpanan Pindahkan ke arsip Anda.</span><span class="sxs-lookup"><span data-stu-id="50ab2-106">Locate your Move to Archive retention tag.</span></span>
2. <span data-ttu-id="50ab2-107">Dalam tag penyimpanan, Ubah periode penyimpanan (periode arsip) agar **tidak pernah** menghentikan item yang Diarsipkan secara otomatis oleh kebijakan penyimpanan.</span><span class="sxs-lookup"><span data-stu-id="50ab2-107">In the retention tag, change the retention period (archive period) to **Never** to stop items from being automatically archived by a retention policy.</span></span>

> [!NOTE]
> <span data-ttu-id="50ab2-108">Ini akan mengubah pengaturan Arsip untuk semua kotak surat dengan tag penyimpanan ini diterapkan.</span><span class="sxs-lookup"><span data-stu-id="50ab2-108">This will change the archive setting for all mailboxes with this retention tag applied to them.</span></span>
