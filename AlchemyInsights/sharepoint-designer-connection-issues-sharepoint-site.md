---
title: Masalah koneksi SharePoint Designer
ms.author: pebaum
author: pebaum
manager: pamgreen
ms.audience: Admin
ms.topic: article
ms.service: o365-administration
ROBOTS: NOINDEX, NOFOLLOW
localization_priority: Normal
ms.collection: Adm_O365
ms.custom: ''
ms.assetid: f2b1b6b4-10c9-4e83-b9cb-529a0b8a3c55
ms.openlocfilehash: 997ba3de58485d4fe6d24b926c33348378af8cd3
ms.sourcegitcommit: c6692ce0fa1358ec3529e59ca0ecdfdea4cdc759
ms.translationtype: MT
ms.contentlocale: id-ID
ms.lasthandoff: 09/14/2020
ms.locfileid: "47727174"
---
# <a name="sharepoint-designer-connection-issues"></a>Masalah koneksi SharePoint Designer 

Jika SharePoint Designer mengalami masalah koneksi ke situs SharePoint, coba solusi umum berikut ini.

Langkah 1: verifikasi bahwa SharePoint Designer 2013 diperbarui dengan [SharePoint Designer Service Pack 1](https://support.microsoft.com/help/2817441/description-of-microsoft-sharepoint-designer-2013-service-pack-1-sp1) dan [pembaruan 2 Agustus 2016 untuk SharePoint Designer 2013](https://support.microsoft.com/help/3114721/august-2-2016-update-for-sharepoint-designer-2013-kb3114721).



Langkah 2: Kosongkan file singgahan lokal:

1. Tutup SharePoint Designer 2013.

2. Di komputer lokal, Hapus semua file yang ditemukan di setiap folder berikut ini.

    - %APPDATA%\Microsoft\Web server Extensions\Cache
    - %APPDATA%\Microsoft\SharePoint Designer\ProxyAssemblyCache
    - %USERPROFILE%\AppData\Local\Microsoft\WebsiteCache

3. Buka SharePoint Designer 2013 dan masukkan akun lagi untuk melihat apakah ia bekerja.

Langkah 3: [Aktifkan autentikasi modern untuk Office 2013 di perangkat Windows](https://docs.microsoft.com/microsoft-365/admin/security-and-compliance/enable-modern-authentication).

Langkah 4: administrator perlu **memperbolehkan skrip kustom** di pengaturan pusat admin SharePoint untuk memperbolehkan koneksi SharePoint Designer. Lihat [memperbolehkan atau mencegah skrip kustom](https://docs.microsoft.com/sharepoint/allow-or-prevent-custom-script) untuk informasi selengkapnya.


