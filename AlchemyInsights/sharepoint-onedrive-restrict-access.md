---
title: Membatasi akses di SharePoint atau OneDrive
ms.author: pebaum
author: pebaum
ms.date: 04/21/2020
ms.audience: ITPro
ms.topic: article
ms.service: o365-administration
ROBOTS: NOINDEX, NOFOLLOW
localization_priority: Normal
ms.assetid: af1b936b-0475-497b-a6d3-e671aef7b717
ms.openlocfilehash: fc6731d5a7747bb4fc8d6cef1b6ac0045d11917d7f97abbb21eea9613b1b1aa2
ms.sourcegitcommit: b5f7da89a650d2915dc652449623c78be6247175
ms.translationtype: MT
ms.contentlocale: id-ID
ms.lasthandoff: 08/05/2021
ms.locfileid: "54093834"
---
# <a name="restrict-access-in-sharepoint-or-onedrive"></a>Membatasi akses di SharePoint atau OneDrive

Ada banyak cara untuk membatasi akses ke SharePoint Online/OneDrive ini. Berikut berbagai metode pembatasan akses yang diuraikan di bawah ini. 

**Pembatasan Izin**

Di SharePoint Online dan OneDrive for Business, kami membatasi akses ke item seperti situs, file, dan folder dengan hanya memberikan akses ke grup/individu yang harus memiliki akses.

- [Mengkustomisasi izin untuk SharePoint pustaka grup](https://support.office.com/article/Customize-permissions-for-a-SharePoint-list-or-library-02d770f3-59eb-4910-a608-5f84cc297782)

- [Mengkustomisasi SharePoint situs Anda](https://docs.microsoft.com/sharepoint/customize-sharepoint-site-permissions)

- [Mengubah izin di subfolder](https://support.office.com/article/Change-the-permissions-on-a-subfolder-5427BD7C-F20A-4F75-8CF2-5359DD45A1A6)

- [Kontrol akses dari perangkat yang tidak dikelola](https://docs.microsoft.com/sharepoint/control-access-from-unmanaged-devices)

Sebagai admin SharePoint global, Anda dapat memblokir atau membatasi akses ke konten SharePoint dan OneDrive dari perangkat yang tidak kelola (yang bukan merupakan gabungan ad hibrid atau mematuhi in Intune).

**Pembatasan Lokasi Jaringan**

Sebagai admin TI, Anda bisa mengontrol akses ke sumber SharePoint dan OneDrive berdasarkan lokasi jaringan yang ditentukan yang Anda percayai. Ini juga dikenal sebagai kebijakan berbasis lokasi. Untuk informasi selengkapnya, silakan lihat [Mengontrol akses ke SharePoint Online OneDrive data berdasarkan lokasi jaringan](https://docs.microsoft.com/sharepoint/control-access-based-on-network-location)

**Pembatasan Penguncian Situs** 

Di SharePoint Online Anda memiliki kemampuan untuk mengunci kumpulan situs, sehingga tidak ada seorang pun yang memiliki akses. Opsi ini diatur melalui PowerShell dan [SharePoint Online Management Shell](https://docs.microsoft.com/powershell/sharepoint/sharepoint-online/connect-sharepoint-online?view=sharepoint-ps) menggunakan properti [Set-SPOSite](https://docs.microsoft.com/powershell/module/sharepoint-online/set-sposite?view=sharepoint-ps) -LockState.

**Membatasi pengguna membuat situs atau subsitus**

Sebagai admin SharePoint atau Admin global, Anda dapat memungkinkan pengguna membuat dan mengelola situs SharePoint mereka sendiri, menentukan jenis situs yang dapat dibuat, dan menentukan lokasi situs. Untuk informasi selengkapnya, silakan lihat [Mengelola pembuatan situs di SharePoint Online](https://docs.microsoft.com/sharepoint/manage-site-creation)

