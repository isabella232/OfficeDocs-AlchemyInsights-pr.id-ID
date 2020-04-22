---
title: 1065 bantasi alamat IP keluar EOP rangesMC146155
ms.author: chrisda
author: chrisda
manager: dansimp
ms.date: 04/21/2020
ms.audience: ITPro
ms.topic: article
ROBOTS: NOINDEX, NOFOLLOW
localization_priority: Normal
ms.custom: 1065
ms.assetid: bd41784e-8002-428d-bc19-25671cfd34e8
ms.openlocfilehash: f4854c32d970d84f3a0664a9e384dc6e3cd0bfa7
ms.sourcegitcommit: 55eff703a17e500681d8fa6a87eb067019ade3cc
ms.translationtype: MT
ms.contentlocale: id-ID
ms.lasthandoff: 04/22/2020
ms.locfileid: "43704600"
---
# <a name="deprecation-of-eop-outbound-ip-address-ranges"></a>Bantasi rentang alamat IP keluar EOP

Kami telah mendeteksi potensi masalah dengan organisasi Anda yang (jika tidak dikoreksi pada tanggal 26 Oktober, 2018) dapat merusak alur e-mail ke tujuan lokal atau eksternal. Seperti yang telah dikomunikasikan sebelumnya, untuk menyederhanakan manajemen kisaran alamat IP, kami mengkonsolidasikan rentang alamat IP Exchange Online Protection (EOP) yang digunakan untuk mengirim dan menerima email di luar Microsoft 365. Analisis kami menunjukkan bahwa satu atau lebih dari sumber email eksternal atau tujuan yang telah dikonfigurasi di konektor aliran surat tidak menerima sambungan dari kisaran alamat IP yang ditunjukkan [di sini](https://docs.microsoft.com/office365/SecurityCompliance/eop/exchange-online-protection-ip-addresses).

Bertindaklah sebelum Oktober 26 untuk memastikan sumber dan tujuan ini akan menerima koneksi ke dan dari semua [Alamat EOP IP yang diterbitkan](https://docs.microsoft.com/office365/SecurityCompliance/eop/exchange-online-protection-ip-addresses).

Untuk informasi lebih lanjut tentang perubahan ini, silakan lihat pesan pusat posting [MC146155](https://portal.office.com/AdminPortal/home?switchtomodern=true#/MessageCenter?id=MC146155), [MC148620](https://portal.office.com/AdminPortal/home?switchtomodern=true#/MessageCenter?id=MC148620), atau [MC149274](https://portal.office.com/AdminPortal/home?switchtomodern=true#/MessageCenter?id=MC149274).

**Catatan**: jika sebelumnya Anda menggunakan IP atau URL penerbitan melalui HTML, XML, dan RSS untuk pembaruan titik akhir, Anda juga harus bermigrasi ke layanan web baru untuk mengotomatisasi jenis pembaruan ini. Untuk informasi selengkapnya, lihat [microsoft 365 Endpoint kategori dan microsoft 365 alamat IP dan URL layanan web](https://techcommunity.microsoft.com/t5/Office-365-Blog/Announcing-Office-365-endpoint-categories-and-Office-365-IP/ba-p/177638).
