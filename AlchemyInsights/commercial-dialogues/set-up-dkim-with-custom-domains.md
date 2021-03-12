---
title: Menyiapkan DKIM dengan domain kustom
ms.author: v-smandalika
author: v-smandalika
manager: dansimp
ms.date: 02/22/2021
audience: Admin
ms.topic: article
ms.service: o365-administration
ROBOTS: NOINDEX, NOFOLLOW
localization_priority: Normal
ms.collection: Adm_O365
ms.custom:
- "9002531"
- "7375"
ms.openlocfilehash: c448956f0dad0738f4de7507ec4686c738a90a55
ms.sourcegitcommit: 6312ee31561db36104f32282d019d069ede69174
ms.translationtype: MT
ms.contentlocale: id-ID
ms.lasthandoff: 03/11/2021
ms.locfileid: "50745255"
---
# <a name="set-up-dkim-with-custom-domains"></a>Menyiapkan DKIM dengan domain kustom

Anda harus menerbitkan dua catatan CNAME untuk setiap domain kustom di DNS. Untuk melakukan ini, gunakan format berikut:

```console
Host name:            selector1._domainkey
Points to address or value:    selector1-<domainGUID>._domainkey.<initialDomain>
TTL:                3600

Host name:            selector2._domainkey
Points to address or value:    selector2-<domainGUID>._domainkey.<initialDomain>
TTL:                3600
```
> [!NOTE]
> **Domainguid** adalah teks di sebelah kiri **. mail.Protection.Outlook.com** dalam catatan MX yang dikustomisasi untuk domain kustom (misalnya, contoso-com untuk domain **contoso.com**). **Initialdomain** adalah domain yang Anda gunakan saat mendaftar untuk Office 365 (misalnya, **contoso.onmicrosoft.com**).

Untuk informasi selengkapnya tentang catatan DNS, lihat [membuat catatan DNS di penyedia hosting DNS untuk Office 365](https://docs.microsoft.com/microsoft-365/admin/get-help-with-domains/create-dns-records-at-any-dns-hosting-provider).