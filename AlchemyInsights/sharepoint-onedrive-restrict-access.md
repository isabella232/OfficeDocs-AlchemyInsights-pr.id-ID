---
title: Membatasi akses dalam SharePoint atau OneDrive
ms.author: kirks
author: Techwriter40
ms.date: 8/7/2018
ms.audience: ITPro
ms.topic: article
ROBOTS: NOINDEX, NOFOLLOW
localization_priority: Normal
ms.assetid: af1b936b-0475-497b-a6d3-e671aef7b717
ms.openlocfilehash: 84f2d4b6e5fd2380a2fa96e30953c68aab203cd3
ms.sourcegitcommit: 1d98db8acb9959aba3b5e308a567ade6b62da56c
ms.translationtype: MT
ms.contentlocale: id-ID
ms.lasthandoff: 08/22/2019
ms.locfileid: "36559880"
---
# <a name="restrict-access-in-sharepoint-or-onedrive"></a>Membatasi akses dalam SharePoint atau OneDrive

Ada banyak cara untuk membatasi akses ke Layanan SharePoint Online/OneDrive. Pembatasan akses ini berbagai metode adalah sebagai berikut. 

**Izin pembatasan**

SharePoint Online dan OneDrive untuk bisnis, kami membatasi akses ke barang-barang seperti situs, file dan folder dengan hanya memberikan akses ke kelompok/individu yang harus memiliki akses.

- [Mengubahsuaikan izin untuk daftar SharePoint atau Perpustakaan](https://support.office.com/article/Customize-permissions-for-a-SharePoint-list-or-library-02d770f3-59eb-4910-a608-5f84cc297782)

- [Mengubahsuaikan izin situs SharePoint](https://docs.microsoft.com/sharepoint/customize-sharepoint-site-permissions)

- [Mengubah hak akses subfolder](https://support.office.com/article/Change-the-permissions-on-a-subfolder-5427BD7C-F20A-4F75-8CF2-5359DD45A1A6)

- [Kontrol akses dari unmanaged perangkat](https://docs.microsoft.com/sharepoint/control-access-from-unmanaged-devices)

Sebagai SharePoint atau admin global di Office 365, Anda dapat memblokir atau membatasi akses ke konten SharePoint dan OneDrive dari unmanaged perangkat (mereka tidak hibrida iklan bergabung atau compliant di Intune).

**Pembatasan lokasi jaringan**

Sebagai seorang IT admin, Anda dapat mengontrol akses ke sumber daya SharePoint dan OneDrive, berdasarkan jaringan didefinisikan lokasi yang Anda percaya. Hal ini juga dikenal sebagai kebijakan berbasis lokasi. Untuk informasi lebih lanjut, silakan lihat [kontrol akses ke SharePoint Online dan data OneDrive berdasarkan lokasi jaringan](https://docs.microsoft.com/sharepoint/control-access-based-on-network-location)

**Situs kunci pembatasan** 

Dalam SharePoint Online Anda memiliki kemampuan untuk mengunci situs koleksi, jadi tidak ada yang memiliki akses. Ini ditetapkan melalui PowerShell dan [SharePoint Online Management Shell](https://docs.microsoft.com/powershell/sharepoint/sharepoint-online/connect-sharepoint-online?view=sharepoint-ps) menggunakan [Set-SPOSite](https://docs.microsoft.com/powershell/module/sharepoint-online/set-sposite?view=sharepoint-ps) - LockState properti.

**Membatasi user dari menciptakan situs atau subsites**

Sebagai SharePoint admin atau admin global Office 365, Anda dapat membiarkan pengguna membuat dan mengelola sendiri situs SharePoint, menentukan apa jenis situs mereka dapat membuat, dan menentukan lokasi situs. Untuk selengkapnya, lihat [mengelola situs penciptaan dalam SharePoint Online](https://docs.microsoft.com/sharepoint/manage-site-creation)

