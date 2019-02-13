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
Jika Anda menerima kesalahan ketika mengaktifkan kantor 2013 pada Remote Desktop Services (RDS) penyebaran, mempertimbangkan memungkinkan ADAL dengan mengedit registri. 
  
|**Kunci registri**|**Jenis**|**Nilai**|
|:-----|:-----|:-----|
|HKEY_CURRENT_USER\Software\Microsoft\Office\15.0\Common\Identity\EnableADAL  <br/> |REG_DWORD  <br/> |1  <br/> |
   
Untuk selengkapnya, lihat [Mengaktifkan otentikasi Modern untuk kantor 2013 pada perangkat Windows](https://docs.microsoft.com/office365/admin/security-and-compliance/enable-modern-authentication).
  
> [!NOTE]
>  ADAL diaktifkan secara default di kantor 365 ProPlus dan kantor 2016. > remote Desktop Services (RDS) sebelumnya bernama Layanan Terminal. 
  

