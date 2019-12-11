---
title: Tidak dapat mengakses folder publik
ms.author: pebaum
author: pebaum
manager: mnirkhe
ms.audience: Admin
ms.topic: article
ROBOTS: NOINDEX, NOFOLLOW
localization_priority: Normal
ms.collection: Adm_O365
ms.custom:
- "3500007"
- "3462"
ms.openlocfilehash: a9305b175e1ca0b992c014a73705447d67e037bc
ms.sourcegitcommit: cbbd46fa9a32873c5446d9fd5a532cea0300b795
ms.translationtype: MT
ms.contentlocale: id-ID
ms.lasthandoff: 12/10/2019
ms.locfileid: "39959498"
---
# <a name="outlook-cannot-connect-to-public-folders"></a>Outlook tidak dapat menyambung ke folder publik

Jika akses folder publik tidak bekerja untuk beberapa pengguna, cobalah berikut ini:

Menyambung ke EXO PowerShell, dan mengkonfigurasi DefaultPublicFolderMailbox pada account pengguna masalah untuk mencocokkan satu pada akun pengguna bekerja.

Contoh:

Get-kotak surat WorkingUser | ft DefaultPublicFolderMailbox, EffectivePublicFolderMailbox

Set-kotak surat ProblemUser-DefaultPublicFolderMailbox \<nilai dari perintah sebelumnya>

Tunggu setidaknya satu jam agar perubahan diterapkan.