---
title: Rangkaian replika
ms.author: v-jmathew
author: v-jmathew
manager: scotv
ms.audience: Admin
ms.topic: article
ms.service: o365-administration
ROBOTS: NOINDEX, NOFOLLOW
localization_priority: Normal
ms.collection: Adm_O365
ms.custom:
- "9004400"
- "9004395"
- "8265"
- "9276"
ms.openlocfilehash: 45cf530c3258fa3c7008c3e8251fdb7b74be6911d0487f58c5ce2530e25ca282
ms.sourcegitcommit: b5f7da89a650d2915dc652449623c78be6247175
ms.translationtype: MT
ms.contentlocale: id-ID
ms.lasthandoff: 08/05/2021
ms.locfileid: "54110683"
---
# <a name="replica-set"></a>Rangkaian replika

AADDS juga disebut sebagai domain terkelola. Ini sebenarnya adalah dua pengontrol domain yang dijalankan dan dikelola oleh backend. Dua DCs tersebut mencakup satu DC utama dan satu replikasi DC. Pencadangan dalam AADDS (domain terkelola) adalah proses otomatis yang dikelola oleh platform Azure. Dalam hal terjadi masalah dengan domain terkelola Anda, dukungan Azure dapat membantu Anda dalam memulihkan dari cadangan.

Anda membuat setiap rangkaian replika di jaringan virtual. Setiap jaringan virtual harus diasingkan ke setiap jaringan virtual lainnya yang menjadi host kumpulan replika domain terkelola. Konfigurasi ini membuat topologi jaringan jala yang mendukung replikasi direktori. Jaringan virtual bisa mendukung beberapa set replika, asalkan setiap rangkaian replika berada dalam subnet virtual yang berbeda.

Untuk detail selengkapnya tentang Kumpulan replika, lihat [Kumpulan Replika Konsep.](https://docs.microsoft.com/azure/active-directory-domain-services/concepts-replica-sets)
