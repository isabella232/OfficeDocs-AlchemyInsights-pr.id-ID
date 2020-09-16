---
title: Memperbaiki masalah penyetelan DKIM
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
ms.openlocfilehash: 35e8023d26fe26211e27521ceb8751d2d7fc7a21
ms.sourcegitcommit: c6692ce0fa1358ec3529e59ca0ecdfdea4cdc759
ms.translationtype: MT
ms.contentlocale: id-ID
ms.lasthandoff: 09/14/2020
ms.locfileid: "47744953"
---
# <a name="fix-dkim-setup-issues"></a>Memperbaiki masalah penyetelan DKIM

Jika Anda mengalami masalah dalam mengaktifkan DKIM untuk domain kustom Anda, gunakan langkah-langkah berikut:

- Sebagian besar masalah penyetelan DKIM terkait dengan catatan DNS yang salah. Verifikasi catatan CNAME DKIM (**bukan** rekaman txt) diformat dengan benar. Untuk informasi selengkapnya, lihat [topik](https://docs.microsoft.com/microsoft-365/security/office-365-security/use-dkim-to-validate-outbound-email#steps-you-need-to-do-to-manually-set-up-dkim)ini.

- Setelah Anda membuat atau memperbarui catatan DNS DKIM Anda di layanan hosting DNS untuk domain Anda (biasanya, pencatat domain Anda), tunggulah catatan DNS untuk disebarkan.

- Jika Anda tidak dapat membuat catatan DNS DKIM di pusat admin, Anda bisa mengganti \<CustomDomain\> dengan domain kustom Anda (misalnya, contoso.com) dan menjalankan perintah ini di [Exchange Online PowerShell](https://docs.microsoft.com/powershell/exchange/exchange-online/connect-to-exchange-online-powershell/connect-to-exchange-online-powershell): `New-DkimSigningConfig -DomainName <CustomDomain> -Enabled $true` .
