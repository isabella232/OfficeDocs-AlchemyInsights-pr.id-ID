---
title: Masuk untuk Microsoft Edge secara otomatis
ms.author: v-smandalika
author: v-smandalika
manager: dansimp
ms.date: 12/03/2020
ms.audience: Admin
ms.topic: article
ms.service: o365-administration
ROBOTS: NOINDEX, NOFOLLOW
localization_priority: Normal
ms.collection: Adm_O365
ms.custom:
- "9003848"
- "6898"
- "8333"
- "9004625"
ms.openlocfilehash: 4e069a1c75caabf3bef7387140edd5650cf966856b888b5c6b5618a603986d6d
ms.sourcegitcommit: b5f7da89a650d2915dc652449623c78be6247175
ms.translationtype: MT
ms.contentlocale: id-ID
ms.lasthandoff: 08/05/2021
ms.locfileid: "54050697"
---
# <a name="sign-in-to-microsoft-edge-automatically"></a>Masuk untuk Microsoft Edge secara otomatis

Microsoft Edge menggunakan akun default OS untuk masuk secara otomatis ke pengguna sesuai dengan bagaimana perangkat pengguna dikonfigurasi. 

Skenario setiap tipe konfigurasi perangkat dan proses masuk pengguna dependennya dijelaskan di bawah ini:

- **Perangkat hibrid/AAD-J:** Opsi ini tersedia pada versi Windows 10, tingkat ke bawah Windows, dan server yang terkait. Pengguna secara otomatis masuk dengan akun Azure Active Directory (AD) mereka.
- **Perangkat tergabung dalam domain:** Opsi ini tersedia di Windows 10, tingkat ke bawah Windows, dan versi server yang terkait. Secara default, pengguna dengan akun domain tidak masuk secara otomatis; untuk mengaktifkan masuk otomatis bagi mereka, gunakan kebijakan **ConfigureOnPremisesAccountAutoSignIn.** Untuk mengaktifkan masuk otomatis bagi pengguna dengan akun Azure AD, pertimbangkan untuk menggabungkan perangkat mereka dengan hibrid.
- Akun default OS adalah akun **Microsoft:** Opsi ini tersedia di Windows 10 RS3 (versi 1709, build 10.0.16299) dan versi yang lebih baru. Skenario tidak seperti terjadi pada perangkat perusahaan. Namun, jika akun default OS adalah akun Microsoft, Microsoft Edge akan masuk secara otomatis ke pengguna dengan akun Microsoft.
 
 
