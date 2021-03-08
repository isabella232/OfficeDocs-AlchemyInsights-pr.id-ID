---
title: Memperbaiki masalah umum dengan pemformatan rekaman DKIM
ms.author: v-smandalika
author: v-smandalika
manager: dansimp
ms.date: 02/23/2021
audience: Admin
ms.topic: article
ms.service: o365-administration
ROBOTS: NOINDEX, NOFOLLOW
localization_priority: Normal
ms.collection: Adm_O365
ms.custom:
- "9002531"
- "7375"
ms.openlocfilehash: 0a59ca1c93121cb4681c0d44b85a9b756c07895b
ms.sourcegitcommit: 78fe9f33438cb0c19f0dab31253b5853b73f4f47
ms.translationtype: MT
ms.contentlocale: id-ID
ms.lasthandoff: 03/05/2021
ms.locfileid: "50524394"
---
# <a name="fix-common-problems-with-dkim-record-formatting"></a>Memperbaiki masalah umum dengan pemformatan rekaman DKIM

Sebagian besar masalah penyiapan DKIM terkait dengan catatan DNS yang tidak benar.

Untuk memperbaiki masalah penyetelan DKIM, verifikasi bahwa catatan CNAME DKIM (**bukan** rekaman txt) diformat dengan benar. Untuk informasi selengkapnya, lihat [apa yang perlu Anda lakukan untuk menyetel DKIM secara manual di Office 365](https://docs.microsoft.com/microsoft-365/security/office-365-security/use-dkim-to-validate-outbound-email).

Jika Anda memerlukan bantuan dengan catatan DNS secara umum, lihat [membuat catatan DNS di penyedia hosting DNS untuk Office 365](https://docs.microsoft.com/microsoft-365/admin/get-help-with-domains/create-dns-records-at-any-dns-hosting-provider).

> [!NOTE]
> Setelah Anda membuat atau memperbarui catatan DNS DKIM Anda di layanan hosting DNS untuk domain Anda, Anda harus menunggu catatan DNS untuk disebarkan.
