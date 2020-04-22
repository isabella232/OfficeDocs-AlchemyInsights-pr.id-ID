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
ms.openlocfilehash: 566d63cbe37d295b3546b9d7d5b14dfc8e8fe0ec
ms.sourcegitcommit: 55eff703a17e500681d8fa6a87eb067019ade3cc
ms.translationtype: MT
ms.contentlocale: id-ID
ms.lasthandoff: 04/22/2020
ms.locfileid: "43703141"
---
# <a name="error-while-activation-office-2013-on-remote-desktop-services"></a><span data-ttu-id="66158-103">Galat saat aktivasi Office 2013 pada layanan desktop jarak jauh</span><span class="sxs-lookup"><span data-stu-id="66158-103">Error while activation Office 2013 on Remote Desktop Services</span></span>

<span data-ttu-id="66158-104">Jika Anda menerima pesan kesalahan saat mengaktifkan Office 2013 pada penyebaran layanan desktop jarak jauh (RDS), pertimbangkan untuk mengaktifkan ADAL dengan mengedit registri.</span><span class="sxs-lookup"><span data-stu-id="66158-104">If you're receiving an error while activating Office 2013 on Remote Desktop Services (RDS) deployments, consider enabling ADAL by editing the registry.</span></span>
  
|<span data-ttu-id="66158-105">**Kunci registri**</span><span class="sxs-lookup"><span data-stu-id="66158-105">**Registry key**</span></span>|<span data-ttu-id="66158-106">**Jenis**</span><span class="sxs-lookup"><span data-stu-id="66158-106">**Type**</span></span>|<span data-ttu-id="66158-107">**Nilai**</span><span class="sxs-lookup"><span data-stu-id="66158-107">**Value**</span></span>|
|:-----|:-----|:-----|
|<span data-ttu-id="66158-108">HKEY_CURRENT_USER \Software\Microsoft\Office\15.0\Common\Identity\EnableADAL</span><span class="sxs-lookup"><span data-stu-id="66158-108">HKEY_CURRENT_USER\Software\Microsoft\Office\15.0\Common\Identity\EnableADAL</span></span>  <br/> |<span data-ttu-id="66158-109">REG_DWORD</span><span class="sxs-lookup"><span data-stu-id="66158-109">REG_DWORD</span></span>  <br/> |<span data-ttu-id="66158-110">1</span><span class="sxs-lookup"><span data-stu-id="66158-110">1</span></span>  <br/> |

<span data-ttu-id="66158-111">Untuk informasi selengkapnya, lihat [mengaktifkan otentikasi modern untuk Office 2013 pada perangkat Windows](https://docs.microsoft.com/office365/admin/security-and-compliance/enable-modern-authentication).</span><span class="sxs-lookup"><span data-stu-id="66158-111">For more information, see [Enable Modern Authentication for Office 2013 on Windows devices](https://docs.microsoft.com/office365/admin/security-and-compliance/enable-modern-authentication).</span></span>
  
> [!NOTE]
>  <span data-ttu-id="66158-112">ADAL diaktifkan secara default di Microsoft 365 aplikasi untuk perusahaan dan Office 2016.</span><span class="sxs-lookup"><span data-stu-id="66158-112">ADAL is enabled by default in Microsoft 365 Apps for enterprise and Office 2016.</span></span> <span data-ttu-id="66158-113">Layanan desktop jarak jauh (RDS) sebelumnya bernama layanan terminal.</span><span class="sxs-lookup"><span data-stu-id="66158-113">Remote Desktop Services (RDS) was previously named Terminal Services.</span></span>
  