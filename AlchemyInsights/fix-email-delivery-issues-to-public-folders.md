---
title: Memperbaiki masalah pengiriman email ke folder publik Surat
ms.author: chrisda
author: chrisda
manager: dansimp
ms.date: 04/21/2020
ms.audience: ITPro
ms.topic: article
ROBOTS: NOINDEX, NOFOLLOW
localization_priority: Normal
ms.custom:
- "1956"
- "3500007"
ms.assetid: ''
ms.openlocfilehash: e261fe60843555fa45927b0a6b36e1ccf79fb028
ms.sourcegitcommit: 55eff703a17e500681d8fa6a87eb067019ade3cc
ms.translationtype: MT
ms.contentlocale: id-ID
ms.lasthandoff: 04/22/2020
ms.locfileid: "43716355"
---
# <a name="fix-email-delivery-issues-to-mail-enabled-public-folders"></a>Memperbaiki masalah pengiriman email ke folder publik Surat

Jika pengirim eksternal tidak dapat mengirim pesan ke folder publik surat Anda, dan pengirim menerima galat: **tidak dapat ditemukan (550 5.4.1)**, verifikasi domain email untuk folder publik dikonfigurasi sebagai domain relay internal dan bukan otoritatif domain:

1. Buka [Exchange Admin Center (eac)](https://docs.microsoft.com/Exchange/exchange-admin-center).

2. Buka \> **domain yang diterima** **aliran e-mail** , pilih domain diterima, lalu klik **Edit**.

3. Di halaman properti yang terbuka, jika jenis domain diatur ke **otoritatif**, Ubah nilai ke **relay internal** , lalu klik **Simpan**.

Jika pengirim eksternal menerima galat **Anda tidak memiliki izin (550 5.7.13)**, jalankan perintah berikut ini di [Exchange Online PowerShell](https://docs.microsoft.com/powershell/exchange/exchange-online/connect-to-exchange-online-powershell/connect-to-exchange-online-powershell) untuk melihat izin untuk pengguna anonim di folder publik:

`Get-PublicFolderClientPermission -Identity "<PublicFolderIdentity>" -User Anonymous`Misalnya, `Get-PublicFolderClientPermission -Identity "\Customer Discussion" -User Anonymous`.

Untuk mengizinkan pengguna eksternal untuk mengirim email ke folder publik ini, tambahkan hak akses CreateItems ke pengguna anonim. Misalnya, `Add-PublicFolderClientPermission -Identity "\Customer Discussion" -User Anonymous -AccessRights CreateItems`.
