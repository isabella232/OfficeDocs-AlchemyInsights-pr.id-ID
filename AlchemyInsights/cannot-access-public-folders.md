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
ms.openlocfilehash: a579b89b68bfb8432adfe64b155803eda2c3b086
ms.sourcegitcommit: a3b42ee05224846327d353b48a8c67dab724f6eb
ms.translationtype: MT
ms.contentlocale: id-ID
ms.lasthandoff: 03/21/2020
ms.locfileid: "42891752"
---
# <a name="outlook-cannot-connect-to-public-folders"></a>Outlook tidak dapat menyambung ke folder publik

Jika akses folder publik tidak bekerja untuk beberapa pengguna, cobalah berikut ini:

Sambungkan ke EXO PowerShell dan konfigurasikan parameter DefaultPublicFolderMailbox pada account pengguna masalah untuk mencocokkan parameter pada akun pengguna bekerja.

Contoh:

Get-kotak surat WorkingUser | ft DefaultPublicFolderMailbox, EffectivePublicFolderMailbox

Set-kotak surat ProblemUser-DefaultPublicFolderMailbox \<nilai dari perintah sebelumnya>

Tunggu setidaknya satu jam agar perubahan diterapkan.

Jika masalah tetap ada, ikuti [prosedur ini](https://aka.ms/pfcte) untuk memecahkan masalah akses folder publik menggunakan Outlook.