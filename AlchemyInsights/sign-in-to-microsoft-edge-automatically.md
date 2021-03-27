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
- "8333"
- "9004625"
ms.openlocfilehash: 6021991c125f5cb2a33ce8db8fe7717b528bf49b
ms.sourcegitcommit: 6bfe9cd9d0b18481e0cac6f1f5bc86ed7df31037
ms.translationtype: MT
ms.contentlocale: id-ID
ms.lasthandoff: 03/27/2021
ms.locfileid: "51398732"
---
# <a name="sign-in-to-microsoft-edge-automatically"></a>Masuk ke Microsoft Edge secara otomatis

Microsoft Edge menggunakan akun default OS untuk secara otomatis masuk ke pengguna sesuai dengan bagaimana perangkat pengguna dikonfigurasi. 

Skenario setiap tipe konfigurasi perangkat dan proses masuk pengguna dependennya dijelaskan di bawah ini:

- **Perangkat adalah hibrid/AAD-J**: Opsi ini tersedia di Windows 10, Windows tingkat bawah, dan versi server yang terkait. Pengguna secara otomatis masuk dengan akun Azure Active Directory (AD) mereka.
- **Perangkat tergabung dalam domain:** Opsi ini tersedia di Windows 10, Windows tingkat bawah, dan versi server yang terkait. Secara default, pengguna dengan akun domain tidak masuk secara otomatis; untuk mengaktifkan masuk otomatis bagi mereka, gunakan kebijakan **ConfigureOnPremisesAccountAutoSignIn.** Untuk mengaktifkan masuk otomatis bagi pengguna dengan akun Azure AD, pertimbangkan untuk menggabungkan perangkat mereka dengan hibrid.
- Akun default OS adalah akun **Microsoft:** Opsi ini tersedia di Windows 10 RS3 (versi 1709, build 10.0.16299) dan versi yang lebih baru. Skenario tidak seperti terjadi pada perangkat perusahaan. Namun, jika akun default OS adalah akun Microsoft, maka Microsoft Edge akan secara otomatis masuk ke pengguna tersebut dengan akun Microsoft.
 
 
