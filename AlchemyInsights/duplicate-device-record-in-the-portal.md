---
title: Duplikat catatan perangkat di portal
ms.author: pebaum
author: pebaum
manager: mnirkhe
ms.audience: Admin
ms.topic: article
ROBOTS: NOINDEX, NOFOLLOW
localization_priority: Priority
ms.collection: Adm_O365
ms.custom:
- "9001495"
- "4386"
ms.openlocfilehash: 277afc59705e6040f0f9ae0c8cad965bd7d3ef65
ms.sourcegitcommit: 89ae9e8b36d1980f89f07b016fff0ec48f96b620
ms.translationtype: HT
ms.contentlocale: id-ID
ms.lasthandoff: 04/23/2020
ms.locfileid: "43789865"
---
# <a name="duplicate-device-record-in-the-portal"></a>Duplikat catatan perangkat di portal

Anda mungkin melihat 2 catatan untuk sebuah perangkat di portal jika perangkat tersebut tidak melaporkan status pengelolaan bersama dengan benar ke situs Pengelola Konfigurasi. Untuk memeriksa status pengelolaan bersama perangkat, tinjau kolom **Dikelola Bersama** untuk perangkat di konsol Pengelola Konfigurasi. Jika kolom tidak terlihat, Anda dapat menambahkannya dengan mengklik kanan header kolom mana saja, lalu memilihnya dari daftar.

Nilai Dikelola Bersama harus **Ya**. Jika nilainya **Tidak**, buka applet klien Pengelola Konfigurasi di perangkat klien dan periksa properti **Pengelolaan Bersama** di tab Umum.

- Jika nilainya **Diaktifkan**, ini menunjukkan masalah ada pada komunikasi klien dengan Titik Pengelolaan. Tinjau **CcmMessaging.log** pada perangkat untuk menyelidiki potensi masalah konektivitas.

- Jika nilainya **Dinonaktifkan** dan perangkat terdaftar di Intune, pastikan bahwa perangkat telah menerima kebijakan Pengelolaan Bersama dengan meninjau **CoManagementHandler.log** di perangkat.
