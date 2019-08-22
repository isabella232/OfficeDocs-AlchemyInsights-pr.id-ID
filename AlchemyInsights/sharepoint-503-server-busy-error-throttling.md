---
title: SharePoint Online Throttling
ms.author: kirks
author: Techwriter40
ms.date: 9/17/2018
ms.audience: ITPro
ms.topic: article
ROBOTS: NOINDEX, NOFOLLOW
localization_priority: Normal
ms.assetid: b376d8ea-50c4-47f0-9720-50d80aa3f7f1
ms.openlocfilehash: c7881c0c7331e0aa74fcc439f52157bb75a56160
ms.sourcegitcommit: 1d98db8acb9959aba3b5e308a567ade6b62da56c
ms.translationtype: MT
ms.contentlocale: id-ID
ms.lasthandoff: 08/22/2019
ms.locfileid: "36559844"
---
# <a name="sharepoint-online-throttling"></a>SharePoint Online Throttling

Pengguna dapat menerima 503 server adalah sibuk kesalahan ketika mencoba untuk menavigasi ke situs SharePoint atau OneDrive. 

Kesalahan ini dapat disebabkan oleh throttling dalam Layanan SharePoint. SharePoint Online menggunakan throttling untuk mempertahankan kinerja yang optimal dan keandalan Layanan SharePoint Online. Throttling batas jumlah tindakan pengguna atau bersamaan panggilan (oleh script atau kode) untuk mencegah penggunaan berlebihan sumber daya. Jika Anda mendapatkan mencekik, 99% dari waktu karena kode kustom.

Untuk informasi lebih lanjut tentang throttling Lihat, [Hindari mendapatkan mencekik atau diblokir di SharePoint Online](https://docs.microsoft.com/sharepoint/dev/general-development/how-to-avoid-getting-throttled-or-blocked-in-sharepoint-online).

Jika Anda percaya kesalahan ini tidak berhubungan dengan throttling, Anda dapat memeriksa jika ada pemeliharaan aktif yang terjadi pada penyewa Anda dengan menavigasi ke [pusat pesan](https://portal.office.com/adminportal/home#/MessageCenter).

 Akhirnya, pastikan Anda mengunjungi halaman [Layanan kesehatan](https://portal.office.com/adminportal/home#/servicehealth) untuk memeriksa setiap nasihat/insiden yang mungkin terjadi.

