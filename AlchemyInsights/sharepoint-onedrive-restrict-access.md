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
ms.openlocfilehash: e9eb1822a7770bc206992cc5fb7e54a5c972b7e2
ms.sourcegitcommit: c6692ce0fa1358ec3529e59ca0ecdfdea4cdc759
ms.translationtype: MT
ms.contentlocale: id-ID
ms.lasthandoff: 09/14/2020
ms.locfileid: "47700458"
---
# <a name="restrict-access-in-sharepoint-or-onedrive"></a>Membatasi akses di SharePoint atau OneDrive

Ada banyak cara untuk membatasi akses ke Layanan SharePoint online/OneDrive. Metode pembatasan akses ini diuraikan di bawah ini. 

**Pembatasan izin**

Di SharePoint online dan OneDrive for Business, kami membatasi akses ke item seperti situs, file, dan folder dengan hanya memberikan akses ke grup/individu yang seharusnya memiliki akses.

- [Mengkustomisasi izin untuk daftar atau pustaka SharePoint](https://support.office.com/article/Customize-permissions-for-a-SharePoint-list-or-library-02d770f3-59eb-4910-a608-5f84cc297782)

- [Mengkustomisasi izin situs SharePoint](https://docs.microsoft.com/sharepoint/customize-sharepoint-site-permissions)

- [Mengubah izin pada subfolder](https://support.office.com/article/Change-the-permissions-on-a-subfolder-5427BD7C-F20A-4F75-8CF2-5359DD45A1A6)

- [Mengontrol akses dari perangkat yang tidak dikelola](https://docs.microsoft.com/sharepoint/control-access-from-unmanaged-devices)

Sebagai admin SharePoint atau global, Anda dapat memblokir atau membatasi akses ke SharePoint dan konten OneDrive dari perangkat yang tidak dikelola (yang bukan iklan hibrid yang digabungkan atau patuh di Intune).

**Pembatasan lokasi jaringan**

Sebagai admin TI, Anda dapat mengontrol akses ke SharePoint dan sumber daya OneDrive berdasarkan lokasi jaringan yang Anda percayai. Ini juga dikenal sebagai kebijakan berbasis lokasi. Untuk informasi selengkapnya, lihat [mengontrol akses ke data SharePoint online dan OneDrive berdasarkan lokasi jaringan](https://docs.microsoft.com/sharepoint/control-access-based-on-network-location)

**Pembatasan kunci situs** 

Dalam SharePoint online, Anda memiliki kemampuan untuk mengunci kumpulan situs, sehingga tidak ada orang yang memiliki akses. Ini diatur melalui PowerShell dan [SharePoint online Management Shell](https://docs.microsoft.com/powershell/sharepoint/sharepoint-online/connect-sharepoint-online?view=sharepoint-ps) menggunakan properti [set-sposite](https://docs.microsoft.com/powershell/module/sharepoint-online/set-sposite?view=sharepoint-ps) -lockstate.

**Membatasi pengguna membuat situs atau subsitus**

Sebagai admin SharePoint atau admin global, Anda bisa memungkinkan pengguna Anda membuat dan mengelola situs SharePoint mereka sendiri, menentukan jenis situs yang dapat mereka buat, dan menentukan lokasi situs. Untuk informasi selengkapnya, lihat [mengelola pembuatan situs di SharePoint online](https://docs.microsoft.com/sharepoint/manage-site-creation)

