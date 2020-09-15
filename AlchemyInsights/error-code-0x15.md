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
# <a name="error-while-activation-office-2013-on-remote-desktop-services"></a>Kesalahan saat aktivasi Office 2013 pada layanan desktop jarak jauh

Jika Anda menerima kesalahan saat mengaktifkan Office 2013 di penyebaran layanan desktop jarak jauh (RDS), pertimbangkan untuk mengaktifkan ADAL dengan mengedit registri.
  
|**Kunci registri**|**Mengetikkan**|**Nilainya**|
|:-----|:-----|:-----|
|HKEY_CURRENT_USER \Software\Microsoft\Office\15.0\Common\Identity\EnableADAL  <br/> |REG_DWORD  <br/> |,1  <br/> |

Untuk informasi selengkapnya, lihat [mengaktifkan autentikasi modern untuk Office 2013 di perangkat Windows](https://docs.microsoft.com/microsoft-365/admin/security-and-compliance/enable-modern-authentication).
  
> [!NOTE]
>  ADAL diaktifkan secara default di aplikasi Microsoft 365 untuk perusahaan dan Office 2016. Layanan desktop jarak jauh (RDS) sebelumnya bernama layanan terminal.
  