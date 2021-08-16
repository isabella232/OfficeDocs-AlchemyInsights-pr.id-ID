---
title: Memperbaiki masalah pengiriman email ke folder publik email aktif
ms.author: chrisda
author: chrisda
manager: dansimp
ms.date: 04/21/2020
ms.audience: ITPro
ms.topic: article
ms.service: o365-administration
ROBOTS: NOINDEX, NOFOLLOW
localization_priority: Normal
ms.custom:
- "1956"
- "3500007"
ms.openlocfilehash: ff1400f694ae037a8658356af068b4c20b8fa9d9908dafedb90db7bb6859530f
ms.sourcegitcommit: b5f7da89a650d2915dc652449623c78be6247175
ms.translationtype: MT
ms.contentlocale: id-ID
ms.lasthandoff: 08/05/2021
ms.locfileid: "54068815"
---
# <a name="fix-email-delivery-issues-to-mail-enabled-public-folders"></a>Memperbaiki masalah pengiriman email ke folder publik email aktif

Jika pengirim eksternal tidak bisa mengirim pesan ke folder publik email aktif Anda, dan pengirim menerima kesalahan: tidak bisa ditemukan **(550 5.4.1),** verifikasi bahwa domain email untuk folder publik dikonfigurasi sebagai domain relai internal dan bukan domain otoritatif:

1. Buka pusat [admin Exchange (EAC).](https://docs.microsoft.com/Exchange/exchange-admin-center)

2. Masuk ke **Alur email Domain** \> **yang** diterima , pilih domain yang diterima, lalu klik **Edit.**

3. Di halaman properti yang terbuka, jika tipe domain diatur ke **Otoritatif,** ubah nilai ke **Relay internal** lalu klik **Simpan.**

Jika pengirim eksternal menerima kesalahan Anda tidak memiliki izin **(550 5.7.13),** jalankan perintah berikut di [Exchange Online PowerShell](https://docs.microsoft.com/powershell/exchange/exchange-online/connect-to-exchange-online-powershell/connect-to-exchange-online-powershell) untuk melihat izin bagi pengguna anonim dalam folder publik:

`Get-PublicFolderClientPermission -Identity "<PublicFolderIdentity>" -User Anonymous` Misalnya, `Get-PublicFolderClientPermission -Identity "\Customer Discussion" -User Anonymous` .

Untuk memperbolehkan pengguna eksternal mengirim email ke folder publik ini, tambahkan akses CreateItems langsung ke pengguna Anonim. Misalnya, `Add-PublicFolderClientPermission -Identity "\Customer Discussion" -User Anonymous -AccessRights CreateItems` .
