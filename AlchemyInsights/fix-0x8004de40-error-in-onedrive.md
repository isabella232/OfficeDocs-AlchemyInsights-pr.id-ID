---
title: Perbaiki kesalahan 0x8004de40 di OneDrive
ms.author: pebaum
author: Techwriter40
ms.date: 6/20/2019
ms.audience: ITPro
ms.topic: article
ROBOTS: NOINDEX, NOFOLLOW
localization_priority: Normal
ms.assetid: ''
ms.openlocfilehash: aa0e0a63ac1e365a7cdce018626740446040a664
ms.sourcegitcommit: a65d196d00adb70045af5caca9828fe44b951f61
ms.translationtype: MT
ms.contentlocale: id-ID
ms.lasthandoff: 09/04/2019
ms.locfileid: "36755851"
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