---
title: Memperbaiki masalah penyiapan DKIM
ms.author: chrisda
author: chrisda
manager: dansimp
ms.date: 04/21/2020
ms.audience: ITPro
ms.topic: article
ms.service: o365-administration
ROBOTS: NOINDEX, NOFOLLOW
localization_priority: Normal
ms.custom: 1389
ms.assetid: ''
ms.openlocfilehash: 5a613321ed79e657350ec4d19b1f07ac0a091b227a8268c793a10edd9990d41f
ms.sourcegitcommit: b5f7da89a650d2915dc652449623c78be6247175
ms.translationtype: MT
ms.contentlocale: id-ID
ms.lasthandoff: 08/05/2021
ms.locfileid: "53945934"
---
# <a name="fix-dkim-setup-issues"></a>Memperbaiki masalah penyiapan DKIM

Jika mengalami masalah saat mengaktifkan DKIM untuk domain kustom, gunakan langkah-langkah berikut:

- Sebagian besar masalah penyiapan DKIM terkait dengan catatan DNS yang salah. Verifikasi catatan DKIM CNAME (**bukan catatan** TXT) telah diformat dengan benar. Untuk informasi selengkapnya, lihat topik [ini](https://docs.microsoft.com/microsoft-365/security/office-365-security/use-dkim-to-validate-outbound-email#steps-you-need-to-do-to-manually-set-up-dkim).

- Setelah membuat atau memperbarui catatan DNS DKIM di layanan hosting DNS untuk domain Anda (biasanya, pendaftar domain Anda), tunggu hingga catatan DNS dis propagate.

- Jika tidak dapat membuat catatan DNS DKIM di pusat admin, Anda dapat menggantinya dengan domain kustom (misalnya, contoso.com) dan menjalankan perintah ini \<CustomDomain\> [di Exchange Online PowerShell](https://docs.microsoft.com/powershell/exchange/exchange-online/connect-to-exchange-online-powershell/connect-to-exchange-online-powershell): `New-DkimSigningConfig -DomainName <CustomDomain> -Enabled $true` .
