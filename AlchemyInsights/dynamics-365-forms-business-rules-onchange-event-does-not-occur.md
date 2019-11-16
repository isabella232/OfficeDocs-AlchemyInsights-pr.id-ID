---
title: Dynamics 365 formulir aturan bisnis-aturan bisnis tidak menembaki formulir
ms.author: pebaum
author: pebaum
ms.audience: ITPro
ms.topic: article
ROBOTS: NOINDEX, NOFOLLOW
localization_priority: Normal
ms.custom:
- "1926"
- "6200018"
ms.openlocfilehash: 3cdd2175083e864b3bffc57a70bb6c6220843fad
ms.sourcegitcommit: b43f77221f47b50c41197a448a9c26c423ce1ad5
ms.translationtype: MT
ms.contentlocale: id-ID
ms.lasthandoff: 11/15/2019
ms.locfileid: "37769342"
---
# <a name="onchange-event-does-not-occur-if-the-field-is-changed-programmatically"></a>Peristiwa OnChange tidak terjadi apabila kolom diubah secara sistematis

Peristiwa *onChange* tidak terjadi apabila kolom diubah secara sistematis menggunakan *atribut.* metode [Setvalue](https://docs.microsoft.com/dynamics365/customer-engagement/developer/clientapi/reference/attributes/setvalue) . Jika Anda ingin event handler untuk *onChange* event untuk menjalankan setelah Anda menetapkan nilai Anda harus menggunakan metode *formcontext. data. entity atribut* [fireonchange](https://docs.microsoft.com/dynamics365/customer-engagement/developer/clientapi/reference/attributes/fireonchange) dalam kode Anda.

[https://docs.microsoft.com/dynamics365/customer-engagement/developer/clientapi/reference/events/attribute-onchange](https://docs.microsoft.com/dynamics365/customer-engagement/developer/clientapi/reference/events/attribute-onchange)
