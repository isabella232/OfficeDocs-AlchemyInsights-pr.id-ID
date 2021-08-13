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
ms.openlocfilehash: af7085890d295cf0c41e11aaf18e404313413100cb8a1134bfac051d5fa26996
ms.sourcegitcommit: b5f7da89a650d2915dc652449623c78be6247175
ms.translationtype: MT
ms.contentlocale: id-ID
ms.lasthandoff: 08/05/2021
ms.locfileid: "53926248"
---
# <a name="hide-microsoft-365-group-from-address-list-gal"></a>Menyembunyikan Microsoft 365 grup dari daftar alamat (GAL)

Untuk menyembunyikan grup Microsoft 365 dari daftar alamat (GAL) klien Exchange (seperti Outlook atau OWA), gunakan perintah berikut di shell EXO:

`Set-UnifiedGroup -Identity GroupName -HiddenFromAddressListsEnabled:$true`

Untuk menyembunyikan grup Microsoft 365 yang terlihat oleh Exchange, gunakan perintah berikut di shell EXO:

`Set-unifiedGroup -Identity GroupName -HiddenFromExchangeClientsEnabled:$true
Check this article for detailed instructions`

