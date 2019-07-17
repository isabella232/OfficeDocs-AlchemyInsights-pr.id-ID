---
title: Dynamics 365 membentuk bisnis aturan - aturan bisnis tidak Tembak untuk bentuk
ms.author: pebaum
author: pebaum
ms.audience: ITPro
ms.topic: article
ROBOTS: NOINDEX, NOFOLLOW
localization_priority: Normal
ms.custom:
- "1926"
- "6200018"
ms.openlocfilehash: 4ade8d2f68b465298e2d6efff3eef4f04f25c3bf
ms.sourcegitcommit: a413a0e27ef4ab8c484fa9fccff8bbef381c8b96
ms.translationtype: MT
ms.contentlocale: id-ID
ms.lasthandoff: 07/16/2019
ms.locfileid: "35747923"
---
# <a name="onchange-event-does-not-occur-if-the-field-is-changed-programmatically"></a>OnChange acara tidak terjadi jika bidang berubah pemrograman

Acara *OnChange* tidak terjadi jika bidang berubah pemrograman menggunakan *atribut.* metode [setValue](https://docs.microsoft.com/en-us/dynamics365/customer-engagement/developer/clientapi/reference/attributes/setvalue) . Jika Anda ingin event handler untuk *OnChange* acara untuk menjalankan setelah Anda mengatur nilai Anda harus menggunakan *atribut formContext.data.entity.* [fireOnchange](https://docs.microsoft.com/en-us/dynamics365/customer-engagement/developer/clientapi/reference/attributes/fireonchange) metode dalam kode Anda.

[https://docs.microsoft.com/dynamics365/customer-engagement/developer/clientapi/reference/events/attribute-onchange](https://docs.microsoft.com/en-us/dynamics365/customer-engagement/developer/clientapi/reference/events/attribute-onchange)
