---
title: 932 upgrade AADConnect
ms.author: chrisda
author: chrisda
manager: dansimp
ms.date: 04/21/2020
ms.audience: ITPro
ms.topic: article
ROBOTS: NOINDEX, NOFOLLOW
localization_priority: Normal
ms.custom:
- "932"
- "1300025"
ms.assetid: 8f43f36c-9722-43a4-b0de-c5341c06dac5
ms.openlocfilehash: fcc5fddb5cfd15407d0533449035317d187931ed
ms.sourcegitcommit: 631cbb5f03e5371f0995e976536d24e9d13746c3
ms.translationtype: MT
ms.contentlocale: id-ID
ms.lasthandoff: 04/22/2020
ms.locfileid: "43766496"
---
# <a name="upgrade-azure-ad-connect"></a><span data-ttu-id="de9a2-102">Meningkatkan Azure AD menyambung</span><span class="sxs-lookup"><span data-stu-id="de9a2-102">Upgrade Azure AD Connect</span></span>

<span data-ttu-id="de9a2-103">Secara default, upgrade otomatis diaktifkan untuk Azure AD menyambung, yang membantu untuk memastikan bahwa Anda menjalankan versi terbaru.</span><span class="sxs-lookup"><span data-stu-id="de9a2-103">By default, automatic upgrade is enabled for Azure AD Connect, which helps to ensure you're running the latest version.</span></span> <span data-ttu-id="de9a2-104">Untuk memverifikasi pengaturan upgrade otomatis, gunakan cmdlet **Get-ADSyncAutoUpgrade** di Azure AD PowerShell.</span><span class="sxs-lookup"><span data-stu-id="de9a2-104">To verify the automatic upgrade settings, use the **Get-ADSyncAutoUpgrade** cmdlet in Azure AD PowerShell.</span></span> <span data-ttu-id="de9a2-105">Cmdlet akan mengembalikan salah satu nilai berikut:</span><span class="sxs-lookup"><span data-stu-id="de9a2-105">The cmdlet will return one of following values:</span></span>

- <span data-ttu-id="de9a2-106">**Enabled**: upgrade otomatis diaktifkan.</span><span class="sxs-lookup"><span data-stu-id="de9a2-106">**Enabled**: Automatic upgrade is enabled.</span></span>

- <span data-ttu-id="de9a2-107">**Nonaktif**: peningkatan otomatis dinonaktifkan.</span><span class="sxs-lookup"><span data-stu-id="de9a2-107">**Disabled**: Automatic upgrade is disabled.</span></span>

- <span data-ttu-id="de9a2-108">**Ditangguhkan**: sistem tidak lagi memenuhi syarat untuk menerima upgrade otomatis.</span><span class="sxs-lookup"><span data-stu-id="de9a2-108">**Suspended**: The system is no longer eligible to receive automatic upgrades.</span></span> <span data-ttu-id="de9a2-109">Anda tidak dapat mengkonfigurasi nilai ini; itu diatur oleh sistem.</span><span class="sxs-lookup"><span data-stu-id="de9a2-109">You can't configure this value; it's set by the system.</span></span>

<span data-ttu-id="de9a2-110">Untuk informasi lebih lanjut, lihat [upgrade otomatis](https://docs.microsoft.com/azure/active-directory/connect/active-directory-aadconnect-feature-automatic-upgrade).</span><span class="sxs-lookup"><span data-stu-id="de9a2-110">For more information, see [Automatic upgrade](https://docs.microsoft.com/azure/active-directory/connect/active-directory-aadconnect-feature-automatic-upgrade).</span></span>

<span data-ttu-id="de9a2-111">Untuk mengunduh versi terbaru Azure AD menyambung, kunjungi [https://www.microsoft.com/download/details.aspx?id=47594](https://www.microsoft.com/download/details.aspx?id=47594).</span><span class="sxs-lookup"><span data-stu-id="de9a2-111">To download the latest version of Azure AD Connect, go to [https://www.microsoft.com/download/details.aspx?id=47594](https://www.microsoft.com/download/details.aspx?id=47594).</span></span>
