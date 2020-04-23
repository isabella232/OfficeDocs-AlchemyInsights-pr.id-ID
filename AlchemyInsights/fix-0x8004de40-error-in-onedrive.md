---
title: Perbaiki kesalahan 0x8004de40 di OneDrive
ms.author: pebaum
author: pebaum
ms.date: 04/21/2020
ms.audience: ITPro
ms.topic: article
ROBOTS: NOINDEX, NOFOLLOW
localization_priority: Normal
ms.assetid: ''
ms.openlocfilehash: 5da4271f242597b195ef61d553fd4a2ffb313025
ms.sourcegitcommit: 55eff703a17e500681d8fa6a87eb067019ade3cc
ms.translationtype: MT
ms.contentlocale: id-ID
ms.lasthandoff: 04/22/2020
ms.locfileid: "43716031"
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