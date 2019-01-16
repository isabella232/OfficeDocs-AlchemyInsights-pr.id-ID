---
title: 932 upgrade AADConnect
ms.author: chrisda
author: chrisda
manager: serdars
ms.date: 6/8/2018
ms.audience: ITPro
ms.topic: article
ROBOTS: NOINDEX, NOFOLLOW
localization_priority: Priority
ms.assetid: 8f43f36c-9722-43a4-b0de-c5341c06dac5
ms.openlocfilehash: 9add88a0e4a2590639cbfc546afdcdf5e6aa4886
ms.sourcegitcommit: d6ea5e9458a2b8ceaab3ac4bd483e1130b9a398a
ms.translationtype: MT
ms.contentlocale: id-ID
ms.lasthandoff: 01/15/2019
ms.locfileid: "28295273"
---
# <a name="upgrade-azure-ad-connect"></a><span data-ttu-id="7cdbe-102">Upgrade iklan Azure terhubung</span><span class="sxs-lookup"><span data-stu-id="7cdbe-102">Upgrade Azure AD Connect</span></span>

<span data-ttu-id="7cdbe-p101">Secara default, upgrade otomatis diaktifkan untuk Azure iklan Connect, yang membantu untuk memastikan Anda sedang menjalankan versi terbaru. Untuk memverifikasi pengaturan upgrade otomatis, gunakan cmdlet **Get-ADSyncAutoUpgrade** di Azure iklan PowerShell. Cmdlet akan kembali salah satu nilai berikut:</span><span class="sxs-lookup"><span data-stu-id="7cdbe-p101">By default, automatic upgrade is enabled for Azure AD Connect, which helps to ensure you're running the latest version. To verify the automatic upgrade settings, use the **Get-ADSyncAutoUpgrade** cmdlet in Azure AD PowerShell. The cmdlet will return one of following values:</span></span> 
  
- <span data-ttu-id="7cdbe-106">**Diaktifkan**: upgrade otomatis diaktifkan.</span><span class="sxs-lookup"><span data-stu-id="7cdbe-106">**Enabled**: Automatic upgrade is enabled.</span></span> 
    
- <span data-ttu-id="7cdbe-107">**Dinonaktifkan**: upgrade otomatis dinonaktifkan.</span><span class="sxs-lookup"><span data-stu-id="7cdbe-107">**Disabled**: Automatic upgrade is disabled.</span></span> 
    
- <span data-ttu-id="7cdbe-p102">**Suspended**: sistem ini tidak lagi memenuhi syarat untuk menerima upgrade otomatis. Anda tidak dapat mengkonfigurasi nilai ini; diatur oleh sistem.</span><span class="sxs-lookup"><span data-stu-id="7cdbe-p102">**Suspended**: The system is no longer eligible to receive automatic upgrades. You can't configure this value; it's set by the system.</span></span> 
    
<span data-ttu-id="7cdbe-110">Untuk informasi lebih lanjut, lihat [upgrade otomatis](https://docs.microsoft.com/azure/active-directory/connect/active-directory-aadconnect-feature-automatic-upgrade).</span><span class="sxs-lookup"><span data-stu-id="7cdbe-110">For more information, see [Automatic upgrade](https://docs.microsoft.com/azure/active-directory/connect/active-directory-aadconnect-feature-automatic-upgrade).</span></span>
  
<span data-ttu-id="7cdbe-111">Untuk men-download versi terbaru dari Azure iklan terhubung, pergi ke [https://www.microsoft.com/download/details.aspx?id=47594](https://www.microsoft.com/download/details.aspx?id=47594).</span><span class="sxs-lookup"><span data-stu-id="7cdbe-111">To download the latest version of Azure AD Connect, go to [https://www.microsoft.com/download/details.aspx?id=47594](https://www.microsoft.com/download/details.aspx?id=47594).</span></span>
  

