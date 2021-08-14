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
ms.openlocfilehash: 5b3dc2338843906fbc7151322b82f304b4ed04b28d8ceb349f2705c309cdeae8
ms.sourcegitcommit: b5f7da89a650d2915dc652449623c78be6247175
ms.translationtype: MT
ms.contentlocale: id-ID
ms.lasthandoff: 08/05/2021
ms.locfileid: "53930064"
---
# <a name="fix-common-problems-with-dkim-record-formatting"></a>Memperbaiki masalah umum dengan pemformatan rekaman DKIM

Sebagian besar masalah pengaturan DKIM terkait dengan catatan DNS yang tidak benar.

Untuk memperbaiki masalah pengaturan DKIM, verifikasi bahwa catatan DKIM CNAME (**bukan rekaman** TXT) telah diformat dengan benar. Untuk informasi selengkapnya, lihat [Apa yang perlu Anda lakukan untuk menyiapkan DKIM secara Office 365](https://docs.microsoft.com/microsoft-365/security/office-365-security/use-dkim-to-validate-outbound-email).

Jika Anda membutuhkan bantuan dengan catatan DNS secara umum, lihat [Membuat catatan DNS di penyedia hosting DNS apa pun untuk Office 365](https://docs.microsoft.com/microsoft-365/admin/get-help-with-domains/create-dns-records-at-any-dns-hosting-provider).

> [!NOTE]
> Setelah membuat atau memperbarui catatan DNS DKIM di layanan hosting DNS untuk domain, Tunggu hingga catatan DNS dis propagate.
