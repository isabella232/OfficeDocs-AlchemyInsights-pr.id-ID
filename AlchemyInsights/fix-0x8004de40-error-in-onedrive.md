---
title: Memperbaiki kesalahan 0x8004de40 di OneDrive
ms.author: pebaum
author: pebaum
ms.date: 04/21/2020
ms.audience: ITPro
ms.topic: article
ms.service: o365-administration
ROBOTS: NOINDEX, NOFOLLOW
localization_priority: Normal
ms.assetid: ''
ms.openlocfilehash: b9bd6dff48f78063e3d47f5fe2f834f59eb9868a
ms.sourcegitcommit: c6692ce0fa1358ec3529e59ca0ecdfdea4cdc759
ms.translationtype: MT
ms.contentlocale: id-ID
ms.lasthandoff: 09/14/2020
ms.locfileid: "47745133"
---
# <a name="fix-0x8004de40-error-in-onedrive"></a>Memperbaiki kesalahan 0x8004de40 di OneDrive

Jika Anda menerima kesalahan 0x8004de40 dengan OneDrive:

- Reboot komputer yang terpengaruh saat tersambung ke domain direktori Acitve Anda.
- Jika reboot tidak memperbaiki masalah, berhenti bergabung dan bergabung kembali dengan perangkat Anda dari Azure AD. 

**Catatan**: Anda harus berada di jaringan perusahaan Anda saat melakukan langkah-langkah ini. Jangan melakukan langkah-langkah ini saat Anda tidak bisa menyambungkan ke infrastruktur perusahaan Anda (misalnya, saat bepergian). 

- Buka wantian perintah yang ditinggikan. 
- Untuk membuka wantian perintah yang ditinggikan, klik- **mulai**, klik kanan **prompt perintah**, lalu klik **Jalankan sebagai administrator**.
- Ketik *dsregcmd/Leave* dan tekan **Enter**.
- Bila sudah selesai, ketikkan *dsregcmd/Join* dan tekan **Enter**.
- Setelah selesai, tutup wantian perintah.
- Hidupkan ulang komputer, dan masuk ke OneDrive.