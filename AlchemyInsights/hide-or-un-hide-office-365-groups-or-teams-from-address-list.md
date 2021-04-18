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
ms.openlocfilehash: 12e221c69775f3dfeed1781b70d3061e1ca0ac3b
ms.sourcegitcommit: 8bc60ec34bc1e40685e3976576e04a2623f63a7c
ms.translationtype: HT
ms.contentlocale: id-ID
ms.lasthandoff: 04/15/2021
ms.locfileid: "51811459"
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
