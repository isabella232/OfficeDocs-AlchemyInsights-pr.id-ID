---
title: Memperbaiki masalah-masalah pengiriman email ke dukungan e-mail folder publik
ms.author: chrisda
author: chrisda
manager: serdars
ms.date: ''
ms.audience: ITPro
ms.topic: article
ROBOTS: NOINDEX, NOFOLLOW
localization_priority: Normal
ms.custom: 1956
ms.assetid: ''
ms.openlocfilehash: 45665f900014c52e6a920325b0a3b0f6f79fb72d
ms.sourcegitcommit: d1c1d5bcb52ba9083e8dd7603feb72436c5154c8
ms.translationtype: MT
ms.contentlocale: id-ID
ms.lasthandoff: 04/17/2019
ms.locfileid: "31910605"
---
# <a name="fix-email-delivery-issues-to-mail-enabled-public-folders"></a>Memperbaiki masalah-masalah pengiriman email ke dukungan e-mail folder publik

Jika pengirim eksternal tidak dapat mengirim pesan ke folder publik Anda dukungan e-mail, dan pengirim menerima kesalahan: **tidak dapat ditemukan (550 5.4.1)**, verifikasi email domain untuk map publik dikonfigurasi sebagai domain internal relay bukan domain otoritatif:

1. Membuka [Pusat admin pertukaran (EAC)](https://docs.microsoft.com/Exchange/exchange-admin-center).

2. Pergi ke **alur E-mail** \> **domain diterima**, pilih domain diterima, dan kemudian klik **mengedit**.

3. Dalam properti halaman yang terbuka, jika jenis domain diatur ke **Authoritative**, mengubah nilai untuk **Internal relay** dan kemudian klik **Simpan**.

Jika pengirim eksternal menerima kesalahan yang **Anda tidak memiliki izin (550 5.7.13)**, jalankan perintah berikut dalam [Exchange Online PowerShell](https://docs.microsoft.com/powershell/exchange/exchange-online/connect-to-exchange-online-powershell/connect-to-exchange-online-powershell) untuk melihat izin untuk pengguna anonim di map publik:

`Get-PublicFolderClientPermission -Identity "<PublicFolderIdentity>" -User Anonymous`Sebagai contoh, `Get-PublicFolderClientPermission -Identity "\Customer Discussion" -User Anonymous`.

Untuk membolehkan pengguna eksternal mengirim email ke folder publik ini, tambahkan CreateItems akses hak untuk pengguna anonim. Sebagai contoh, `Add-PublicFolderClientPermission -Identity "\Customer Discussion" -User Anonymous -AccessRights CreateItems`.
