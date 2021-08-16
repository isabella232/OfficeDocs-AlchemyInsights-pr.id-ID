---
title: Penghentian 1065 rentang alamat IP keluar EOPMC146155
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
ms.openlocfilehash: 214abc57a99c70a02a7d159441713e007f6ad980f67e373780d4ca297f69f764
ms.sourcegitcommit: b5f7da89a650d2915dc652449623c78be6247175
ms.translationtype: MT
ms.contentlocale: id-ID
ms.lasthandoff: 08/05/2021
ms.locfileid: "54031265"
---
# <a name="deprecation-of-eop-outbound-ip-address-ranges"></a>Penghentian rentang alamat IP keluar EOP

Kami telah mendeteksi potensi masalah dengan organisasi Anda yang (jika tidak diperbaiki pada 26 Oktober 2018) mungkin aliran email ke tujuan lokal atau eksternal Anda. Seperti yang dikomunikasikan sebelumnya, untuk menyederhanakan manajemen rentang alamat IP, kami menggabungkan rentang alamat IP Exchange Online Protection (EOP) yang digunakan untuk mengirim dan menerima email di luar Microsoft 365. Analisis kami menunjukkan bahwa salah satu atau beberapa sumber email atau tujuan eksternal yang telah Anda konfigurasi dalam konektor alur email tidak menerima koneksi dari rentang alamat IP yang diperlihatkan di [sini](https://docs.microsoft.com/office365/SecurityCompliance/eop/exchange-online-protection-ip-addresses).

Bertindak sebelum 26 Oktober untuk memastikan sumber dan tujuan ini akan menerima koneksi ke dan dari semua alamat [IP EOP yang diterbitkan.](https://docs.microsoft.com/office365/SecurityCompliance/eop/exchange-online-protection-ip-addresses)

Untuk informasi selengkapnya tentang perubahan ini, silakan lihat Postingan Pusat Pesan [MC146155](https://portal.office.com/AdminPortal/home?switchtomodern=true#/MessageCenter?id=MC146155), [MC148620](https://portal.office.com/AdminPortal/home?switchtomodern=true#/MessageCenter?id=MC148620), atau [MC149274](https://portal.office.com/AdminPortal/home?switchtomodern=true#/MessageCenter?id=MC149274).

**Catatan**: Jika sebelumnya menggunakan IP atau URL penerbitan melalui HTML, XML, dan RSS untuk pembaruan titik akhir, Anda juga harus melakukan migrasi ke layanan web baru untuk mengotomatisasi tipe pembaruan ini. Untuk informasi selengkapnya, lihat [Microsoft 365 titik akhir Microsoft 365 layanan web URL dan Alamat IP.](https://techcommunity.microsoft.com/t5/Office-365-Blog/Announcing-Office-365-endpoint-categories-and-Office-365-IP/ba-p/177638)
