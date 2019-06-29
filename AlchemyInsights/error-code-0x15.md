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
Jika Anda menerima kesalahan ketika mengaktifkan kantor 2013 pada Remote Desktop Services (RDS) penyebaran, mempertimbangkan memungkinkan ADAL dengan mengedit registri.
  
|**Kunci registri**|**Jenis**|**Nilai**|
|:-----|:-----|:-----|
|HKEY_CURRENT_USER\Software\Microsoft\Office\15.0\Common\Identity\EnableADAL  <br/> |REG_DWORD  <br/> |1  <br/> |

Untuk selengkapnya, lihat [Mengaktifkan otentikasi Modern untuk kantor 2013 pada perangkat Windows](https://docs.microsoft.com/office365/admin/security-and-compliance/enable-modern-authentication).
  
> [!NOTE]
>  ADAL diaktifkan secara default di kantor 365 ProPlus dan kantor 2016. > remote Desktop Services (RDS) sebelumnya bernama Layanan Terminal.
  