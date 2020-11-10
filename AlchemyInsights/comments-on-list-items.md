---
title: Komentar pada item daftar
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
- "9003821"
- "6841"
ms.openlocfilehash: 5940d1a96324c5ca77331485a115689abe547ef7
ms.sourcegitcommit: 534e9217d99336eb471166ff83231c7e408fb1d9
ms.translationtype: MT
ms.contentlocale: id-ID
ms.lasthandoff: 11/09/2020
ms.locfileid: "48982490"
---
# <a name="comments-on-list-items"></a>Komentar pada item daftar

Pengguna akan segera bisa menambahkan dan menghapus komentar pada item daftar. Pengguna dapat melihat semua komentar pada item daftar dan filter di antara tampilan yang memperlihatkan komentar atau aktivitas yang terkait dengan item.

**Pengaturan waktu** :

**Rilis bertarget** : diluncurkan bertahap pada pertengahan Oktober dan diharapkan untuk diselesaikan pada pertengahan November

**Rilis standar** : bertahap diluncurkan pada pertengahan November dan diharapkan untuk diselesaikan pada awal Desember

**Rollout** : rilis bertarget untuk seluruh organisasi

Pengguna perlu memperhatikan hal berikut sebelum mereka bisa menambahkan dan menghapus komentar:

- Komentar mengikuti pengaturan izin yang melekat di SharePoint.
- Daftar klasik yang belum dibuat untuk diperlihatkan dalam antarmuka pengguna modern, seperti daftar tugas, tidak akan memiliki fitur komentar ini.
- Komentar pada daftar di teams tidak tersedia dengan rilis ini.
- Komentar tidak diindeks oleh pencarian.

Admin bisa menonaktifkan fitur ini pada tingkat organisasi dengan mengubah parameter **Commentsonlistitemsdisabled** dalam Cmdlet PowerShell **set-spotenant** .

Saat ini tidak dimungkinkan untuk menonaktifkan komentar pada tingkat situs atau daftar. Kami berharap untuk memiliki kontrol tersebut dalam pembaruan yang lebih baru, mungkin dalam kuartal pertama 2021.
