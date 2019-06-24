---
title: Memperbaiki kesalahan 0x8004de40 di OneDrive
ms.author: kirks
author: Techwriter40
ms.date: 6/20/2019
ms.audience: ITPro
ms.topic: article
ROBOTS: NOINDEX, NOFOLLOW
localization_priority: Normal
ms.assetid: ''
ms.openlocfilehash: 2256fb66cb7a4e2adcff9fda16a80c87e2997f0c
ms.sourcegitcommit: 8f6a1be929b275faa295ba8aeeae17898a47c3b0
ms.translationtype: MT
ms.contentlocale: id-ID
ms.lasthandoff: 06/21/2019
ms.locfileid: "35133980"
---
# <a name="fix-0x8004de40-error-in-onedrive"></a>Memperbaiki kesalahan 0x8004de40 di OneDrive

Jika Anda menerima kesalahan 0x8004de40 dengan OneDrive:

- Reboot komputer terkena saat terhubung ke domain Acitve direktori.
- Jika reboot tidak mengatasi masalah tersebut, keluar dan bergabung kembali perangkat Anda dari iklan Azure. 

**Catatan**: Anda harus berada di jaringan perusahaan Anda sambil melakukan langkah-langkah berikut. Tidak melakukan langkah-langkah berikut ketika Anda tidak dapat terhubung ke infrastruktur perusahaan Anda (misalnya, saat bepergian). 

- Buka ditinggikan command prompt. 
- Untuk membuka ditinggikan command prompt, klik - **Start**, klik kanan **Prompt Perintah**, dan kemudian klik **Jalankan sebagai administrator**.
- Ketik *dsregcmd /leave* dan tekan **Enter**.
- Ketika selesai, *ketik/Join dsregcmd* dan tekan **Enter**.
- Setelah selesai, tutup command prompt.
- Reboot komputer, dan login ke OneDrive.