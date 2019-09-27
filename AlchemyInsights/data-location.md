---
title: Lokasi data
ms.author: pebaum
author: pebaum
ms.audience: ITPro
ms.topic: article
ROBOTS: NOINDEX, NOFOLLOW
localization_priority: Normal
ms.custom:
- "945"
- "5300023"
ms.assetid: 3bab036c-dbaa-406a-8b73-1e5f31993436
ms.openlocfilehash: 0e683c8266d425be95e87c590d4cb5d56108721a
ms.sourcegitcommit: 71978e2bb779b5955fd113f84512b83321b26912
ms.translationtype: MT
ms.contentlocale: id-ID
ms.lasthandoff: 09/26/2019
ms.locfileid: "37207264"
---
# <a name="data-location"></a><span data-ttu-id="91806-102">Lokasi data</span><span class="sxs-lookup"><span data-stu-id="91806-102">Data location</span></span>

<span data-ttu-id="91806-103">Anda dapat melihat lokasi penyewa Office 365 Anda di pusat admin atau dengan menyambung ke Exchange Online melalui PowerShell.</span><span class="sxs-lookup"><span data-stu-id="91806-103">You can view the location of your Office 365 tenant in the admin center or by connecting to Exchange Online via PowerShell.</span></span>


<span data-ttu-id="91806-104">**Pusat admin:**</span><span class="sxs-lookup"><span data-stu-id="91806-104">**Admin center:**</span></span>
1. <span data-ttu-id="91806-105">Masuk ke [Pusat admin](https://admin.microsoft.com/Adminportal/Home).</span><span class="sxs-lookup"><span data-stu-id="91806-105">Log in to the [admin center](https://admin.microsoft.com/Adminportal/Home).</span></span>
2. <span data-ttu-id="91806-106">Pilih **pengaturan** > **profil organisasi**.</span><span class="sxs-lookup"><span data-stu-id="91806-106">Select **Settings** > **Organization profile**.</span></span>
3. <span data-ttu-id="91806-107">Di bawah **Lokasi data**, pilih **Lihat rincian**.</span><span class="sxs-lookup"><span data-stu-id="91806-107">Under **Data location**, select **View details**.</span></span>


<span data-ttu-id="91806-108">**Powershell:**</span><span class="sxs-lookup"><span data-stu-id="91806-108">**PowerShell:**</span></span>
1. <span data-ttu-id="91806-109">Menyambung ke Exchange Online menggunakan Windows PowerShell.</span><span class="sxs-lookup"><span data-stu-id="91806-109">Connect to Exchange Online by using Windows PowerShell.</span></span>
2. <span data-ttu-id="91806-110">Jalankan cmdlet [Get-OrganizationalUnit](https://docs.microsoft.com/en-us/powershell/module/exchange/active-directory/get-organizationalunit) untuk menampilkan daftar properti penghuni Anda.</span><span class="sxs-lookup"><span data-stu-id="91806-110">Execute the [Get-OrganizationalUnit](https://docs.microsoft.com/en-us/powershell/module/exchange/active-directory/get-organizationalunit) cmdlet to display a list of your tenant’s properties.</span></span> 
3. <span data-ttu-id="91806-111">Lihat properti OrganizationId.</span><span class="sxs-lookup"><span data-stu-id="91806-111">Look at the OrganizationId property.</span></span>

<span data-ttu-id="91806-112">Bila Anda memiliki lokasi data untuk EXO dan SPO, Anda dapat menentukan lokasi data untuk layanan lain yang dapat Anda gunakan dari [tempat data Anda berada](https://products.office.com/where-is-your-data-located).</span><span class="sxs-lookup"><span data-stu-id="91806-112">When you have the data location for EXO and SPO, you can determine the data location for other services you may use from [Where your data is located](https://products.office.com/where-is-your-data-located).</span></span>