---
title: 0x8004de40 kesalahan ketika meluncurkan OneDrive
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
- "6886"
- "9003837"
ms.openlocfilehash: f689fcf9432e9b356843efe73ed0f79a32735e6f
ms.sourcegitcommit: 1ac3474897abb7c4969e222f934294e05f468536
ms.translationtype: MT
ms.contentlocale: id-ID
ms.lasthandoff: 10/30/2020
ms.locfileid: "48823051"
---
# <a name="0x8004de40-error-when-launching-onedrive"></a>0x8004de40 kesalahan ketika meluncurkan OneDrive

Jika Anda menerima kesalahan **0x8004de40** saat masuk ke OneDrive, reboot komputer saat tersambung ke domain kerja atau sekolah Anda. Jika Anda menerima kesalahan ini setelah reboot, coba ini saat tersambung ke domain kerja atau sekolah Anda:

1. Klik mulai, lalu ketikkan **CMD** atau **command prompt**  dalam kotak pencarian, klik kanan pada aplikasi prompt perintah, lalu pilih  **Jalankan sebagai administrator** . Jika Anda dimintai kata sandi administrator atau untuk konfirmasi, ketikkan kata sandi, atau klik **Perbolehkan** .  

2. Di jendela prompt perintah, ketik **dsregcmd/Leave**  dan tunggu hingga perintah selesai. Lalu ketikkan **dsregcmd/Join** dan tunggu hingga perintah selesai.
3. Hidupkan ulang komputer Anda.
