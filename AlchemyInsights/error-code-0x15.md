---
title: Kode kesalahan 0x15
ms.author: pebaum
author: pebaum
ms.date: 04/21/2020
ms.audience: ITPro
ms.topic: article
ms.service: o365-administration
ROBOTS: NOINDEX, NOFOLLOW
localization_priority: Normal
ms.custom:
- "919"
- "2000022"
ms.assetid: 0d566afe-b21f-4f1b-8ca9-4b4d3b0f5435
description: Jika Anda menerima kesalahan saat mengaktifkan Office 2013 di penyebaran layanan desktop jarak jauh (RDS), pertimbangkan untuk mengaktifkan ADAL dengan mengedit registri.
ms.openlocfilehash: deb2ac4b0fb6a7b2e0045ff1b0ba95ad6e5e4a3a
ms.sourcegitcommit: c6692ce0fa1358ec3529e59ca0ecdfdea4cdc759
ms.translationtype: MT
ms.contentlocale: id-ID
ms.lasthandoff: 09/14/2020
ms.locfileid: "47709190"
---
# <a name="error-while-activation-office-2013-on-remote-desktop-services"></a><span data-ttu-id="8629a-103">Kesalahan saat aktivasi Office 2013 pada layanan desktop jarak jauh</span><span class="sxs-lookup"><span data-stu-id="8629a-103">Error while activation Office 2013 on Remote Desktop Services</span></span>

<span data-ttu-id="8629a-104">Jika Anda menerima kesalahan saat mengaktifkan Office 2013 di penyebaran layanan desktop jarak jauh (RDS), pertimbangkan untuk mengaktifkan ADAL dengan mengedit registri.</span><span class="sxs-lookup"><span data-stu-id="8629a-104">If you're receiving an error while activating Office 2013 on Remote Desktop Services (RDS) deployments, consider enabling ADAL by editing the registry.</span></span>
  
|<span data-ttu-id="8629a-105">**Kunci registri**</span><span class="sxs-lookup"><span data-stu-id="8629a-105">**Registry key**</span></span>|<span data-ttu-id="8629a-106">**Mengetikkan**</span><span class="sxs-lookup"><span data-stu-id="8629a-106">**Type**</span></span>|<span data-ttu-id="8629a-107">**Nilainya**</span><span class="sxs-lookup"><span data-stu-id="8629a-107">**Value**</span></span>|
|:-----|:-----|:-----|
|<span data-ttu-id="8629a-108">HKEY_CURRENT_USER \Software\Microsoft\Office\15.0\Common\Identity\EnableADAL</span><span class="sxs-lookup"><span data-stu-id="8629a-108">HKEY_CURRENT_USER\Software\Microsoft\Office\15.0\Common\Identity\EnableADAL</span></span>  <br/> |<span data-ttu-id="8629a-109">REG_DWORD</span><span class="sxs-lookup"><span data-stu-id="8629a-109">REG_DWORD</span></span>  <br/> |<span data-ttu-id="8629a-110">,1</span><span class="sxs-lookup"><span data-stu-id="8629a-110">1</span></span>  <br/> |

<span data-ttu-id="8629a-111">Untuk informasi selengkapnya, lihat [mengaktifkan autentikasi modern untuk Office 2013 di perangkat Windows](https://docs.microsoft.com/microsoft-365/admin/security-and-compliance/enable-modern-authentication).</span><span class="sxs-lookup"><span data-stu-id="8629a-111">For more information, see [Enable Modern Authentication for Office 2013 on Windows devices](https://docs.microsoft.com/microsoft-365/admin/security-and-compliance/enable-modern-authentication).</span></span>
  
> [!NOTE]
>  <span data-ttu-id="8629a-112">ADAL diaktifkan secara default di aplikasi Microsoft 365 untuk perusahaan dan Office 2016.</span><span class="sxs-lookup"><span data-stu-id="8629a-112">ADAL is enabled by default in Microsoft 365 Apps for enterprise and Office 2016.</span></span> <span data-ttu-id="8629a-113">Layanan desktop jarak jauh (RDS) sebelumnya bernama layanan terminal.</span><span class="sxs-lookup"><span data-stu-id="8629a-113">Remote Desktop Services (RDS) was previously named Terminal Services.</span></span>
  