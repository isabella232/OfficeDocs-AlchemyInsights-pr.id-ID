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
# <a name="error-while-activation-office-2013-on-remote-desktop-services"></a>Galat saat aktivasi Office 2013 pada layanan desktop jarak jauh

Jika Anda menerima pesan kesalahan saat mengaktifkan Office 2013 pada penyebaran layanan desktop jarak jauh (RDS), pertimbangkan untuk mengaktifkan ADAL dengan mengedit registri.
  
|**Kunci registri**|**Jenis**|**Nilai**|
|:-----|:-----|:-----|
|HKEY_CURRENT_USER \Software\Microsoft\Office\15.0\Common\Identity\EnableADAL  <br/> |REG_DWORD  <br/> |1  <br/> |

Untuk informasi selengkapnya, lihat [mengaktifkan otentikasi modern untuk Office 2013 pada perangkat Windows](https://docs.microsoft.com/office365/admin/security-and-compliance/enable-modern-authentication).
  
> [!NOTE]
>  ADAL diaktifkan secara default di Microsoft 365 aplikasi untuk perusahaan dan Office 2016. Layanan desktop jarak jauh (RDS) sebelumnya bernama layanan terminal.
  