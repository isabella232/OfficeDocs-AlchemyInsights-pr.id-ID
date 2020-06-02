---
title: Kode galat 0x15
ms.author: pebaum
author: pebaum
ms.date: 04/21/2020
ms.audience: ITPro
ms.topic: article
ROBOTS: NOINDEX, NOFOLLOW
localization_priority: Normal
ms.custom:
- "919"
- "2000022"
ms.assetid: 0d566afe-b21f-4f1b-8ca9-4b4d3b0f5435
description: Jika Anda menerima pesan kesalahan saat mengaktifkan Office 2013 pada penyebaran layanan desktop jarak jauh (RDS), pertimbangkan untuk mengaktifkan ADAL dengan mengedit registri.
ms.openlocfilehash: 468d13e59602cf173ed2e17af44c66babfc28703
ms.sourcegitcommit: bc7d6f4f3c9f7060d073f5130e1ec856e248d020
ms.translationtype: MT
ms.contentlocale: id-ID
ms.lasthandoff: 06/02/2020
ms.locfileid: "44506849"
---
# <a name="error-while-activation-office-2013-on-remote-desktop-services"></a><span data-ttu-id="88d56-103">Galat saat aktivasi Office 2013 pada layanan desktop jarak jauh</span><span class="sxs-lookup"><span data-stu-id="88d56-103">Error while activation Office 2013 on Remote Desktop Services</span></span>

<span data-ttu-id="88d56-104">Jika Anda menerima pesan kesalahan saat mengaktifkan Office 2013 pada penyebaran layanan desktop jarak jauh (RDS), pertimbangkan untuk mengaktifkan ADAL dengan mengedit registri.</span><span class="sxs-lookup"><span data-stu-id="88d56-104">If you're receiving an error while activating Office 2013 on Remote Desktop Services (RDS) deployments, consider enabling ADAL by editing the registry.</span></span>
  
|<span data-ttu-id="88d56-105">**Kunci registri**</span><span class="sxs-lookup"><span data-stu-id="88d56-105">**Registry key**</span></span>|<span data-ttu-id="88d56-106">**Jenis**</span><span class="sxs-lookup"><span data-stu-id="88d56-106">**Type**</span></span>|<span data-ttu-id="88d56-107">**Nilai**</span><span class="sxs-lookup"><span data-stu-id="88d56-107">**Value**</span></span>|
|:-----|:-----|:-----|
|<span data-ttu-id="88d56-108">HKEY_CURRENT_USER \Software\Microsoft\Office\15.0\Common\Identity\EnableADAL</span><span class="sxs-lookup"><span data-stu-id="88d56-108">HKEY_CURRENT_USER\Software\Microsoft\Office\15.0\Common\Identity\EnableADAL</span></span>  <br/> |<span data-ttu-id="88d56-109">REG_DWORD</span><span class="sxs-lookup"><span data-stu-id="88d56-109">REG_DWORD</span></span>  <br/> |<span data-ttu-id="88d56-110">1</span><span class="sxs-lookup"><span data-stu-id="88d56-110">1</span></span>  <br/> |

<span data-ttu-id="88d56-111">Untuk informasi selengkapnya, lihat [mengaktifkan otentikasi modern untuk Office 2013 pada perangkat Windows](https://docs.microsoft.com/microsoft-365/admin/security-and-compliance/enable-modern-authentication).</span><span class="sxs-lookup"><span data-stu-id="88d56-111">For more information, see [Enable Modern Authentication for Office 2013 on Windows devices](https://docs.microsoft.com/microsoft-365/admin/security-and-compliance/enable-modern-authentication).</span></span>
  
> [!NOTE]
>  <span data-ttu-id="88d56-112">ADAL diaktifkan secara default di Microsoft 365 aplikasi untuk perusahaan dan Office 2016.</span><span class="sxs-lookup"><span data-stu-id="88d56-112">ADAL is enabled by default in Microsoft 365 Apps for enterprise and Office 2016.</span></span> <span data-ttu-id="88d56-113">Layanan desktop jarak jauh (RDS) sebelumnya bernama layanan terminal.</span><span class="sxs-lookup"><span data-stu-id="88d56-113">Remote Desktop Services (RDS) was previously named Terminal Services.</span></span>
  