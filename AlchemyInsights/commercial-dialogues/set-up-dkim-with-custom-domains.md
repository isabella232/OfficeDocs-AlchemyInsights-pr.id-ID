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
ms.openlocfilehash: cb1f621dffc88464c339b55998efb5440cfd775c
ms.sourcegitcommit: ab75f66355116e995b3cb5505465b31989339e28
ms.translationtype: MT
ms.contentlocale: id-ID
ms.lasthandoff: 08/13/2021
ms.locfileid: "58332310"
---
# <a name="set-up-dkim-with-custom-domains"></a>Menyiapkan DKIM dengan domain kustom

Anda harus menerbitkan dua catatan CNAME untuk setiap domain kustom dalam DNS. Untuk melakukan ini, gunakan format berikut ini:

```console
Host name:            selector1._domainkey
Points to address or value:    selector1-<domainGUID>._domainkey.<initialDomain>
TTL:                3600

Host name:            selector2._domainkey
Points to address or value:    selector2-<domainGUID>._domainkey.<initialDomain>
TTL:                3600
```
**Catatan:** **DomainGUID** adalah teks di sebelah kiri **.mail.protection.outlook.com** dalam rekaman MX yang dikustomisasi untuk domain kustom (misalnya, contoso-com untuk domain **contoso.com**). **InitialDomain** adalah domain yang Anda gunakan saat Anda mendaftar Office 365 (misalnya, **contoso.onmicrosoft.com**).

Untuk informasi selengkapnya tentang catatan DNS, lihat [Membuat catatan DNS di penyedia hosting DNS apa pun untuk Office 365](https://docs.microsoft.com/microsoft-365/admin/get-help-with-domains/create-dns-records-at-any-dns-hosting-provider).