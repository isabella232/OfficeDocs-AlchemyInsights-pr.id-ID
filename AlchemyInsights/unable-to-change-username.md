---
title: Tidak dapat mengubah nama pengguna
ms.author: pebaum
author: pebaum
manager: scotv
ms.date: 07/24/2020
ms.audience: Admin
ms.topic: article
ROBOTS: NOINDEX, NOFOLLOW
localization_priority: Priority
ms.collection: Adm_O365
ms.custom:
- "1729"
- "9000183"
ms.openlocfilehash: 34aecdf503699ee500179f0958158fc964d77fcb
ms.sourcegitcommit: b10cea11b4975354b91193327b58aa4740d34833
ms.translationtype: MT
ms.contentlocale: id-ID
ms.lasthandoff: 07/28/2020
ms.locfileid: "45439549"
---
# <a name="unable-to-change-username"></a>Tidak dapat mengubah nama pengguna

Dalam beberapa kasus, perubahan UPN (UserPrincipalName) tidak disebarkan ke Cloud. Anda mungkin menerima galat validasi di portal 365 Office atau tidak dapat mengubah nama pengguna atau alamat email. Untuk mengatasi masalah ini, secara manual menetapkan UserPrincipalName menggunakan perintah PowerShell ini.

**Contoh: mengubah nama pengguna**

PowerShellCopy

PS C: \> set-MsolUserPrincipalName-UserPrincipalName "davidc@contoso.com"-NewUserPrincipalName "davidchew@contoso.com"

Perintah ini mengganti nama davidc@contoso.com menjadi davidchew@contoso.com.

Untuk informasi selengkapnya, lihat [set-MsolUserPrincipalName](https://docs.microsoft.com/powershell/module/msonline/set-msoluserprincipalname?view=azureadps-1.0).