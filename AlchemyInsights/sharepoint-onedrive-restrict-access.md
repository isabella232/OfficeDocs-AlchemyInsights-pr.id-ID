---
title: Membatasi akses di SharePoint atau OneDrive
ms.author: pebaum
author: pebaum
ms.date: 8/7/2018
ms.audience: ITPro
ms.topic: article
ROBOTS: NOINDEX, NOFOLLOW
localization_priority: Normal
ms.assetid: af1b936b-0475-497b-a6d3-e671aef7b717
ms.openlocfilehash: 242388af3ae8887616fc123f24502a8e5ac8dfbe
ms.sourcegitcommit: 0f0186044a3597e42ad14c32ca58e7224344dcfa
ms.translationtype: MT
ms.contentlocale: id-ID
ms.lasthandoff: 12/15/2019
ms.locfileid: "40053768"
---
# <a name="restrict-access-in-sharepoint-or-onedrive"></a>Membatasi akses di SharePoint atau OneDrive

Ada banyak cara untuk membatasi akses ke SharePoint online/Layanan OneDrive. Ini berbagai metode pembatasan akses diuraikan di bawah ini. 

**Pembatasan izin**

Di SharePoint online dan OneDrive for Business, kami membatasi akses ke item seperti situs, file, dan folder hanya dengan memberikan akses ke grup/individu yang seharusnya memiliki akses.

- [Menyesuaikan izin untuk SharePoint daftar atau Perpustakaan](https://support.office.com/article/Customize-permissions-for-a-SharePoint-list-or-library-02d770f3-59eb-4910-a608-5f84cc297782)

- [Menyesuaikan izin situs SharePoint](https://docs.microsoft.com/sharepoint/customize-sharepoint-site-permissions)

- [Mengubah izin pada subfolder](https://support.office.com/article/Change-the-permissions-on-a-subfolder-5427BD7C-F20A-4F75-8CF2-5359DD45A1A6)

- [Mengontrol akses dari perangkat yang tidak dikelola](https://docs.microsoft.com/sharepoint/control-access-from-unmanaged-devices)

Sebagai SharePoint atau global admin di Office 365, Anda dapat memblokir atau membatasi akses ke SharePoint dan OneDrive konten dari perangkat yang tidak dikelola (yang tidak hibrida AD bergabung atau sesuai di Intune).

**Pembatasan lokasi jaringan**

Sebagai admin IT, Anda dapat mengontrol akses ke sumber daya SharePoint dan OneDrive berdasarkan lokasi jaringan yang ditentukan yang Anda percayai. Ini juga dikenal sebagai kebijakan berbasis lokasi. Untuk informasi selengkapnya, silakan lihat [kontrol akses ke SharePoint online dan data OneDrive berdasarkan lokasi jaringan](https://docs.microsoft.com/sharepoint/control-access-based-on-network-location)

**Pembatasan kunci situs** 

Dalam SharePoint online Anda memiliki kemampuan untuk mengunci koleksi situs, sehingga tidak ada yang memiliki akses. Ini diatur melalui PowerShell dan [SharePoint online Management Shell](https://docs.microsoft.com/powershell/sharepoint/sharepoint-online/connect-sharepoint-online?view=sharepoint-ps) menggunakan properti [set-sposite](https://docs.microsoft.com/powershell/module/sharepoint-online/set-sposite?view=sharepoint-ps) -lockstate.

**Membatasi pengguna membuat situs atau subsitus**

Sebagai admin SharePoint atau admin global 365 Office, Anda dapat membiarkan pengguna membuat dan mengelola situs SharePoint mereka sendiri, menentukan jenis situs yang dapat mereka buat, dan menentukan lokasi situs. Untuk informasi lebih lanjut, silakan lihat [Kelola pembuatan situs di SharePoint online](https://docs.microsoft.com/sharepoint/manage-site-creation)

