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
ms.openlocfilehash: 61ba34e6d554831da712a92401f26fabb02c26b7
ms.sourcegitcommit: 286000b588adef1bbbb28337a9d9e087ec783fa2
ms.translationtype: MT
ms.contentlocale: id-ID
ms.lasthandoff: 04/27/2020
ms.locfileid: "43908347"
---
# <a name="hide-microsoft-365-group-from-address-list-gal"></a>Sembunyikan Microsoft 365 grup dari daftar alamat (GAL)

Untuk menyembunyikan grup Microsoft 365 dari daftar alamat (GAL) klien Exchange (seperti Outlook atau OWA), gunakan perintah berikut di EXO Shell:

`Set-UnifiedGroup -Identity GroupName -HiddenFromAddressListsEnabled:$true`

Untuk menyembunyikan grup Microsoft 365 dari yang terlihat untuk Exchange klien, gunakan perintah berikut di EXO Shell:

`Set-unifiedGroup -Identity GroupName -HiddenFromExchangeClientsEnabled:$true
Check this article for detailed instructions`

