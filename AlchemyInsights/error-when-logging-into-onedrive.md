---
title: 0x8004de40 saat meluncurkan OneDrive
ms.author: pebaum
author: pebaum
manager: scotv
ms.audience: Admin
ms.topic: article
ms.service: o365-administration
ROBOTS: NOINDEX, NOFOLLOW
localization_priority: Normal
ms.collection: Adm_O365
ms.custom:
- "6886"
- "9003837"
ms.openlocfilehash: e329d7fe881a0fc9514584e06aa2d6e8ebab5b11
ms.sourcegitcommit: 8bc60ec34bc1e40685e3976576e04a2623f63a7c
ms.translationtype: MT
ms.contentlocale: id-ID
ms.lasthandoff: 04/15/2021
ms.locfileid: "51813655"
---
# <a name="0x8004de40-error-when-launching-onedrive"></a>0x8004de40 saat meluncurkan OneDrive

Jika Anda menerima pesan **kesalahan 0x8004de40** masuk ke OneDrive, mulai ulang komputer saat tersambung ke domain kantor atau sekolah Anda. Jika Anda menerima kesalahan ini setelah memulai ulang, coba hal ini saat tersambung ke domain kerja atau sekolah Anda:

1. Klik Mulai, lalu **ketikkan cmd** atau **prompt perintah**  dalam kotak pencarian, klik kanan aplikasi prompt perintah, lalu pilih Jalankan  **sebagai administrator**. Jika Anda dimintai kata sandi administrator atau konfirmasi, ketik kata sandi, atau klik **Perbolehkan.**  

2. Di jendela Prompt Perintah, ketik **dsregcmd /leave**  dan tunggu perintah selesai. Lalu ketik **dsregcmd /join** dan tunggu perintah selesai.
3. Me-reboot komputer Anda.
