---
title: Gambar pengguna tidak ditampilkan di Microsoft Teams bagan organisasi
ms.author: pebaum
author: pebaum
manager: scotv
ms.date: 08/23/2021
ms.audience: Admin
ms.topic: article
ms.service: o365-administration
ROBOTS: NOINDEX, NOFOLLOW
localization_priority: Priority
ms.collection: Adm_O365
ms.custom:
- "12620"
- "9007457"
ms.openlocfilehash: 661b04913581ddd6650316298134ff9835ef3a90
ms.sourcegitcommit: 3986fa5377895cfc9fd98aca0739e599ebafb712
ms.translationtype: MT
ms.contentlocale: id-ID
ms.lasthandoff: 08/23/2021
ms.locfileid: "58792757"
---
# <a name="user-picture-not-showing-in-microsoft-teams-organization-chart"></a>Gambar pengguna tidak ditampilkan di Microsoft Teams bagan organisasi

Jika satu atau beberapa orang di organisasi Anda kehilangan foto profil mereka di bagan organisasi, mungkin pengaturan **ShowInAddressLists** diatur ke **False:**

1. Masuk ke pusat admin Microsoft 365 > [**Pengguna Aktif**](https://admin.microsoft.com/Adminportal/Home?source=applauncher#/users), lalu pilih pengguna dengan foto yang hilang. 
1. Pilih tab **Email,** dan pastikan **Perlihatkan di daftar alamat global** diatur ke **Ya.** 

Jika mengatur **ShowInAddressLists** **ke Ya** tidak berfungsi, periksa hal berikut:

- Pengguna mungkin disembunyikan dari daftar penerima di Exchange. Untuk informasi selengkapnya, lihat [Mengelola daftar alamat di Exchange Online](https://docs.microsoft.com/exchange/address-books/address-lists/manage-address-lists#use-the-eac-to-hide-recipients-from-address-lists). 
- Pengguna mungkin disembunyikan dari daftar alamat di Azure Active Directory. Untuk informasi selengkapnya, lihat [Set-AzureADUser](https://docs.microsoft.com/powershell/module/azuread/set-azureaduser?view=azureadps-2.0). 
