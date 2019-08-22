---
title: 932 upgrade AADConnect
ms.author: chrisda
author: chrisda
manager: dansimp
ms.date: 6/8/2018
ms.audience: ITPro
ms.topic: article
ROBOTS: NOINDEX, NOFOLLOW
localization_priority: Normal
ms.custom:
- "932"
- "1300025"
ms.assetid: 8f43f36c-9722-43a4-b0de-c5341c06dac5
ms.openlocfilehash: ff3f74348599788edd8ce0991fe49bb6a54b55af
ms.sourcegitcommit: 1d98db8acb9959aba3b5e308a567ade6b62da56c
ms.translationtype: MT
ms.contentlocale: id-ID
ms.lasthandoff: 08/22/2019
ms.locfileid: "36506086"
---
# <a name="upgrade-azure-ad-connect"></a><span data-ttu-id="9ba75-102">Upgrade iklan Azure terhubung</span><span class="sxs-lookup"><span data-stu-id="9ba75-102">Upgrade Azure AD Connect</span></span>

<span data-ttu-id="9ba75-103">Secara default, upgrade otomatis diaktifkan untuk Azure iklan Connect, yang membantu untuk memastikan Anda sedang menjalankan versi terbaru.</span><span class="sxs-lookup"><span data-stu-id="9ba75-103">By default, automatic upgrade is enabled for Azure AD Connect, which helps to ensure you're running the latest version.</span></span> <span data-ttu-id="9ba75-104">Untuk memverifikasi pengaturan upgrade otomatis, gunakan cmdlet **Get-ADSyncAutoUpgrade** di Azure iklan PowerShell.</span><span class="sxs-lookup"><span data-stu-id="9ba75-104">To verify the automatic upgrade settings, use the **Get-ADSyncAutoUpgrade** cmdlet in Azure AD PowerShell.</span></span> <span data-ttu-id="9ba75-105">Cmdlet akan kembali salah satu nilai berikut:</span><span class="sxs-lookup"><span data-stu-id="9ba75-105">The cmdlet will return one of following values:</span></span>

- <span data-ttu-id="9ba75-106">**Diaktifkan**: upgrade otomatis diaktifkan.</span><span class="sxs-lookup"><span data-stu-id="9ba75-106">**Enabled**: Automatic upgrade is enabled.</span></span>

- <span data-ttu-id="9ba75-107">**Dinonaktifkan**: upgrade otomatis dinonaktifkan.</span><span class="sxs-lookup"><span data-stu-id="9ba75-107">**Disabled**: Automatic upgrade is disabled.</span></span>

- <span data-ttu-id="9ba75-108">**Suspended**: sistem ini tidak lagi memenuhi syarat untuk menerima upgrade otomatis.</span><span class="sxs-lookup"><span data-stu-id="9ba75-108">**Suspended**: The system is no longer eligible to receive automatic upgrades.</span></span> <span data-ttu-id="9ba75-109">Anda tidak dapat mengkonfigurasi nilai ini; diatur oleh sistem.</span><span class="sxs-lookup"><span data-stu-id="9ba75-109">You can't configure this value; it's set by the system.</span></span>

<span data-ttu-id="9ba75-110">Untuk informasi lebih lanjut, lihat [upgrade otomatis](https://docs.microsoft.com/azure/active-directory/connect/active-directory-aadconnect-feature-automatic-upgrade).</span><span class="sxs-lookup"><span data-stu-id="9ba75-110">For more information, see [Automatic upgrade](https://docs.microsoft.com/azure/active-directory/connect/active-directory-aadconnect-feature-automatic-upgrade).</span></span>

<span data-ttu-id="9ba75-111">Untuk men-download versi terbaru dari Azure iklan terhubung, pergi ke [https://www.microsoft.com/download/details.aspx?id=47594](https://www.microsoft.com/download/details.aspx?id=47594).</span><span class="sxs-lookup"><span data-stu-id="9ba75-111">To download the latest version of Azure AD Connect, go to [https://www.microsoft.com/download/details.aspx?id=47594](https://www.microsoft.com/download/details.aspx?id=47594).</span></span>
