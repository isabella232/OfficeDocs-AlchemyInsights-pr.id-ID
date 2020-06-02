---
title: Masalah sambungan SharePoint Designer
ms.author: pebaum
author: pebaum
manager: pamgreen
ms.audience: Admin
ms.topic: article
ROBOTS: NOINDEX, NOFOLLOW
localization_priority: Normal
ms.collection: Adm_O365
ms.custom: ''
ms.assetid: f2b1b6b4-10c9-4e83-b9cb-529a0b8a3c55
ms.openlocfilehash: 01ccc6bc28148f397fb6cd2b7a0eaaeb5b51973f
ms.sourcegitcommit: bc7d6f4f3c9f7060d073f5130e1ec856e248d020
ms.translationtype: MT
ms.contentlocale: id-ID
ms.lasthandoff: 06/02/2020
ms.locfileid: "44511547"
---
# <a name="sharepoint-designer-connection-issues"></a>Masalah sambungan SharePoint Designer 

Jika SharePoint Designer mengalami masalah sambungan ke situs SharePoint, silakan coba solusi umum berikut ini.

Langkah 1: verifikasi bahwa 2013 SharePoint Designer diperbarui dengan [SharePoint Designer Paket Layanan 1](https://support.microsoft.com/help/2817441/description-of-microsoft-sharepoint-designer-2013-service-pack-1-sp1) dan [2 Agustus 2016 pemutakhiran untuk 2013 Designer SharePoint](https://support.microsoft.com/help/3114721/august-2-2016-update-for-sharepoint-designer-2013-kb3114721).



Langkah 2: Kosongkan file cache lokal:

1. Tutup SharePoint Designer 2013.

2. Pada komputer lokal, Hapus semua berkas yang ditemukan di setiap folder berikut ini.

    - %APPDATA%\Microsoft\Web server Extensions\Cache
    - % AppData%\microsoft\sharepoint Designer\ProxyAssemblyCache
    - %USERPROFILE%\AppData\Local\Microsoft\WebsiteCache

3. Buka SharePoint Designer 2013 dan masukkan akun lagi untuk melihat apakah ia bekerja.

Langkah 3: [aktifkan otentikasi modern untuk Office 2013 pada perangkat Windows](https://docs.microsoft.com/microsoft-365/admin/security-and-compliance/enable-modern-authentication).

Langkah 4: Administrator akan perlu untuk **mengizinkan skrip kustom** di Tataan Pusat admin SharePoint untuk mengizinkan sambungan SharePoint Designer. Lihat [membolehkan atau mencegah skrip kustom](https://docs.microsoft.com/sharepoint/allow-or-prevent-custom-script) untuk informasi lebih lanjut.


