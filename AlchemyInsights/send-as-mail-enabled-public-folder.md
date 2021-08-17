---
title: Folder Publik Kirim Sebagai Email yang Diaktifkan di EXO
ms.author: chrisda
author: chrisda
manager: dansimp
ms.date: 04/21/2020
ms.audience: ITPro
ms.topic: article
ms.service: o365-administration
ROBOTS: NOINDEX, NOFOLLOW
localization_priority: Normal
ms.custom:
- "1956"
- "3500007"
ms.openlocfilehash: 22aa3e8f46c2ff4f62cb520b9498041dffb9d3a3eb607d788cc97b10bf32dbb5
ms.sourcegitcommit: b5f7da89a650d2915dc652449623c78be6247175
ms.translationtype: MT
ms.contentlocale: id-ID
ms.lasthandoff: 08/05/2021
ms.locfileid: "54052569"
---
# <a name="sendas-mail-enabled-public-folder"></a>Folder Publik SendAs Mail Enabled

Contoh berikut ini menetapkan izin "Kirim Sebagai" untuk folder publik dengan dukungan email NewPF1 kepada pengguna Jason.

Add-RecipientPermission -Identity 'NewPF1' -Trustee "Jason" -AccessRights 'SendAs'

Untuk informasi parameter dan sintaks yang mendetail, lihat Menetapkan izin "Kirim Sebagai" atau "Kirim Atas [Nama" untuk folder publik berkemampuan email.](https://docs.microsoft.com/exchange/collaboration-exo/public-folders/assign-permissions-mail-enabled-pfs)

