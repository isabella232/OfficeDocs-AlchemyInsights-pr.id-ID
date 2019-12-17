---
title: Pelambatan SharePoint online
ms.author: pebaum
author: pebaum
ms.date: 9/17/2018
ms.audience: ITPro
ms.topic: article
ROBOTS: NOINDEX, NOFOLLOW
localization_priority: Normal
ms.assetid: b376d8ea-50c4-47f0-9720-50d80aa3f7f1
ms.openlocfilehash: 5fdbb315698a58145e5437b0a7b127ce0062a76f
ms.sourcegitcommit: 0f0186044a3597e42ad14c32ca58e7224344dcfa
ms.translationtype: MT
ms.contentlocale: id-ID
ms.lasthandoff: 12/15/2019
ms.locfileid: "40048619"
---
# <a name="sharepoint-online-throttling"></a>Pelambatan SharePoint online

Pengguna akan menerima 503 server sibuk galat saat berusaha menavigasi ke situs SharePoint atau OneDrive. 

Galat ini dapat disebabkan oleh pelambatan dalam Layanan SharePoint. SharePoint Online menggunakan pelambatan untuk mempertahankan kinerja optimal dan keandalan Layanan SharePoint online. Pelambatan membatasi jumlah tindakan pengguna atau panggilan bersamaan (dengan skrip atau kode) untuk mencegah penggunaan sumber daya berlebihan. Jika Anda mendapatkan throttled, 99% dari waktu itu karena kode kustom.

Untuk informasi lebih lanjut tentang pelambatan Lihat, [Hindari mendapatkan mengalami kelambatan atau diblokir di SharePoint online](https://docs.microsoft.com/sharepoint/dev/general-development/how-to-avoid-getting-throttled-or-blocked-in-sharepoint-online).

Jika Anda yakin galat ini tidak terkait dengan throttling, Anda dapat memeriksa apakah ada pemeliharaan aktif yang terjadi pada penyewa Anda dengan menavigasi ke [pusat pesan](https://portal.office.com/adminportal/home#/MessageCenter).

 Akhirnya, pastikan Anda mengunjungi halaman [layanan kesehatan](https://portal.office.com/adminportal/home#/servicehealth) untuk memeriksa setiap saran/insiden yang mungkin terjadi.

