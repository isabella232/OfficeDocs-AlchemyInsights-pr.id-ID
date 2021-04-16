---
title: Ikon daya atau baterai tidak ada di Windows 10
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
- "9002953"
- "5655"
ms.openlocfilehash: 95b68cee58f88d04f02e29477b139f7f583dc0b1
ms.sourcegitcommit: 8bc60ec34bc1e40685e3976576e04a2623f63a7c
ms.translationtype: HT
ms.contentlocale: id-ID
ms.lasthandoff: 04/15/2021
ms.locfileid: "51790551"
---
# <a name="power-or-battery-icon-missing-in-windows-10"></a>Ikon daya atau baterai tidak ada di Windows 10

Jika perangkat Windows 10 memiliki baterai (misalnya, laptop atau tablet, atau PC yang disambungkan melalui USB ke UPS), biasanya ikon daya/baterai ditampilkan di taskbar dekat jam, misalnya:

![Ikon baterai](media/battery-icon.png)

Jika Anda tidak melihat ikon ini, ikon mungkin tersembunyi:

1. Masuk ke **[Pengaturan > Personalisasi > Taskbar](ms-settings:taskbar?activationSource=GetHelp)**.

2. Di area Pemberitahuan, klik **Pilih ikon yang muncul di taskbar**.

3. Lalu, temukan item **Daya** di daftar dan alihkan pengaturannya ke **Aktif**.

    ![Menampilkan ikon daya di Taskbar](media/power-icon-on.png)

**Pemecahan masalah**

Jika Anda telah mengikuti instruksi di atas dan tombol alih **Daya** berwarna abu-abu atau tidak terlihat, di kotak pencarian di taskbar, ketik **device manager**, lalu pilih **Device Manager** di daftar hasil. Di bawah **Baterai**, klik kanan baterai perangkat Anda, klik **Nonaktifkan**, lalu klik **Ya**. Tunggu beberapa detik, lalu klik kanan baterai dan klik **Aktifkan**. Lalu, hidupkan ulang perangkat Anda.

Jika Anda telah mengikuti instruksi di atas, tetapi ikon baterai tidak muncul di taskbar, di kotak pencarian di taskbar, ketik **manajer tugas**, lalu klik **Manajer Tugas** di daftar hasil. Di tab **Proses**, di bawah **Nama**, klik kanan **Explorer**, lalu klik **Hidupkan ulang**.
