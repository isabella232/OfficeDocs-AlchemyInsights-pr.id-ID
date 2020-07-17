---
title: Masalah dengan mesin onboarding
ms.author: pebaum
author: pebaum
manager: scotv
ms.date: 07/14/2020
ms.audience: Admin
ms.topic: article
ROBOTS: NOINDEX, NOFOLLOW
localization_priority: Priority
ms.collection: Adm_O365
ms.custom:
- "6023"
- "9002913"
ms.openlocfilehash: 19b516dc21472e2c80a8b9046f802b329d15e4d6
ms.sourcegitcommit: 45c2aaeee58c0be466b76c7f0cd71e796d3c8f76
ms.translationtype: MT
ms.contentlocale: id-ID
ms.lasthandoff: 07/15/2020
ms.locfileid: "45141652"
---
# <a name="issues-with-onboarding-machines"></a><span data-ttu-id="595cf-102">Masalah dengan mesin onboarding</span><span class="sxs-lookup"><span data-stu-id="595cf-102">Issues with onboarding machines</span></span>

<span data-ttu-id="595cf-103">Anda mungkin memiliki masalah dengan mesin onboarding untuk layanan MDATP.</span><span class="sxs-lookup"><span data-stu-id="595cf-103">You might have issues with onboarding machines to MDATP service.</span></span> <span data-ttu-id="595cf-104">Jika Anda dapat mengakses mesin pengguna akhir, ikuti langkah berikut:</span><span class="sxs-lookup"><span data-stu-id="595cf-104">If you can access the end-user machine, follow these steps:</span></span>

1. <span data-ttu-id="595cf-105">Unduh alat diagnostik [Penganalisis konektivitas klien](https://aka.ms/mdatpanalyzer) .</span><span class="sxs-lookup"><span data-stu-id="595cf-105">Download the [Client Connectivity Analyzer](https://aka.ms/mdatpanalyzer) diagnostic tool.</span></span>
2. <span data-ttu-id="595cf-106">Ekstrak dan jalankan MDATPAnalyzer. CMD.</span><span class="sxs-lookup"><span data-stu-id="595cf-106">Extract and run MDATPAnalyzer.cmd.</span></span>
3. <span data-ttu-id="595cf-107">Temukan log diagnostik di folder yang disebut MDATPClientAnalyzerResult, folder yang sama di mana alat Analyzer diunduh.</span><span class="sxs-lookup"><span data-stu-id="595cf-107">Locate the diagnostic log in the folder called MDATPClientAnalyzerResult, the same folder where the Analyzer tool is downloaded.</span></span>
4. <span data-ttu-id="595cf-108">Tinjau file log, MDATPClientAnalyzer.txt, untuk menemukan masalah konektivitas atau pengaturan proxy Internet.</span><span class="sxs-lookup"><span data-stu-id="595cf-108">Review the log file, MDATPClientAnalyzer.txt, to find connectivity or internet proxy settings issues.</span></span>