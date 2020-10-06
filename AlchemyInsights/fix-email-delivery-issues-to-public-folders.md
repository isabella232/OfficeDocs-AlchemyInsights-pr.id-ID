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
ms.openlocfilehash: 74a26306766ed7952a3bbbcb06f1f0113a113024
ms.sourcegitcommit: 9fd002ce49ad9a7e58c3eb997a8063e2e1feab55
ms.translationtype: MT
ms.contentlocale: id-ID
ms.lasthandoff: 10/06/2020
ms.locfileid: "48366467"
---
# <a name="fix-email-delivery-issues-to-mail-enabled-public-folders"></a>Memperbaiki masalah pengiriman email ke folder publik email aktif

Jika pengirim eksternal tidak dapat mengirim pesan ke folder publik yang mendukung email Anda, dan pengirim menerima kesalahan: **tidak dapat ditemukan (550 5.4.1)**, verifikasi domain email untuk folder publik dikonfigurasikan sebagai domain relay internal dan bukan domain otoritatif:

1. Buka [Pusat admin Exchange (eac)](https://docs.microsoft.com/Exchange/exchange-admin-center).

2. Masuk ke domain **email** yang \> **diterima**, pilih domain diterima, lalu klik **Edit**.

3. Di halaman properti yang terbuka, jika tipe domain diatur ke **otoritatif**, Ubah nilai ke **relay internal** lalu klik **Simpan**.

Jika pengirim eksternal menerima kesalahan yang **tidak Anda miliki izin (550 5.7.13)**, jalankan perintah berikut di [Exchange Online PowerShell](https://docs.microsoft.com/powershell/exchange/exchange-online/connect-to-exchange-online-powershell/connect-to-exchange-online-powershell) untuk melihat izin untuk pengguna anonim dalam folder publik:

`Get-PublicFolderClientPermission -Identity "<PublicFolderIdentity>" -User Anonymous` Misalnya, `Get-PublicFolderClientPermission -Identity "\Customer Discussion" -User Anonymous` .

Untuk memperbolehkan pengguna eksternal mengirim email ke folder publik ini, tambahkan akses CreateItems ke pengguna anonim. Misalnya, `Add-PublicFolderClientPermission -Identity "\Customer Discussion" -User Anonymous -AccessRights CreateItems` .
