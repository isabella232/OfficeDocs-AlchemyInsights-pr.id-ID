---
title: Situs modern sebagai situs akar
ms.author: kirks
author: Techwriter40
ms.audience: ITPro
ms.topic: article
ROBOTS: NOINDEX, NOFOLLOW
localization_priority: Normal
ms.assetid: ''
ms.openlocfilehash: 6166493f79379f44b1a9bbbaca6becfe624fe912
ms.sourcegitcommit: 22ce2315c8cf643137ab3420cdc1cda41433d44a
ms.translationtype: MT
ms.contentlocale: id-ID
ms.lasthandoff: 05/14/2019
ms.locfileid: "34057727"
---
# <a name="modern-site-as-root-site"></a>Situs modern sebagai situs akar

[Target Release](https://docs.microsoft.com/en-us/office365/admin/manage/release-options-in-office-365?view=o365-worldwide) pelanggan sekarang dapat mengaktifkan pengalaman situs modern komunikasi di situs klasik akar penyewa SharePoint mereka.

Fitur ini dapat diaktifkan dengan menjalankan cmdlet PowerShell sederhana. Pada keberhasilan pelaksanaan PowerShell command(s), situs akar akan memiliki halaman rumah situs komunikasi baru. Rincian tentang persyaratan PowerShell cmdlet dan fitur tersedia dalam artikel [Aktifkan-SPOCommSite](https://docs.microsoft.com/en-us/powershell/module/sharepoint-online/Enable-SPOCommSite?view=sharepoint-ps). 

Kita akan secara bertahap rolling hal ini, off secara default, untuk pelanggan yang ditargetkan rilis di awal Mei 2019 dan gulungan keluar akan tersedia di seluruh dunia oleh akhir Juni 2019. Lanjutkan untuk merujuk kepada [Pusat pesan](https://admin.microsoft.com/AdminPortal/Home#/MessageCenter) fitur baru lainnya dengan Modern. 

**Penting**: Jangan menghapus situs akar klasik untuk membuat situs komunikasi modern. Hal ini tidak didukung oleh Microsoft. Menghapus situs akar akan membuat semua situs SharePoint dalam organisasi Anda tidak dapat diakses untuk semua pengguna, sampai Anda mengembalikan situs atau membuat situs baru di URL yang sama. 
 
 