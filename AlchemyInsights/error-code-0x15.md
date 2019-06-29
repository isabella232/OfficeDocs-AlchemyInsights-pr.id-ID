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
ms.openlocfilehash: e2249d8ebbd2313c64dda5656a3243fa76d97a9a
ms.sourcegitcommit: 5fb7a4b28859690020efdea630d03e70cc0e6334
ms.translationtype: MT
ms.contentlocale: id-ID
ms.lasthandoff: 06/28/2019
ms.locfileid: "35388248"
---
<span data-ttu-id="4770c-103">Jika Anda menerima kesalahan ketika mengaktifkan kantor 2013 pada Remote Desktop Services (RDS) penyebaran, mempertimbangkan memungkinkan ADAL dengan mengedit registri.</span><span class="sxs-lookup"><span data-stu-id="4770c-103">If you're receiving an error while activating Office 2013 on Remote Desktop Services (RDS) deployments, consider enabling ADAL by editing the registry.</span></span>
  
|<span data-ttu-id="4770c-104">**Kunci registri**</span><span class="sxs-lookup"><span data-stu-id="4770c-104">**Registry key**</span></span>|<span data-ttu-id="4770c-105">**Jenis**</span><span class="sxs-lookup"><span data-stu-id="4770c-105">**Type**</span></span>|<span data-ttu-id="4770c-106">**Nilai**</span><span class="sxs-lookup"><span data-stu-id="4770c-106">**Value**</span></span>|
|:-----|:-----|:-----|
|<span data-ttu-id="4770c-107">HKEY_CURRENT_USER\Software\Microsoft\Office\15.0\Common\Identity\EnableADAL</span><span class="sxs-lookup"><span data-stu-id="4770c-107">HKEY_CURRENT_USER\Software\Microsoft\Office\15.0\Common\Identity\EnableADAL</span></span>  <br/> |<span data-ttu-id="4770c-108">REG_DWORD</span><span class="sxs-lookup"><span data-stu-id="4770c-108">REG_DWORD</span></span>  <br/> |<span data-ttu-id="4770c-109">1</span><span class="sxs-lookup"><span data-stu-id="4770c-109">1</span></span>  <br/> |

<span data-ttu-id="4770c-110">Untuk selengkapnya, lihat [Mengaktifkan otentikasi Modern untuk kantor 2013 pada perangkat Windows](https://docs.microsoft.com/office365/admin/security-and-compliance/enable-modern-authentication).</span><span class="sxs-lookup"><span data-stu-id="4770c-110">For more information, see [Enable Modern Authentication for Office 2013 on Windows devices](https://docs.microsoft.com/office365/admin/security-and-compliance/enable-modern-authentication).</span></span>
  
> [!NOTE]
>  <span data-ttu-id="4770c-111">ADAL diaktifkan secara default di kantor 365 ProPlus dan kantor 2016.</span><span class="sxs-lookup"><span data-stu-id="4770c-111">ADAL is enabled by default in Office 365 ProPlus and Office 2016.</span></span> <span data-ttu-id="4770c-112">> remote Desktop Services (RDS) sebelumnya bernama Layanan Terminal.</span><span class="sxs-lookup"><span data-stu-id="4770c-112">>  Remote Desktop Services (RDS) was previously named Terminal Services.</span></span>
  