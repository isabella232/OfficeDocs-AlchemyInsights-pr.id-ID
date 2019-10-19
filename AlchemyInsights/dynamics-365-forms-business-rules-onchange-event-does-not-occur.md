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
ms.openlocfilehash: cbdedd2c5fcf5517243e60e36d86479d6c3f7814
ms.sourcegitcommit: 037331d71f06750d972c0b6278b23bb15c4806ca
ms.translationtype: MT
ms.contentlocale: id-ID
ms.lasthandoff: 10/18/2019
ms.locfileid: "36529022"
---
# <a name="onchange-event-does-not-occur-if-the-field-is-changed-programmatically"></a>Peristiwa OnChange tidak terjadi apabila kolom diubah secara sistematis

Peristiwa *onChange* tidak terjadi apabila kolom diubah secara sistematis menggunakan *atribut.* metode [Setvalue](https://docs.microsoft.com/dynamics365/customer-engagement/developer/clientapi/reference/attributes/setvalue) . Jika Anda ingin aktivitas handler untuk *onChange* peristiwa untuk menjalankan setelah Anda menetapkan nilai Anda harus menggunakan *atribut formcontext. data. entity.* metode [Fireonchange](https://docs.microsoft.com/dynamics365/customer-engagement/developer/clientapi/reference/attributes/fireonchange) dalam kode Anda.

[https://docs.microsoft.com/dynamics365/customer-engagement/developer/clientapi/reference/events/attribute-onchange](https://docs.microsoft.com/dynamics365/customer-engagement/developer/clientapi/reference/events/attribute-onchange)
