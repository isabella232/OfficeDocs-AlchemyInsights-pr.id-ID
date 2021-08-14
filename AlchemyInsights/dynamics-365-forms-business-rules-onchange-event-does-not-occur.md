---
title: Aturan Dynamics 365 Forms Business - Aturan Bisnis Tidak Berlaku untuk Formulir
ms.author: pebaum
author: pebaum
ms.audience: ITPro
ms.topic: article
ms.service: o365-administration
ROBOTS: NOINDEX, NOFOLLOW
localization_priority: Normal
ms.custom:
- "1926"
- "6200018"
ms.openlocfilehash: 8425918950e1ef6c44f2866e6fa8987fe165536ae21e08ea6a1da880f761d512
ms.sourcegitcommit: b5f7da89a650d2915dc652449623c78be6247175
ms.translationtype: MT
ms.contentlocale: id-ID
ms.lasthandoff: 08/05/2021
ms.locfileid: "53947302"
---
# <a name="onchange-event-does-not-occur-if-the-field-is-changed-programmatically"></a>Kejadian OnChange tidak terjadi jika bidang diubah secara terprogram

Kejadian *OnChange* tidak terjadi jika bidang diubah secara terprogram menggunakan *atribut.* [metode setValue.](https://docs.microsoft.com/dynamics365/customer-engagement/developer/clientapi/reference/attributes/setvalue) Jika Anda ingin penanganan kejadian untuk kejadian *OnChange* berjalan setelah menetapkan nilai, Anda harus menggunakan metode atribut *formContext.data.entity* [fireOnchange](https://docs.microsoft.com/dynamics365/customer-engagement/developer/clientapi/reference/attributes/fireonchange) dalam kode Anda.

[https://docs.microsoft.com/dynamics365/customer-engagement/developer/clientapi/reference/events/attribute-onchange](https://docs.microsoft.com/dynamics365/customer-engagement/developer/clientapi/reference/events/attribute-onchange)
