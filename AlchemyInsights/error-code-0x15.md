---
title: Kode kesalahan 0x15
ms.author: pebaum
author: pebaum
ms.date: 10/31/2018
ms.audience: ITPro
ms.topic: article
ROBOTS: NOINDEX, NOFOLLOW
localization_priority: Normal
ms.assetid: 0d566afe-b21f-4f1b-8ca9-4b4d3b0f5435
description: Jika Anda menerima kesalahan ketika mengaktifkan kantor 2013 pada Remote Desktop Services (RDS) penyebaran, mempertimbangkan memungkinkan ADAL dengan mengedit registri.
ms.openlocfilehash: 6d4076ecb5c6ee3c3cf4c4610ad4aa29ab477d8a
ms.sourcegitcommit: dd43cc0a9470f98b8ef2a3787c823801d674c666
ms.translationtype: MT
ms.contentlocale: id-ID
ms.lasthandoff: 02/12/2019
ms.locfileid: "29929091"
---
<span data-ttu-id="4e39b-103">Jika Anda menerima kesalahan ketika mengaktifkan kantor 2013 pada Remote Desktop Services (RDS) penyebaran, mempertimbangkan memungkinkan ADAL dengan mengedit registri.</span><span class="sxs-lookup"><span data-stu-id="4e39b-103">If you're receiving an error while activating Office 2013 on Remote Desktop Services (RDS) deployments, consider enabling ADAL by editing the registry.</span></span> 
  
|<span data-ttu-id="4e39b-104">**Kunci registri**</span><span class="sxs-lookup"><span data-stu-id="4e39b-104">**Registry key**</span></span>|<span data-ttu-id="4e39b-105">**Jenis**</span><span class="sxs-lookup"><span data-stu-id="4e39b-105">**Type**</span></span>|<span data-ttu-id="4e39b-106">**Nilai**</span><span class="sxs-lookup"><span data-stu-id="4e39b-106">**Value**</span></span>|
|:-----|:-----|:-----|
|<span data-ttu-id="4e39b-107">HKEY_CURRENT_USER\Software\Microsoft\Office\15.0\Common\Identity\EnableADAL</span><span class="sxs-lookup"><span data-stu-id="4e39b-107">HKEY_CURRENT_USER\Software\Microsoft\Office\15.0\Common\Identity\EnableADAL</span></span>  <br/> |<span data-ttu-id="4e39b-108">REG_DWORD</span><span class="sxs-lookup"><span data-stu-id="4e39b-108">REG_DWORD</span></span>  <br/> |<span data-ttu-id="4e39b-109">1</span><span class="sxs-lookup"><span data-stu-id="4e39b-109">1</span></span>  <br/> |
   
<span data-ttu-id="4e39b-110">Untuk selengkapnya, lihat [Mengaktifkan otentikasi Modern untuk kantor 2013 pada perangkat Windows](https://docs.microsoft.com/office365/admin/security-and-compliance/enable-modern-authentication).</span><span class="sxs-lookup"><span data-stu-id="4e39b-110">For more information, see [Enable Modern Authentication for Office 2013 on Windows devices](https://docs.microsoft.com/office365/admin/security-and-compliance/enable-modern-authentication).</span></span>
  
> [!NOTE]
>  <span data-ttu-id="4e39b-p101">ADAL diaktifkan secara default di kantor 365 ProPlus dan kantor 2016. > remote Desktop Services (RDS) sebelumnya bernama Layanan Terminal.</span><span class="sxs-lookup"><span data-stu-id="4e39b-p101">ADAL is enabled by default in Office 365 ProPlus and Office 2016. >  Remote Desktop Services (RDS) was previously named Terminal Services.</span></span> 
  

