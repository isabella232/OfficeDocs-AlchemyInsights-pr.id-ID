---
title: Saluran pribadi
ms.author: pebaum
author: pebaum
manager: mnirkhe
ms.audience: Admin
ms.topic: article
ROBOTS: NOINDEX, NOFOLLOW
localization_priority: Normal
ms.collection: Adm_O365
ms.custom:
- "9001223"
- "3205"
ms.openlocfilehash: be518df0d40123c1f0da6596bd6e2e91a0c2c8fa
ms.sourcegitcommit: 057d87c9d866fa1371d02350420d13774545c028
ms.translationtype: MT
ms.contentlocale: id-ID
ms.lasthandoff: 05/02/2020
ms.locfileid: "44005441"
---
# <a name="private-channels-in-microsoft-teams"></a>Saluran pribadi di Microsoft teams

Saluran privat adalah fitur baru di Microsoft teams. Perhatikan bahwa saluran pribadi tidak dapat dikonversi dari saluran standar atau sebaliknya.

Untuk rincian tentang saluran pribadi, seperti informasi tentang [pembuatan saluran pribadi dan keanggotaan](https://docs.microsoft.com/MicrosoftTeams/private-channels#private-channel-creation-and-membership) dan [situs SharePoint saluran pribadi](https://docs.microsoft.com/MicrosoftTeams/private-channels#private-channel-sharepoint-sites), lihat [saluran pribadi di Microsoft teams](https://docs.microsoft.com/MicrosoftTeams/private-channels). 

**Catatan:** Karena konfigurasi untuk retensi pesan saluran pribadi belum didukung, penyewa dengan kebijakan retensi diaktifkan tidak akan memiliki saluran pribadi diaktifkan secara default. Saluran pribadi dapat diaktifkan di pusat admin teams. Selain itu, perhatikan bahwa meskipun retensi pesan pribadi saluran tidak didukung, Penyimpanan file yang dibagi di saluran pribadi didukung.

**Butuh pemilik tim baru?**

Jika pemilik Channel pribadi Anda keluar, Anda dapat menambahkan pemilik tim baru melalui teams PowerShell.


- Buka [di sini](https://www.powershellgallery.com/packages/MicrosoftTeams/1.0.6) untuk menginstal tim PowerShell.

Berikut adalah cmdlet Anda akan perlu:

`
    Add-TeamChannelUser -GroupId <group_id> -DisplayName "<channel_name>" -User <UPN> -Role Owner
`

Untuk informasi selengkapnya tentang teams PowerShell, lihat [ringkasan teams PowerShell](https://docs.microsoft.com/microsoftteams/teams-powershell-overview).
