---
title: Memperbaiki masalah pengaturan DKIM
ms.author: chrisda
author: chrisda
manager: dansimp
ms.date: ''
ms.audience: ITPro
ms.topic: article
ROBOTS: NOINDEX, NOFOLLOW
localization_priority: Normal
ms.custom: 1389
ms.assetid: ''
ms.openlocfilehash: 4d6dadbcbf71fe6e9ea56d6a82a7d8ababdd38ef
ms.sourcegitcommit: 4b7e478ce700c0b781efec3857ac4dce5bdf00c6
ms.translationtype: MT
ms.contentlocale: id-ID
ms.lasthandoff: 06/07/2019
ms.locfileid: "34765153"
---
# <a name="fix-dkim-setup-issues"></a>Memperbaiki masalah pengaturan DKIM

Jika Anda mengalami masalah yang memungkinkan DKIM untuk domain kustom, gunakan langkah-langkah berikut:

- Sebagian besar masalah pengaturan DKIM yang terkait dengan data DNS yang salah. Pastikan DKIM data CNAME (**bukan** data TXT) diformat dengan benar. Untuk selengkapnya, lihat [topik](https://docs.microsoft.com/office365/SecurityCompliance/use-dkim-to-validate-outbound-email#what-you-need-to-do-to-manually-set-up-dkim-in-office-365)ini.

- Setelah membuat atau memperbarui data DKIM dengan DNS pada layanan hosting DNS untuk domain Anda (biasanya, registrar domain), menunggu data DNS untuk menyebarkan.

- Jika Anda tidak dapat membuat data DKIM DNS di pusat admin, Anda dapat mengganti \<CustomDomain\> dengan domain kustom (misalnya, contoso.com) dan menjalankan perintah ini di [PowerShell Online asing](https://docs.microsoft.com/powershell/exchange/exchange-online/connect-to-exchange-online-powershell/connect-to-exchange-online-powershell): `New-DkimSigningConfig -DomainName <CustomDomain> -Enabled $true`.
