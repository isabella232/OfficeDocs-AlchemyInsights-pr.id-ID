---
title: SharePoint Masalah koneksi Designer
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
ms.openlocfilehash: d55f7c1902bb623900fa74bdae70695b6e04ad84ce7b6ea314db614283ec436d
ms.sourcegitcommit: b5f7da89a650d2915dc652449623c78be6247175
ms.translationtype: MT
ms.contentlocale: id-ID
ms.lasthandoff: 08/05/2021
ms.locfileid: "53942028"
---
# <a name="sharepoint-designer-connection-issues"></a>SharePoint Masalah koneksi Designer 

Jika SharePoint Designer mengalami masalah koneksi ke SharePoint Anda, cobalah solusi umum berikut ini.

Langkah 1: Verifikasi bahwa SharePoint Designer 2013 diperbarui dengan [SharePoint Designer Service Pack 1](https://support.microsoft.com/help/2817441/description-of-microsoft-sharepoint-designer-2013-service-pack-1-sp1) dan Pembaruan 2 Agustus [2016 untuk SharePoint Designer 2013](https://support.microsoft.com/help/3114721/august-2-2016-update-for-sharepoint-designer-2013-kb3114721).



Langkah 2: Hapus file cache lokal:

1. Tutup SharePoint Designer 2013.

2. Pada komputer lokal, hapus semua file yang ditemukan dalam setiap folder berikut ini.

    - %APPDATA%\Microsoft\Web Server Extensions\Cache
    - %APPDATA%\Microsoft\SharePoint Designer\ProxyAssemblyCache
    - %USERPROFILE%\AppData\Local\Microsoft\WebsiteCache

3. Buka SharePoint Designer 2013 dan masukkan kembali akun untuk melihat apakah cara kerjanya.

Langkah 3: [Aktifkan Autentikasi Modern untuk Office 2013 di Windows Anda.](https://docs.microsoft.com/microsoft-365/admin/security-and-compliance/enable-modern-authentication)

Langkah 4: Administrator perlu **untuk Memperbolehkan Skrip Kustom** dalam SharePoint Pusat Admin untuk memperbolehkan koneksi SharePoint Designer. Lihat [Memperbolehkan atau mencegah skrip kustom](https://docs.microsoft.com/sharepoint/allow-or-prevent-custom-script) untuk informasi selengkapnya.


