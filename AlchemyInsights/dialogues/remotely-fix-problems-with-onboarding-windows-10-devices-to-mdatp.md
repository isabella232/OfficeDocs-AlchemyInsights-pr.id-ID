---
title: Memperbaiki masalah secara jarak jauh dengan perangkat orientasi otomatis Windows 10 ke proteksi ancaman tingkat lanjut Microsoft Defender
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
ms.openlocfilehash: 5473d090f6d4680f9a62f34f943ac6cea53b2079
ms.sourcegitcommit: 4883f1f89d4c6ca23161e9a43ff206ad21d4f09b
ms.translationtype: MT
ms.contentlocale: id-ID
ms.lasthandoff: 03/08/2021
ms.locfileid: "50693653"
---
# <a name="remotely-fix-problems-with-onboarding-windows-10-devices-to-microsoft-defender-advanced-threat-protection"></a><span data-ttu-id="9408f-102">Memperbaiki masalah secara jarak jauh dengan perangkat orientasi otomatis Windows 10 ke proteksi ancaman tingkat lanjut Microsoft Defender</span><span class="sxs-lookup"><span data-stu-id="9408f-102">Remotely fix problems with onboarding Windows 10 devices to Microsoft Defender Advanced Threat Protection</span></span>

<span data-ttu-id="9408f-103">Jika Anda bisa mengakses komputer jarak jauh, ikuti langkah berikut:</span><span class="sxs-lookup"><span data-stu-id="9408f-103">If you can access the remote computer, follow these steps:</span></span>

1. <span data-ttu-id="9408f-104">Unduh alat diagnostik [Penganalisis konektivitas klien](https://go.microsoft.com/fwlink/?linkid=2143466) .</span><span class="sxs-lookup"><span data-stu-id="9408f-104">Download the [Client Connectivity Analyzer](https://go.microsoft.com/fwlink/?linkid=2143466) diagnostic tool.</span></span>
2. <span data-ttu-id="9408f-105">Ekstrak dan jalankan MDATPAnalyzer. CMD.</span><span class="sxs-lookup"><span data-stu-id="9408f-105">Extract and run MDATPAnalyzer.cmd.</span></span>
3. <span data-ttu-id="9408f-106">Temukan log diagnostik dalam folder MDATPClientAnalyzerResult, yang merupakan folder yang sama di mana alat Penganalisis diunduh.</span><span class="sxs-lookup"><span data-stu-id="9408f-106">Locate the diagnostic log in the MDATPClientAnalyzerResult folder, which is the same folder where the Analyzer tool was downloaded.</span></span>
4. <span data-ttu-id="9408f-107">Untuk menemukan masalah konektivitas atau pengaturan proksi internet, Tinjau file log yang MDATPClientAnalyzer.txt.</span><span class="sxs-lookup"><span data-stu-id="9408f-107">To find issues with connectivity or Internet proxy settings, review the log file MDATPClientAnalyzer.txt.</span></span>

<span data-ttu-id="9408f-108">Untuk mempelajari selengkapnya, lihat [masalah dengan mesin orientasi](https://go.microsoft.com/fwlink/?linkid=2143634).</span><span class="sxs-lookup"><span data-stu-id="9408f-108">To learn more, see [Issues with onboarding machines](https://go.microsoft.com/fwlink/?linkid=2143634).</span></span>
