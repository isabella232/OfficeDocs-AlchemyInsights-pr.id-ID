---
title: Alamat 1065 bantahan EOP outbound IP rangesMC146155
ms.author: chrisda
author: chrisda
manager: serdars
ms.date: 9/28/2018
ms.audience: ITPro
ms.topic: article
ROBOTS: NOINDEX, NOFOLLOW
localization_priority: Priority
ms.assetid: bd41784e-8002-428d-bc19-25671cfd34e8
ms.openlocfilehash: ec87141ffaa2fa3484620a9b52851e3e92f20b6b
ms.sourcegitcommit: d6ea5e9458a2b8ceaab3ac4bd483e1130b9a398a
ms.translationtype: MT
ms.contentlocale: id-ID
ms.lasthandoff: 01/15/2019
ms.locfileid: "28294857"
---
# <a name="deprecation-of-eop-outbound-ip-address-ranges"></a>Bantahan dari EOP kisaran alamat IP keluar

Kami telah mendeteksi potensi masalah dengan organisasi yang (jika tidak diperbaiki oleh 26 Oktober 2018) mungkin istirahat alur e-mail ke lokal atau tujuan eksternal. Sebagaimana diwartakan sebelumnya, untuk menyederhanakan manajemen kisaran alamat IP, kita sedang mengkonsolidasikan rentang alamat IP perlindungan Online pertukaran (EOP) yang digunakan untuk mengirim dan menerima email di luar Office 365. Analisis kami menunjukkan bahwa satu atau lebih email eksternal sumber atau tujuan yang dikonfigurasi di mail aliran konektor tidak menerima koneksi dari IP alamat rentang ditunjukkan [di sini](https://docs.microsoft.com/office365/SecurityCompliance/eop/exchange-online-protection-ip-addresses).
  
Bertindak sebelum Oktober 26 untuk memastikan sumber dan tujuan ini akan menerima koneksi ke dan dari semua [diterbitkan alamat EOP IP](https://docs.microsoft.com/office365/SecurityCompliance/eop/exchange-online-protection-ip-addresses).
  
Untuk informasi lebih lanjut mengenai perubahan ini, lihat pusat pesan posting [MC146155](https://portal.office.com/AdminPortal/home?switchtomodern=true#/MessageCenter?id=MC146155), [MC148620](https://portal.office.com/AdminPortal/home?switchtomodern=true#/MessageCenter?id=MC148620), atau [MC149274](https://portal.office.com/AdminPortal/home?switchtomodern=true#/MessageCenter?id=MC149274).
  
 **Catatan**: jika Anda sebelumnya menggunakan IP atau URL penerbitan melalui HTML, XML, dan RSS pembaruan endpoint, Anda juga harus memigrasi ke layanan web baru untuk mengotomatisasi jenis update. Untuk informasi lebih lanjut, lihat [kategori endpoint Office 365 dan kantor 365 alamat IP dan URL web layanan](https://techcommunity.microsoft.com/t5/Office-365-Blog/Announcing-Office-365-endpoint-categories-and-Office-365-IP/ba-p/177638).
  

