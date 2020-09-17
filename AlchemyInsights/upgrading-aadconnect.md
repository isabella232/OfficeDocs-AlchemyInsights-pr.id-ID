---
title: 932 memutakhirkan AADConnect
ms.author: chrisda
author: chrisda
manager: dansimp
ms.date: 04/21/2020
ms.audience: ITPro
ms.topic: article
ms.service: o365-administration
ROBOTS: NOINDEX, NOFOLLOW
localization_priority: Normal
ms.custom:
- "932"
- "1300025"
ms.assetid: 8f43f36c-9722-43a4-b0de-c5341c06dac5
ms.openlocfilehash: 5c8ec5d9282c53c655e28f5d38fe36fc3ab005b8
ms.sourcegitcommit: c6692ce0fa1358ec3529e59ca0ecdfdea4cdc759
ms.translationtype: MT
ms.contentlocale: id-ID
ms.lasthandoff: 09/15/2020
ms.locfileid: "47806042"
---
# <a name="upgrade-azure-ad-connect"></a><span data-ttu-id="0b10a-102">Memutakhirkan Azure AD Connect</span><span class="sxs-lookup"><span data-stu-id="0b10a-102">Upgrade Azure AD Connect</span></span>

<span data-ttu-id="0b10a-103">Secara default, pemutakhiran otomatis diaktifkan untuk Azure AD Connect, yang membantu memastikan Anda menjalankan versi terbaru.</span><span class="sxs-lookup"><span data-stu-id="0b10a-103">By default, automatic upgrade is enabled for Azure AD Connect, which helps to ensure you're running the latest version.</span></span> <span data-ttu-id="0b10a-104">Untuk memverifikasi pengaturan pemutakhiran otomatis, gunakan cmdlet **Get-ADSyncAutoUpgrade** di Azure AD PowerShell.</span><span class="sxs-lookup"><span data-stu-id="0b10a-104">To verify the automatic upgrade settings, use the **Get-ADSyncAutoUpgrade** cmdlet in Azure AD PowerShell.</span></span> <span data-ttu-id="0b10a-105">Cmdlet akan mengembalikan salah satu nilai berikut:</span><span class="sxs-lookup"><span data-stu-id="0b10a-105">The cmdlet will return one of following values:</span></span>

- <span data-ttu-id="0b10a-106">**Diaktifkan**: pemutakhiran otomatis diaktifkan.</span><span class="sxs-lookup"><span data-stu-id="0b10a-106">**Enabled**: Automatic upgrade is enabled.</span></span>

- <span data-ttu-id="0b10a-107">**Dinonaktifkan**: pemutakhiran otomatis dinonaktifkan.</span><span class="sxs-lookup"><span data-stu-id="0b10a-107">**Disabled**: Automatic upgrade is disabled.</span></span>

- <span data-ttu-id="0b10a-108">**Ditangguhkan**: sistem tidak lagi memenuhi syarat untuk menerima Pemutakhiran otomatis.</span><span class="sxs-lookup"><span data-stu-id="0b10a-108">**Suspended**: The system is no longer eligible to receive automatic upgrades.</span></span> <span data-ttu-id="0b10a-109">Anda tidak bisa mengonfigurasi nilai ini; ini diatur oleh sistem.</span><span class="sxs-lookup"><span data-stu-id="0b10a-109">You can't configure this value; it's set by the system.</span></span>

<span data-ttu-id="0b10a-110">Untuk informasi selengkapnya, lihat [pemutakhiran otomatis](https://docs.microsoft.com/azure/active-directory/connect/active-directory-aadconnect-feature-automatic-upgrade).</span><span class="sxs-lookup"><span data-stu-id="0b10a-110">For more information, see [Automatic upgrade](https://docs.microsoft.com/azure/active-directory/connect/active-directory-aadconnect-feature-automatic-upgrade).</span></span>

<span data-ttu-id="0b10a-111">Untuk mengunduh versi terbaru Azure AD Connect, masuk ke [https://www.microsoft.com/download/details.aspx?id=47594](https://www.microsoft.com/download/details.aspx?id=47594) .</span><span class="sxs-lookup"><span data-stu-id="0b10a-111">To download the latest version of Azure AD Connect, go to [https://www.microsoft.com/download/details.aspx?id=47594](https://www.microsoft.com/download/details.aspx?id=47594).</span></span>
