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
ms.openlocfilehash: d725eb0d46dcbf1b5b6d77ca9f59fcafa5298bf1
ms.sourcegitcommit: 55eff703a17e500681d8fa6a87eb067019ade3cc
ms.translationtype: MT
ms.contentlocale: id-ID
ms.lasthandoff: 04/22/2020
ms.locfileid: "43717565"
---
# <a name="fix-dkim-setup-issues"></a>Memperbaiki masalah penyiapan DKIM

Jika Anda mengalami masalah saat mengaktifkan DKIM untuk domain kustom, gunakan langkah berikut:

- Sebagian besar masalah penyiapan DKIM terkait dengan data DNS yang salah. Verifikasi data CNAME DKIM (**bukan** data TXT) diformat dengan benar. Untuk informasi lebih lanjut, lihat [topik](https://docs.microsoft.com/office365/SecurityCompliance/use-dkim-to-validate-outbound-email#what-you-need-to-do-to-manually-set-up-dkim-in-office-365)ini.

- Setelah membuat atau memperbarui data DNS DKIM di layanan hosting DNS untuk domain (biasanya, registrar domain), tunggu hingga data DNS diterapkan.

- Jika Anda tidak dapat membuat data DNS DKIM di pusat admin, Anda dapat \<mengganti customdomain\> dengan domain kustom anda (misalnya, contoso.com) dan menjalankan perintah ini di [Exchange Online PowerShell](https://docs.microsoft.com/powershell/exchange/exchange-online/connect-to-exchange-online-powershell/connect-to-exchange-online-powershell):. `New-DkimSigningConfig -DomainName <CustomDomain> -Enabled $true`
