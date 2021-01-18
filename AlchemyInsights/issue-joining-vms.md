---
title: Masalah penggabungan VM
ms.author: v-smandalika
author: v-smandalika
manager: dansimp
ms.date: 01/15/2021
ms.audience: Admin
ms.topic: article
ms.service: o365-administration
ROBOTS: NOINDEX, NOFOLLOW
localization_priority: Priority
ms.collection: Adm_O365
ms.custom:
- "7924"
- "9004395"
ms.openlocfilehash: 77a889f05d6c4e7b19a1e0a66a99ffc0565c69d8
ms.sourcegitcommit: a61a29dbd0382370fea0be5fa4a61c9a1a9354c7
ms.translationtype: MT
ms.contentlocale: id-ID
ms.lasthandoff: 01/18/2021
ms.locfileid: "49885208"
---
# <a name="issue-joining-vms"></a>Masalah penggabungan VM

Untuk mengatasi masalah yang terjadi saat mencoba bergabung dengan VM, lakukan langkah-langkah berikut:

1. Cobalah untuk masuk menggunakan format **UPN** (misalnya, ' joeuser@contoso.com ') dan bukan nama **SAMAccountName** (' CONTOSO\joeuser ').
2. Pastikan bahwa Anda telah mengaktifkan sinkronisasi kata sandi sesuai dengan langkah-langkah yang diuraikan dalam panduan *memulai* .
3. Pastikan bahwa akun pengguna yang terpengaruh bukan akun eksternal dalam penyewa Azure AD. Pengguna eksternal tidak bisa masuk ke domain terkelola karena layanan domain Azure AD tidak memiliki kredensial untuk akun pengguna tersebut.
4. Jika akun pengguna yang terpengaruh adalah akun pengguna berbasis awan saja, pastikan bahwa pengguna telah mengubah kata sandinya setelah Anda mengaktifkan layanan domain Azure AD. Langkah ini menyebabkan hash kredensial yang diperlukan untuk layanan domain Azure AD yang akan dihasilkan.
5. Jika akun pengguna yang terpengaruh disinkronisasi dari direktori lokal, verifikasi bahwa rilis Azure AD Connect yang direkomendasikan telah dikonfigurasikan untuk melakukan sinkronisasi penuh.
6. Jika masalah tetap ada setelah mengonfirmasi langkah 4, jalankan perintah berikut ini dari mesin sinkronisasi Anda:
 
     `"net stop 'Microsoft Azure AD Sync'"`  
     `"net start 'Microsoft Azure AD Sync'"`.