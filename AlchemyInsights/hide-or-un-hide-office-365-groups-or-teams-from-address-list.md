---
title: Sembunyikan atau perlihatkan grup atau tim Office 365 dari daftar alamat
ms.author: pebaum
author: pebaum
manager: scotv
ms.audience: Admin
ms.topic: article
ms.service: o365-administration
ROBOTS: NOINDEX, NOFOLLOW
localization_priority: Priority
ms.collection: Adm_O365
ms.custom:
- "9002947"
- "5642"
ms.openlocfilehash: 7e667e22cd81f38a1a2c1385bf42e5227cb641480f4b505110ee7349a13f13a1
ms.sourcegitcommit: b5f7da89a650d2915dc652449623c78be6247175
ms.translationtype: MT
ms.contentlocale: id-ID
ms.lasthandoff: 08/05/2021
ms.locfileid: "54088399"
---
# <a name="hide-or-un-hide-office-365-groups-or-teams-from-address-list"></a>Sembunyikan atau perlihatkan grup atau tim Office 365 dari daftar alamat

Gunakan perintah EXO PowerShell berikut untuk menyembunyikan atau memperlihatkan grup/tim Office 365 dari daftar alamat (GAL) klien Exchange (Outlook, OWA):

`
    Set-UnifiedGroup -Identity GroupName -HiddenFromAddressListsEnabled:<$true> or <$false>
`

Gunakan perintah EXO PowerShell berikut untuk menyembunyikan atau memperlihatkan grup/tim Office365 dari klien Exchange (Outlook, OWA):

`
    Set-unifiedGroup -Identity GroupName -HiddenFromExchangeClientsEnabled:<$true> or <$false>
`

- Untuk petunjuk selengkapnya, lihat [Menyembunyikan Grup Office 365 dari GAL dan Klien Exchange ](https://docs.microsoft.com/schooldatasync/hide-office-365-groups-from-the-gal).
