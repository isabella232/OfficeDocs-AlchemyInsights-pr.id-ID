---
title: Instruksi untuk menyembunyikan/memunculkan grup dari daftar alamat
ms.author: pebaum
author: pebaum
manager: scotv
ms.audience: Admin
ms.topic: article
ms.service: o365-administration
ROBOTS: NOINDEX, NOFOLLOW
localization_priority: Normal
ms.collection: Adm_O365
ms.custom:
- "1200024"
- "3161"
ms.openlocfilehash: 4d55866700b9b8494f1f692cd3b865116b96a1bc
ms.sourcegitcommit: 8bc60ec34bc1e40685e3976576e04a2623f63a7c
ms.translationtype: MT
ms.contentlocale: id-ID
ms.lasthandoff: 04/15/2021
ms.locfileid: "51831881"
---
# <a name="hide-microsoft-365-group-from-address-list-gal"></a>Menyembunyikan grup Microsoft 365 dari daftar alamat (GAL)

Untuk menyembunyikan grup Microsoft 365 dari daftar alamat (GAL) klien Exchange (seperti Outlook atau OWA), gunakan perintah berikut di shell EXO:

`Set-UnifiedGroup -Identity GroupName -HiddenFromAddressListsEnabled:$true`

Untuk menyembunyikan grup Microsoft 365 agar tidak terlihat oleh klien Exchange, gunakan perintah berikut di shell EXO:

`Set-unifiedGroup -Identity GroupName -HiddenFromExchangeClientsEnabled:$true
Check this article for detailed instructions`

