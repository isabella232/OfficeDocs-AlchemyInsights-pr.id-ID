---
title: Masalah dengan komputer onboarding hingga Pertahanan Microsoft untuk Titik Akhir
ms.author: pebaum
author: pebaum
manager: scotv
ms.date: 07/14/2020
ms.audience: Admin
ms.topic: article
ms.service: o365-administration
ROBOTS: NOINDEX, NOFOLLOW
localization_priority: Priority
ms.collection: Adm_O365
ms.custom:
- "6023"
- "9002913"
ms.openlocfilehash: 7ccec69f8ab43f277978176519a7f8f8df443846
ms.sourcegitcommit: 1d73771d147325cfd8578e6816becd8331913890
ms.translationtype: HT
ms.contentlocale: id-ID
ms.lasthandoff: 03/19/2021
ms.locfileid: "50901570"
---
# <a name="issues-with-onboarding-machines-to-microsoft-defender-for-endpoints"></a><span data-ttu-id="a2504-102">Masalah dengan komputer onboarding hingga Pertahanan Microsoft untuk Titik Akhir</span><span class="sxs-lookup"><span data-stu-id="a2504-102">Issues with onboarding machines to Microsoft Defender for Endpoints</span></span>

<span data-ttu-id="a2504-103">Anda mungkin mengalami masalah dengan komputer onboarding hingga layanan MDE.</span><span class="sxs-lookup"><span data-stu-id="a2504-103">You might have issues with onboarding machines to MDE service.</span></span> <span data-ttu-id="a2504-104">Jika Anda dapat mengakses komputer pengguna akhir, ikuti langkah-langkah ini:</span><span class="sxs-lookup"><span data-stu-id="a2504-104">If you can access the end-user machine, follow these steps:</span></span>

1. <span data-ttu-id="a2504-105">Unduh versi pratinjau terbaru alat diagnosis [MDE Client Analyzer](https://aka.ms/betamdeanalyzer) Anda.</span><span class="sxs-lookup"><span data-stu-id="a2504-105">Download the latest preview version of the [MDE Client Analyzer](https://aka.ms/betamdeanalyzer) diagnostic tool.</span></span>
2. <span data-ttu-id="a2504-106">Klik kanan **MDEClientAnalyzer.cmd** dan pilih ‘Jalankan sebagai administrator’.</span><span class="sxs-lookup"><span data-stu-id="a2504-106">Right click **MDEClientAnalyzer.cmd** and select ‘Run as administrator’.</span></span>
3. <span data-ttu-id="a2504-107">Ikuti semua panduan yang disarankan di **MDEClientAnalyzer.htm**.</span><span class="sxs-lookup"><span data-stu-id="a2504-107">Follow any guidance suggested in **MDEClientAnalyzer.htm**.</span></span>
4. <span data-ttu-id="a2504-108">Untuk log verbose lainnya, tinjau sub folder yang dibuat bernama **MDEClientAnalyzerResult**.</span><span class="sxs-lookup"><span data-stu-id="a2504-108">For more verbose logs, review the created sub-folder named **MDEClientAnalyzerResult**.</span></span>
5. <span data-ttu-id="a2504-109">Jika perlu panduan yang lain, hubungi [dukungan Pertahanan Microsoft untuk Titik Akhir](https://docs.microsoft.com/windows/security/threat-protection/microsoft-defender-atp/contact-support) dan sediakan file MDEClientAnalyzerResult.zip yang dihasilkan untuk analisis.</span><span class="sxs-lookup"><span data-stu-id="a2504-109">If additional guidance is needed, contact [Microsoft Defender for Endpoint support](https://docs.microsoft.com/windows/security/threat-protection/microsoft-defender-atp/contact-support) and provide the resulting MDEClientAnalyzerResult.zip file for analysis.</span></span>
