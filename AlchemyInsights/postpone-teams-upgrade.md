---
title: Menunda pemutakhiran tim
ms.author: pebaum
author: pebaum
manager: mnirkhe
ms.audience: Admin
ms.topic: article
ms.service: o365-administration
ROBOTS: NOINDEX, NOFOLLOW
localization_priority: Normal
ms.collection: Adm_O365
ms.custom:
- "2737"
- "4000006"
ms.openlocfilehash: ae0611df247790200d0192e018ff5f0128f23cb4
ms.sourcegitcommit: c6692ce0fa1358ec3529e59ca0ecdfdea4cdc759
ms.translationtype: MT
ms.contentlocale: id-ID
ms.lasthandoff: 09/14/2020
ms.locfileid: "47741774"
---
# <a name="how-to-postpone-the-microsoft-driven-teams-upgrade"></a>Cara menunda pemutakhiran tim yang didukung Microsoft

**Penting**: kami bisa membantu memperbaiki hal ini untuk Anda menggunakan diagnostik dukungan, tapi kelihatannya Anda tidak menggunakan pusat admin baru. Untuk menggunakan pusat admin baru, geser tombol alih di bagian kanan atas yang bertuliskan **Pusat admin baru** ke kanan. Menggunakan pusat admin baru, klik widget **perlu bantuan?** , ketikkan "tunda pemutakhiran tim", lalu ikuti perintah untuk menjalankan diagnostik.

Jika Anda menerima komunikasi tentang pemutakhiran otomatis berbasis Microsoft dari Skype for Business ke Microsoft teams, dan Anda ingin menunda pemutakhiran otomatis ke yang lebih baru, admin global Anda bisa masuk ke [portal admin teams](https://admin.teams.microsoft.com/dashboard) dan, setelah memilih tombol **refresh status** di bawah Pemutakhiran Microsoft teams, pilih tombol **tunda** . Untuk melihat tanggal baru untuk pemutakhiran otomatis penyewa Anda ke Microsoft teams, refresh halaman portal admin teams.

**Catatan:** Tombol **tunda** hanya akan tersedia jika Anda telah menerima pemberitahuan pusat pesan tentang pemutakhiran otomatis. 

Admin global juga bisa menjalankan [Get-CsTeamsUpgradeStatus](https://docs.microsoft.com/powershell/module/skype/get-csteamsupgradestatus?view=skype-ps) untuk mempelajari selengkapnya tentang status pemutakhiran mereka saat ini.
