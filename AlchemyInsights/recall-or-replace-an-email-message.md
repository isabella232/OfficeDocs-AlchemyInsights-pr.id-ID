---
title: Ingat atau mengganti pesan email
ms.author: daeite
author: daeite
manager: joallard
ms.date: 05/15/2019
ms.audience: Admin
ms.topic: article
ROBOTS: NOINDEX, NOFOLLOW
localization_priority: Normal
ms.collection: Adm_O365
ms.custom:
- "1860"
- "9000260"
ms.assetid: ''
ms.openlocfilehash: d5952041f6f2fd736e975abf06cc22880d21a089
ms.sourcegitcommit: 1d98db8acb9959aba3b5e308a567ade6b62da56c
ms.translationtype: MT
ms.contentlocale: id-ID
ms.lasthandoff: 08/22/2019
ms.locfileid: "36553435"
---
# <a name="recall-or-replace-an-email-message-in-office-365"></a>Ingat atau mengganti pesan email di Office 365

- Anda dapat **hanya ingat pesan yang dikirim ke pengguna di organisasi Anda**. Jika pesan dikirim ke alamat Gmail, misalnya, Anda tidak bisa mengingat itu.
- Anda dapat **hanya ingat pesan yang dikirim dari 2016 Outlook untuk PC**. Jika pengguna mengirim pesan menggunakan Outlook untuk Mac atau Outlook di web, Anda tidak bisa mengingat itu.
- Jika Anda seorang admin, Anda dapat **mengingat pesan atas nama pengguna dengan menggunakan PowerShell**. Anda tidak bisa mengingat pesan dari di admin center. Gulir ke bawah untuk "Mencari dan menghapus pesan email di organisasi Anda" untuk informasi lebih lanjut.

**Ingat atau mengganti pesan email yang dikirim**

1. Di panel map di sebelah kiri jendela Outlook, pilih folder Item Terkirim.
2. Buka pesan yang ingin Anda ingat. Anda harus mengklik ganda untuk membuka pesan. Memilih pesan sehingga muncul di panel baca tidak akan mengizinkan Anda untuk mengingat pesan.
3. Dari tab Pesan, pilih **tindakan** > **Ingat pesan ini**.
4. Memilih **menghapus belum dibaca salinan pesan ini** atau **menghapus salinan yang belum dibaca dan menggantinya dengan pesan baru**, lalu pilih **OK**.
5. Jika Anda mengirim pesan penggantian, menulis pesan, lalu pilih **kirim**.
6. Keberhasilan atau kegagalan mengingat pesan tergantung pada pengaturan penerima di Outlook.

Untuk informasi lebih lanjut, termasuk bagaimana untuk memeriksa ingat, lihat [ingat atau mengganti pesan email yang dikirim](https://support.office.com/article/35027f88-d655-4554-b4f8-6c0729a723a0).

***Mencari dan menghapus pesan email di organisasi Anda*** Untuk mencari dan menghapus pesan email di organisasi Anda, sangat mudah jika Anda global admin. Jika Anda tidak global admin, akun Anda harus ditambahkan ke grup peran Manajer eDiscovery, atau untuk peran manajemen pencarian kepatuhan. Untuk menghapus pesan, Anda akan perlu untuk bergabung dengan grup peran manajemen organisasi atau peran manajemen pencarian dan pembersihan. Izin untuk peran ini ditetapkan di [Pusat Keamanan & kepatuhan](https://protection.office.com/).

1. [Buat konten pencarian](https://docs.microsoft.com/office365/securitycompliance/content-search) untuk menemukan pesan untuk menghapus.
2. [Terhubung ke keamanan & Compliance Center PowerShell](https://docs.microsoft.com/powershell/exchange/office-365-scc/connect-to-scc-powershell/connect-to-scc-powershell?view=exchange-ps). 

Jika Anda menggunakan MFA, lihat [tersambung ke kantor 365 keamanan & kepatuhan pusat PowerShell menggunakan multi faktor otentikasi](https://docs.microsoft.com/powershell/exchange/office-365-scc/connect-to-scc-powershell/mfa-connect-to-scc-powershell?view=exchange-ps). 
