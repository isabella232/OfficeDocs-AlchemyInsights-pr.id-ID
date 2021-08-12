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
ms.openlocfilehash: 23c57356c8bd94c1cbafb538c9318208429754115a7c4e88abc93d293b5ea6e1
ms.sourcegitcommit: b5f7da89a650d2915dc652449623c78be6247175
ms.translationtype: MT
ms.contentlocale: id-ID
ms.lasthandoff: 08/05/2021
ms.locfileid: "53946582"
---
# <a name="0x8004de40-error-when-launching-onedrive"></a>0x8004de40 saat meluncurkan OneDrive

Jika Anda menerima pesan **0x8004de40** masuk ke komputer OneDrive, mulai ulang komputer saat tersambung ke domain kantor atau sekolah Anda. Jika Anda menerima kesalahan ini setelah memulai ulang, coba hal ini saat tersambung ke domain kerja atau sekolah Anda:

1. Klik Mulai, lalu **ketikkan cmd** atau **prompt perintah**  dalam kotak pencarian, klik kanan aplikasi prompt perintah, lalu pilih Jalankan  **sebagai administrator**. Jika Anda dimintai kata sandi administrator atau konfirmasi, ketik kata sandi, atau klik **Perbolehkan.**  

2. Di jendela Prompt Perintah, ketik **dsregcmd /leave**  dan tunggu perintah selesai. Lalu ketik **dsregcmd /join** dan tunggu perintah selesai.
3. Me-reboot komputer Anda.
