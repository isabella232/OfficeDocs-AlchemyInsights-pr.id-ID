---
title: Kode kesalahan 0x15
ms.author: pebaum
author: pebaum
ms.date: 10/31/2018
ms.audience: ITPro
ms.topic: article
ROBOTS: NOINDEX, NOFOLLOW
localization_priority: Normal
ms.custom:
- "919"
- "2000022"
ms.assetid: 0d566afe-b21f-4f1b-8ca9-4b4d3b0f5435
description: Jika Anda menerima kesalahan ketika mengaktifkan kantor 2013 pada Remote Desktop Services (RDS) penyebaran, mempertimbangkan memungkinkan ADAL dengan mengedit registri.
ms.openlocfilehash: 4ef2943e5a529368fa2c614e4431cf180924fbb8
ms.sourcegitcommit: 1d98db8acb9959aba3b5e308a567ade6b62da56c
ms.translationtype: MT
ms.contentlocale: id-ID
ms.lasthandoff: 08/22/2019
ms.locfileid: "36527005"
---
# <a name="error-while-activation-office-2013-on-remote-desktop-services"></a><span data-ttu-id="dcd2c-103">Kesalahan saat aktivasi kantor 2013 pada Remote Desktop Services</span><span class="sxs-lookup"><span data-stu-id="dcd2c-103">Error while activation Office 2013 on Remote Desktop Services</span></span>

<span data-ttu-id="dcd2c-104">Jika Anda menerima kesalahan ketika mengaktifkan kantor 2013 pada Remote Desktop Services (RDS) penyebaran, mempertimbangkan memungkinkan ADAL dengan mengedit registri.</span><span class="sxs-lookup"><span data-stu-id="dcd2c-104">If you're receiving an error while activating Office 2013 on Remote Desktop Services (RDS) deployments, consider enabling ADAL by editing the registry.</span></span>
  
|<span data-ttu-id="dcd2c-105">**Kunci registri**</span><span class="sxs-lookup"><span data-stu-id="dcd2c-105">**Registry key**</span></span>|<span data-ttu-id="dcd2c-106">**Jenis**</span><span class="sxs-lookup"><span data-stu-id="dcd2c-106">**Type**</span></span>|<span data-ttu-id="dcd2c-107">**Nilai**</span><span class="sxs-lookup"><span data-stu-id="dcd2c-107">**Value**</span></span>|
|:-----|:-----|:-----|
|<span data-ttu-id="dcd2c-108">HKEY_CURRENT_USER\Software\Microsoft\Office\15.0\Common\Identity\EnableADAL</span><span class="sxs-lookup"><span data-stu-id="dcd2c-108">HKEY_CURRENT_USER\Software\Microsoft\Office\15.0\Common\Identity\EnableADAL</span></span>  <br/> |<span data-ttu-id="dcd2c-109">REG_DWORD</span><span class="sxs-lookup"><span data-stu-id="dcd2c-109">REG_DWORD</span></span>  <br/> |<span data-ttu-id="dcd2c-110">1</span><span class="sxs-lookup"><span data-stu-id="dcd2c-110">1</span></span>  <br/> |

<span data-ttu-id="dcd2c-111">Untuk selengkapnya, lihat [Mengaktifkan otentikasi Modern untuk kantor 2013 pada perangkat Windows](https://docs.microsoft.com/office365/admin/security-and-compliance/enable-modern-authentication).</span><span class="sxs-lookup"><span data-stu-id="dcd2c-111">For more information, see [Enable Modern Authentication for Office 2013 on Windows devices](https://docs.microsoft.com/office365/admin/security-and-compliance/enable-modern-authentication).</span></span>
  
> [!NOTE]
>  <span data-ttu-id="dcd2c-112">ADAL diaktifkan secara default di kantor 365 ProPlus dan kantor 2016.</span><span class="sxs-lookup"><span data-stu-id="dcd2c-112">ADAL is enabled by default in Office 365 ProPlus and Office 2016.</span></span> <span data-ttu-id="dcd2c-113">Remote Desktop Services (RDS) sebelumnya bernama Layanan Terminal.</span><span class="sxs-lookup"><span data-stu-id="dcd2c-113">Remote Desktop Services (RDS) was previously named Terminal Services.</span></span>
  