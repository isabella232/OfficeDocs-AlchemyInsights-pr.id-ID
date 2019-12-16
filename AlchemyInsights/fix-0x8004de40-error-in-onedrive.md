---
title: Perbaiki kesalahan 0x8004de40 di OneDrive
ms.author: pebaum
author: pebaum
ms.date: 6/20/2019
ms.audience: ITPro
ms.topic: article
ROBOTS: NOINDEX, NOFOLLOW
localization_priority: Normal
ms.assetid: ''
ms.openlocfilehash: 48b29f57763ca22a71a23b2afddcac0e8e8a95db
ms.sourcegitcommit: 0f0186044a3597e42ad14c32ca58e7224344dcfa
ms.translationtype: MT
ms.contentlocale: id-ID
ms.lasthandoff: 12/15/2019
ms.locfileid: "40052040"
---
# <a name="fix-0x8004de40-error-in-onedrive"></a>Perbaiki kesalahan 0x8004de40 di OneDrive

Jika Anda menerima galat 0x8004de40 dengan OneDrive:

- Reboot komputer yang terpengaruh saat tersambung ke domain direktori Acitve Anda.
- Jika reboot tidak memperbaiki masalah, keluar dan bergabung kembali perangkat Anda dari Azure AD. 

**Catatan**: Anda harus berada di jaringan korporat Anda saat melakukan langkah ini. Jangan lakukan langkah ini ketika Anda tidak dapat terhubung ke infrastruktur perusahaan Anda (misalnya, saat bepergian). 

- Buka wantian perintah yang ditinggikan. 
- Untuk membuka wantian perintah yang ditinggikan, klik- **mulai**, klik kanan **wantian perintah**, dan kemudian klik **Jalankan sebagai administrator**.
- Ketik *dsregcmd/Leave* dan tekan **Enter**.
- Setelah selesai, ketik *dsregcmd/Join* dan tekan **Enter**.
- Setelah selesai, tutup wantian perintah.
- Reboot komputer, dan masuk ke OneDrive.