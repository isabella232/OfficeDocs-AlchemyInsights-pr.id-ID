---
title: Petunjuk untuk menyembunyikan/menampilkan grup dari daftar alamat
ms.author: pebaum
author: pebaum
manager: mnirkhe
ms.audience: Admin
ms.topic: article
ROBOTS: NOINDEX, NOFOLLOW
localization_priority: Normal
ms.collection: Adm_O365
ms.custom:
- "1200024"
- "3161"
ms.openlocfilehash: 02368d6a06df90d76ee1bd5448819e7ffe12c18c
ms.sourcegitcommit: f28dafa0f727870038f72bc904da926daf4ec07b
ms.translationtype: MT
ms.contentlocale: id-ID
ms.lasthandoff: 06/05/2020
ms.locfileid: "44580012"
---
# <a name="hide-microsoft-365-group-from-address-list-gal"></a>Sembunyikan Microsoft 365 grup dari daftar alamat (GAL)

Untuk menyembunyikan Microsoft 365 grup dari alamat daftar (GAL) klien Exchange (seperti Outlook atau OWA), gunakan perintah berikut di EXO Shell:

`Set-UnifiedGroup -Identity GroupName -HiddenFromAddressListsEnabled:$true`

Untuk menyembunyikan grup Microsoft 365 dari yang terlihat untuk Exchange klien, gunakan perintah berikut di EXO Shell:

`Set-unifiedGroup -Identity GroupName -HiddenFromExchangeClientsEnabled:$true
Check this article for detailed instructions`

