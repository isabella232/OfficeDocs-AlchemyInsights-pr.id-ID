---
title: Gambar pengguna masih muncul di Microsoft Teams organisasi
ms.author: pebaum
author: pebaum
manager: scotv
ms.date: 09/13/2021
ms.audience: Admin
ms.topic: article
ms.service: o365-administration
ROBOTS: NOINDEX, NOFOLLOW
localization_priority: Priority
ms.collection: Adm_O365
ms.custom:
- "13834"
- "9007457"
ms.openlocfilehash: be4c6feb55e6b7c4667566946d8d3640cc0ffb1d
ms.sourcegitcommit: b47c6d5e74819b73becaf1dc5eacc72eaf7c1055
ms.translationtype: MT
ms.contentlocale: id-ID
ms.lasthandoff: 09/15/2021
ms.locfileid: "59422251"
---
# <a name="user-picture-still-appears-in-the-microsoft-teams-organization-chart"></a>Gambar pengguna masih muncul di Microsoft Teams organisasi

Jika satu atau beberapa orang di organisasi Anda telah dinonaktifkan atau dihapus, dan foto profil mereka masih muncul di bagan organisasi, ada kemungkinan pengaturan **ShowInAddressLists** diatur ke False: 

1. Masuk ke pusat admin Microsoft 365 > [Pengguna Aktif](https://admin.microsoft.com/Adminportal/Home?source=applauncher#/users) dan pilih pengguna dengan foto yang masih muncul. 
1. Pilih tab **Email,** dan pastikan **Perlihatkan di daftar alamat global** diatur ke **Tidak.**

Jika mengatur **ShowInAddressLists** **menjadi** Tidak tidak berfungsi, periksa hal berikut: 

- Pengguna mungkin diperlihatkan dari daftar penerima dalam Exchange. Untuk informasi selengkapnya, lihat [Mengelola daftar alamat di Exchange Online](https://docs.microsoft.com/exchange/address-books/address-lists/manage-address-lists#use-the-eac-to-hide-recipients-from-address-lists). 
- Pengguna mungkin diperlihatkan dari daftar alamat dalam Azure Active Directory. Untuk informasi selengkapnya, lihat [Set-AzureADUser](https://docs.microsoft.com/powershell/module/azuread/set-azureaduser?view=azureadps-2.0). 