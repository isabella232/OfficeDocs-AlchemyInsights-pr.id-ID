---
title: Kumpulan replika
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
ms.openlocfilehash: 3834696ff59b7e96e90a5b660a489003dfa9729c
ms.sourcegitcommit: 581c696ec108184adae9d4bc8f47cb9247131de8
ms.translationtype: MT
ms.contentlocale: id-ID
ms.lasthandoff: 03/10/2021
ms.locfileid: "50714249"
---
# <a name="replica-set"></a>Kumpulan replika

Tambahkan juga disebut sebagai domain terkelola. Sebenarnya ada dua pengontrol domain yang dijalankan dan dipelihara oleh backend. Dua DCs menyertakan satu DC utama dan satu replikasi DC. Pencadangan di AADDS (domain terkelola) adalah proses otomatis yang dikelola oleh platform Azure. Dalam Kejadian masalah dengan domain terkelola Anda, dukungan Azure dapat membantu Anda memulihkan dari cadangan.

Anda membuat setiap rangkaian replika dalam jaringan virtual. Setiap jaringan virtual harus dipengpeered ke setiap jaringan virtual lainnya yang menghosting kumpulan replika domain terkelola. Konfigurasi ini membuat topologi jaringan mesh yang mendukung replikasi direktori. Jaringan virtual bisa mendukung beberapa kumpulan replika, asalkan setiap rangkaian replika berada dalam subnet virtual berbeda.

Untuk detail selengkapnya tentang kumpulan replika, lihat [rangkaian replika konsep](https://docs.microsoft.com/azure/active-directory-domain-services/concepts-replica-sets).
