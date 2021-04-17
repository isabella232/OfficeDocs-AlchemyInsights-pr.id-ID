---
title: Menyambungkan ke modul MSCommerce
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
- "9001212"
- "3529"
ms.openlocfilehash: 8e6819f6d6ff37baab4bdd49cb5a87c32490f841
ms.sourcegitcommit: 8bc60ec34bc1e40685e3976576e04a2623f63a7c
ms.translationtype: MT
ms.contentlocale: id-ID
ms.lasthandoff: 04/15/2021
ms.locfileid: "51829739"
---
# <a name="mscommerce-requires-a-company-or-billing-administrator-account"></a>MSCommerce memerlukan akun Administrator Perusahaan atau Tagihan

Modul MSCommerce memerlukan akun dengan hak istimewa Perusahaan atau Administrator Tagihan. Jika menerima kesalahan berikut, Anda perlu menyambungkan kembali dengan akun lain.

*ErrorMessage - Server jarak jauh mengembalikan kesalahan: (403) Dilarang. ErrorDetails - Di C:\Program Files\WindowsPowerShell\Modules\MSCommerce\1.2\MSCommerce.psm1:216 char:5*<br>
*+&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;HandleError -ErrorContext $_ -CustomErrorMessage "Gagal mencoba ulang ...*<br>
\+&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~<br>
&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;*+ CategoryInfo : NotSpecified: (:) [Write-Error], WriteErrorException*<br>
&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;*+ FullyQualifiedErrorId : Microsoft.PowerShell.Commands.WriteErrorException,HandleError*

Jika akun Anda tidak memiliki hak istimewa Perusahaan atau Administrator Tagihan, hubungi Admin TI Anda.
