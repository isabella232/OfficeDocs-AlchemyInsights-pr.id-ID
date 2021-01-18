---
title: Menetapkan grup ke peran Azure AD
ms.author: v-smandalika
author: v-smandalika
manager: dansimp
ms.date: 01/15/2021
ms.audience: Admin
ms.topic: article
ms.service: o365-administration
ROBOTS: NOINDEX, NOFOLLOW
localization_priority: Priority
ms.collection: Adm_O365
ms.custom:
- "7898"
- "9003230"
ms.openlocfilehash: feca81fe785bc45e47f6faa876230b5c7701713d
ms.sourcegitcommit: 6dc6f999e840c90694a246b90062950205679420
ms.translationtype: MT
ms.contentlocale: id-ID
ms.lasthandoff: 01/15/2021
ms.locfileid: "49885069"
---
# <a name="assigning-groups-to-azure-ad-role"></a>Menetapkan grup ke peran Azure AD

Untuk menetapkan grup Azure AD dengan sumber kewenangan di Azure AD ke peran Azure AD, lakukan langkah-langkah berikut:

1. Membuat grup baru-untuk membuat grup baru:

    untuk. Masuk ke Pusat admin Azure AD dengan **administrator peran istimewa** atau izin **administrator global** .
    b. Pilih **grup > direktori aktif Azure > semua grup > grup baru**.
    's. Buat grup.

2. Tetapkan peran ke grup selama pembuatan grup atau setelah grup dibuat.

    untuk. Untuk menetapkan peran ke grup pada saat pembuatan grup, Aktifkan tombol Alihkan **AZURE AD bisa ditetapkan ke grup** dan Buat grup.
    b. Untuk menetapkan peran ke grup setelah dibuat, navigasikan ke tab **peran yang ditetapkan** untuk grup yang baru dibuat, dan tetapkan peran ke grup.  

**Mengelola keanggotaan grup yang ditetapkan untuk peran Azure AD**

Untuk mencegah elevasi hak istimewa, secara default, hanya administrator peran istimewa dan administrator global yang bisa mengubah keanggotaan grup yang ditetapkan pada peran. Namun, mereka dapat memilih untuk menetapkan pemilik untuk grup tersebut dan mendelegasikan tugas ini.

Untuk detail selengkapnya tentang penetapan grup awan ke Azure AD, lihat [menetapkan peran iklan ke grup awan](https://docs.microsoft.com/azure/active-directory/roles/groups-concept). Untuk detail selengkapnya tentang pemecahan masalah yang ditetapkan untuk grup awan, lihat [memecahkan masalah yang ditetapkan untuk grup awan](https://docs.microsoft.com/azure/active-directory/roles/groups-faq-troubleshooting).





