---
title: Duplikat catatan perangkat di portal
ms.author: pebaum
author: pebaum
manager: scotv
ms.audience: Admin
ms.topic: article
ms.service: o365-administration
ROBOTS: NOINDEX, NOFOLLOW
localization_priority: Priority
ms.collection: Adm_O365
ms.custom:
- "9001495"
- "4386"
ms.openlocfilehash: e6f477807823e68965ce966faf0a6f50f9472f3d
ms.sourcegitcommit: 8bc60ec34bc1e40685e3976576e04a2623f63a7c
ms.translationtype: HT
ms.contentlocale: id-ID
ms.lasthandoff: 04/15/2021
ms.locfileid: "51814519"
---
# <a name="duplicate-device-record-in-the-portal"></a>Duplikat catatan perangkat di portal

Anda mungkin melihat 2 catatan untuk sebuah perangkat di portal jika perangkat tersebut tidak melaporkan status pengelolaan bersama dengan benar ke situs Pengelola Konfigurasi. Untuk memeriksa status pengelolaan bersama perangkat, tinjau kolom **Dikelola Bersama** untuk perangkat di konsol Pengelola Konfigurasi. Jika kolom tidak terlihat, Anda dapat menambahkannya dengan mengklik kanan header kolom mana saja, lalu memilihnya dari daftar.

Nilai Dikelola Bersama harus **Ya**. Jika nilainya **Tidak**, buka applet klien Pengelola Konfigurasi di perangkat klien dan periksa properti **Pengelolaan Bersama** di tab Umum.

- Jika nilainya **Diaktifkan**, ini menunjukkan masalah ada pada komunikasi klien dengan Titik Pengelolaan. Tinjau **CcmMessaging.log** pada perangkat untuk menyelidiki potensi masalah konektivitas.

- Jika nilainya **Dinonaktifkan** dan perangkat terdaftar di Intune, pastikan bahwa perangkat telah menerima kebijakan Pengelolaan Bersama dengan meninjau **CoManagementHandler.log** di perangkat.
