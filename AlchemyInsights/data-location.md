---
title: Lokasi data
ms.author: pebaum
author: pebaum
ms.audience: ITPro
ms.topic: article
ROBOTS: NOINDEX, NOFOLLOW
localization_priority: Normal
ms.custom:
- "945"
- "5300023"
ms.assetid: 3bab036c-dbaa-406a-8b73-1e5f31993436
ms.openlocfilehash: ec8fb91dfe77cb251579ce23eb0579b114b101d9
ms.sourcegitcommit: 358e7ed05c262f909bfa9ed0df730e1fd89266b8
ms.translationtype: MT
ms.contentlocale: id-ID
ms.lasthandoff: 11/27/2019
ms.locfileid: "39627849"
---
# <a name="data-location"></a>Lokasi data

Anda dapat melihat lokasi penyewa Office 365 Anda di pusat admin atau dengan menyambung ke Exchange Online melalui PowerShell.


**Pusat admin:**
1. Masuk ke [Pusat admin](https://admin.microsoft.com/Adminportal/Home).
2. Pilih **pengaturan** > **profil organisasi**.
3. Di bawah **Lokasi data**, pilih **Lihat rincian**.


**Powershell:**
1. Menyambung ke Exchange Online menggunakan Windows PowerShell.
2. Jalankan cmdlet [Get-OrganizationalUnit](https://docs.microsoft.com/powershell/module/exchange/active-directory/get-organizationalunit) untuk menampilkan daftar properti penghuni Anda. 
3. Lihat properti OrganizationId.

Bila Anda memiliki lokasi data untuk EXO dan SPO, Anda dapat menentukan lokasi data untuk layanan lain yang dapat Anda gunakan dari [tempat data Anda berada](https://products.office.com/where-is-your-data-located).