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
ms.openlocfilehash: 7eb642f85f437fe216c49ce6b060c9061b477629fbd45f50ca0ef315b8cd32d3
ms.sourcegitcommit: b5f7da89a650d2915dc652449623c78be6247175
ms.translationtype: MT
ms.contentlocale: id-ID
ms.lasthandoff: 08/05/2021
ms.locfileid: "54004157"
---
# <a name="duplicate-device-record-in-the-portal"></a>Duplikat catatan perangkat di portal

Anda mungkin melihat 2 catatan untuk sebuah perangkat di portal jika perangkat tersebut tidak melaporkan status pengelolaan bersama dengan benar ke situs Pengelola Konfigurasi. Untuk memeriksa status pengelolaan bersama perangkat, tinjau kolom **Dikelola Bersama** untuk perangkat di konsol Pengelola Konfigurasi. Jika kolom tidak terlihat, Anda dapat menambahkannya dengan mengklik kanan header kolom mana saja, lalu memilihnya dari daftar.

Nilai Dikelola Bersama harus **Ya**. Jika nilainya **Tidak**, buka applet klien Pengelola Konfigurasi di perangkat klien dan periksa properti **Pengelolaan Bersama** di tab Umum.

- Jika nilainya **Diaktifkan**, ini menunjukkan masalah ada pada komunikasi klien dengan Titik Pengelolaan. Tinjau **CcmMessaging.log** pada perangkat untuk menyelidiki potensi masalah konektivitas.

- Jika nilainya **Dinonaktifkan** dan perangkat terdaftar di Intune, pastikan bahwa perangkat telah menerima kebijakan Pengelolaan Bersama dengan meninjau **CoManagementHandler.log** di perangkat.
