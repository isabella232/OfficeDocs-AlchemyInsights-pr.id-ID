---
title: Tingkat izin SharePoint Online
ms.author: kirks
author: Techwriter40
manager: pamgreen
ms.audience: Admin
ms.topic: article
ROBOTS: NOINDEX, NOFOLLOW
localization_priority: Normal
ms.collection: Adm_O365
ms.custom: ''
ms.assetid: f2b1b6b4-10c9-4e83-b9cb-529a0b8a3c55
ms.openlocfilehash: 356fef8e02f2c1fd9d209c68194685bb0acaa367
ms.sourcegitcommit: 4b7e478ce700c0b781efec3857ac4dce5bdf00c6
ms.translationtype: MT
ms.contentlocale: id-ID
ms.lasthandoff: 06/07/2019
ms.locfileid: "34760696"
---
# <a name="sharepoint-designer-connection-issues"></a>Masalah sambungan SharePoint Designer 

Jika SharePoint Designer mengalami masalah sambungan ke situs SharePoint, silahkan mencoba solusi umum berikut.

Langkah 1: Verifikasikan SharePoint Designer diperbarui.

- [SharePoint Designer 2013](https://www.microsoft.com/download/details.aspx?id=35491)

- [SharePoint Designer Paket Layanan 1 (SP1)](https://support.microsoft.com/help/2817441/description-of-microsoft-sharepoint-designer-2013-service-pack-1-sp1)

- [Pembaruan untuk SharePoint Designer 2013 (KB3114721)](https://support.microsoft.com/help/3114721/august-2-2016-update-for-sharepoint-designer-2013-kb3114721)

Langkah 2: Kosongkan cache lokal file

- Dekat SharePoint desainer 2013.

- Pada komputer lokal, browse ke folder berikut untuk menghapus cache file.

- Klik mulai, jalankan dan menghapus semua file yang ditemukan di bawah masing-masing di bawah lokasi.

%APPDATA%\Microsoft\Web server Extensions\Cache %APPDATA%\Microsoft\SharePoint Designer\ProxyAssemblyCache %USERPROFILE%\AppData\Local\Microsoft\WebsiteCache

Buka SharePoint desainer 2013 dan masukkan account lagi untuk melihat apakah ia bekerja.

Langkah 3: [mengaktifkan otentikasi Modern untuk kantor 2013 pada perangkat Windows](https://docs.microsoft.com/office365/admin/security-and-compliance/enable-modern-authentication?redirectSourcePath=/article/Enable-Modern-Authentication-for-Office-2013-on-Windows-devices-7dc1c01a-090f-4971-9677-f1b192d6c910&view=o365-worldwide)

Langkah 4: Administrator akan perlu untuk membolehkan Custom Script untuk memungkinkan koneksi SharePoint Designer.

Untuk langkah-langkah rinci, contoh dan pertimbangan Lihat [Bolehkan atau mencegah script kustom](https://docs.microsoft.com/sharepoint/allow-or-prevent-custom-script).


