---
title: Masuk ke Microsoft Edge secara otomatis
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
ms.openlocfilehash: 68a1119abd0a3f687b6448bb6e58c6485c239c0f
ms.sourcegitcommit: 94036315916fbc79dca2a692c2e9bc1139dd28f6
ms.translationtype: MT
ms.contentlocale: id-ID
ms.lasthandoff: 12/08/2020
ms.locfileid: "49677766"
---
# <a name="sign-in-to-microsoft-edge-automatically"></a>Masuk ke Microsoft Edge secara otomatis

Microsoft Edge menggunakan akun default OS untuk secara otomatis memasukkan pengguna sesuai dengan cara perangkat pengguna dikonfigurasi. 

Skenario setiap tipe konfigurasi perangkat dan proses masuk pengguna dependen diuraikan di bawah ini:

1. **Perangkat ini hibrid/AAD-J**: opsi ini tersedia di Windows 10, Windows tingkat bawah, dan versi server terkait. Pengguna secara otomatis masuk dengan akun Azure Active Directory (AD) mereka.
2. **Perangkat ini tergabung dalam domain**: opsi ini tersedia di Windows 10, Windows tingkat bawah, dan versi server terkait. Secara default, pengguna dengan akun domain tidak masuk secara otomatis; untuk mengaktifkan masuk otomatis bagi mereka, gunakan kebijakan **Configureonpremisesaccountautosignin** . Untuk mengaktifkan masuk otomatis bagi pengguna dengan akun Azure AD, pertimbangkan hibrid-bergabung dengan perangkat mereka.
3. **Akun default OS adalah akun Microsoft**: opsi ini tersedia di Windows 10 RS3 (versi 1709, Build 10.0.16299) dan versi yang lebih baru. Skenario tidak mungkin terjadi pada perangkat perusahaan. Namun, jika akun default OS adalah akun Microsoft, maka Microsoft Edge akan secara otomatis masuk ke pengguna dengan akun Microsoft.
 
 
