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
# <a name="error-while-activation-office-2013-on-remote-desktop-services"></a>Galat saat aktivasi Office 2013 pada layanan desktop jarak jauh

Jika Anda menerima pesan kesalahan saat mengaktifkan Office 2013 pada penyebaran layanan desktop jarak jauh (RDS), pertimbangkan untuk mengaktifkan ADAL dengan mengedit registri.
  
|**Kunci registri**|**Jenis**|**Nilai**|
|:-----|:-----|:-----|
|HKEY_CURRENT_USER \Software\Microsoft\Office\15.0\Common\Identity\EnableADAL  <br/> |REG_DWORD  <br/> |1  <br/> |

Untuk informasi selengkapnya, lihat [mengaktifkan otentikasi modern untuk Office 2013 pada perangkat Windows](https://docs.microsoft.com/microsoft-365/admin/security-and-compliance/enable-modern-authentication).
  
> [!NOTE]
>  ADAL diaktifkan secara default di Microsoft 365 aplikasi untuk perusahaan dan Office 2016. Layanan desktop jarak jauh (RDS) sebelumnya bernama layanan terminal.
  