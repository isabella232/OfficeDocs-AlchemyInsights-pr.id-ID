---
title: Memperbaiki masalah penyiapan DKIM
ms.author: chrisda
author: chrisda
manager: dansimp
ms.date: 04/21/2020
ms.audience: ITPro
ms.topic: article
ROBOTS: NOINDEX, NOFOLLOW
localization_priority: Normal
ms.custom: 1389
ms.assetid: ''
ms.openlocfilehash: 8195b0e3fada6da033b2d95b1fc6600e7fa3341e
ms.sourcegitcommit: bc7d6f4f3c9f7060d073f5130e1ec856e248d020
ms.translationtype: MT
ms.contentlocale: id-ID
ms.lasthandoff: 06/02/2020
ms.locfileid: "44506777"
---
# <a name="fix-dkim-setup-issues"></a>Memperbaiki masalah penyiapan DKIM

Jika Anda mengalami masalah saat mengaktifkan DKIM untuk domain kustom, gunakan langkah berikut:

- Sebagian besar masalah penyiapan DKIM terkait dengan data DNS yang salah. Verifikasi data CNAME DKIM (**bukan** data TXT) diformat dengan benar. Untuk informasi lebih lanjut, lihat [topik](https://docs.microsoft.com/microsoft-365/security/office-365-security/use-dkim-to-validate-outbound-email#steps-you-need-to-do-to-manually-set-up-dkim)ini.

- Setelah membuat atau memperbarui data DNS DKIM di layanan hosting DNS untuk domain (biasanya, registrar domain), tunggu hingga data DNS diterapkan.

- Jika Anda tidak dapat membuat data DNS DKIM di pusat admin, Anda dapat mengganti \<CustomDomain\> dengan domain kustom (misalnya, contoso.com) dan menjalankan perintah ini di [Exchange Online PowerShell](https://docs.microsoft.com/powershell/exchange/exchange-online/connect-to-exchange-online-powershell/connect-to-exchange-online-powershell): `New-DkimSigningConfig -DomainName <CustomDomain> -Enabled $true` .
