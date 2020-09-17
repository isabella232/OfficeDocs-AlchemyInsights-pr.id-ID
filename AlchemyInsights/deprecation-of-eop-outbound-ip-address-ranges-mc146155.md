---
title: penghentian 1065 alamat IP keluar EOP rangesMC146155
ms.author: chrisda
author: chrisda
manager: dansimp
ms.date: 04/21/2020
ms.audience: ITPro
ms.topic: article
ms.service: o365-administration
ROBOTS: NOINDEX, NOFOLLOW
localization_priority: Normal
ms.custom: 1065
ms.assetid: bd41784e-8002-428d-bc19-25671cfd34e8
ms.openlocfilehash: afd725668f906339f4b7d769bb67a4d2ee5a6ac6
ms.sourcegitcommit: c6692ce0fa1358ec3529e59ca0ecdfdea4cdc759
ms.translationtype: MT
ms.contentlocale: id-ID
ms.lasthandoff: 09/15/2020
ms.locfileid: "47806798"
---
# <a name="deprecation-of-eop-outbound-ip-address-ranges"></a>Penghentian rentang alamat IP keluar EOP

Kami telah mendeteksi potensi masalah dengan organisasi Anda yang (jika tidak diperbaiki oleh 26 Oktober, 2018) mungkin memutus aliran email ke tujuan lokal atau eksternal Anda. Seperti yang dikomunikasikan sebelumnya, untuk menyederhanakan manajemen rentang alamat IP, kami mengonsolidasi rentang alamat IP Exchange Online Protection (EOP) yang digunakan untuk mengirim dan menerima email di luar Microsoft 365. Analisis kami menunjukkan bahwa satu atau beberapa sumber atau tujuan email eksternal yang telah Anda konfigurasikan dalam konektor aliran email tidak menerima koneksi dari rentang alamat IP yang diperlihatkan [di sini](https://docs.microsoft.com/office365/SecurityCompliance/eop/exchange-online-protection-ip-addresses).

Bertindak sebelum Oktober 26 untuk memastikan sumber dan tujuan ini akan menerima koneksi ke dan dari semua [Alamat IP EOP yang diterbitkan](https://docs.microsoft.com/office365/SecurityCompliance/eop/exchange-online-protection-ip-addresses).

Untuk informasi selengkapnya tentang perubahan ini, silakan lihat postingan pusat pesan [MC146155](https://portal.office.com/AdminPortal/home?switchtomodern=true#/MessageCenter?id=MC146155), [MC148620](https://portal.office.com/AdminPortal/home?switchtomodern=true#/MessageCenter?id=MC148620), atau [MC149274](https://portal.office.com/AdminPortal/home?switchtomodern=true#/MessageCenter?id=MC149274).

**Catatan**: jika sebelumnya Anda menggunakan penerbitan IP atau URL melalui HTML, XML, dan RSS untuk pembaruan titik akhir, Anda juga harus melakukan migrasi ke layanan web baru untuk mengotomatisasi tipe pembaruan ini. Untuk informasi selengkapnya, lihat [kategori microsoft 365 Endpoint dan alamat IP microsoft 365 dan layanan web URL](https://techcommunity.microsoft.com/t5/Office-365-Blog/Announcing-Office-365-endpoint-categories-and-Office-365-IP/ba-p/177638).
