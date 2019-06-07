---
title: Memperbaiki masalah-masalah pengiriman email ke dukungan e-mail folder publik
ms.author: chrisda
author: chrisda
manager: dansimp
ms.date: ''
ms.audience: ITPro
ms.topic: article
ROBOTS: NOINDEX, NOFOLLOW
localization_priority: Normal
ms.custom: 1956
ms.assetid: ''
ms.openlocfilehash: 900b6cc2765937ee005c7e7dce5d33bbdf582601
ms.sourcegitcommit: 4b7e478ce700c0b781efec3857ac4dce5bdf00c6
ms.translationtype: MT
ms.contentlocale: id-ID
ms.lasthandoff: 06/07/2019
ms.locfileid: "34752672"
---
# <a name="fix-email-delivery-issues-to-mail-enabled-public-folders"></a>Memperbaiki masalah-masalah pengiriman email ke dukungan e-mail folder publik

Jika pengirim eksternal tidak dapat mengirim pesan ke folder publik Anda dukungan e-mail, dan pengirim menerima kesalahan: **tidak dapat ditemukan (550 5.4.1)**, verifikasi email domain untuk map publik dikonfigurasi sebagai domain internal relay bukan domain otoritatif:

1. Membuka [Pusat admin pertukaran (EAC)](https://docs.microsoft.com/Exchange/exchange-admin-center).

2. Pergi ke **alur E-mail** \> **domain diterima**, pilih domain diterima, dan kemudian klik **mengedit**.

3. Dalam properti halaman yang terbuka, jika jenis domain diatur ke **Authoritative**, mengubah nilai untuk **Internal relay** dan kemudian klik **Simpan**.

Jika pengirim eksternal menerima kesalahan yang **Anda tidak memiliki izin (550 5.7.13)**, jalankan perintah berikut dalam [Exchange Online PowerShell](https://docs.microsoft.com/powershell/exchange/exchange-online/connect-to-exchange-online-powershell/connect-to-exchange-online-powershell) untuk melihat izin untuk pengguna anonim di map publik:

`Get-PublicFolderClientPermission -Identity "<PublicFolderIdentity>" -User Anonymous`Sebagai contoh, `Get-PublicFolderClientPermission -Identity "\Customer Discussion" -User Anonymous`.

Untuk membolehkan pengguna eksternal mengirim email ke folder publik ini, tambahkan CreateItems akses hak untuk pengguna anonim. Sebagai contoh, `Add-PublicFolderClientPermission -Identity "\Customer Discussion" -User Anonymous -AccessRights CreateItems`.
