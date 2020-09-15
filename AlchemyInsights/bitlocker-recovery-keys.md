---
title: Kunci pemulihan BitLocker
ms.author: pebaum
author: pebaum
manager: mnirkhe
ms.audience: Admin
ms.topic: article
ms.service: o365-administration
ROBOTS: NOINDEX, NOFOLLOW
localization_priority: Normal
ms.collection: Adm_O365
ms.custom:
- "1922"
- "9000220"
ms.openlocfilehash: 7c56e68cf303939d8e7d4ee0a7301e367ecfe9f9
ms.sourcegitcommit: c6692ce0fa1358ec3529e59ca0ecdfdea4cdc759
ms.translationtype: MT
ms.contentlocale: id-ID
ms.lasthandoff: 09/14/2020
ms.locfileid: "47685889"
---
# <a name="accessing-bitlocker-recovery-keys"></a>Mengakses tombol pemulihan BitLocker

Saat mengonfigurasi pengaturan BitLocker kebijakan proteksi titik akhir, dimungkinkan untuk menentukan apakah informasi pemulihan BitLocker akan disimpan dalam direktori aktif Azure.

Jika pengaturan tersebut dikonfigurasi, data pemulihan yang disimpan harus terlihat oleh admin Intune sebagai bagian dari data catatan perangkat di Intune Device Blade dengan dua cara:

Perangkat-perangkat Azure AD-> "perangkat" atau perangkat-> semua perangkat-> "perangkat"-> tombol pemulihan

Alternatifnya, jika ada akses administratif ke perangkat itu sendiri, kunci pemulihan (kata sandi) dapat dilihat dengan menjalankan perintah berikut ini dari wantian perintah yang ditinggikan:

```
manage-bde -protectors c: -get
Example
Volume C: []
All Key Protectors
    TPM:
      ID: {8A5D13D6-7ED9-46C8-A74F-AC3ADF016EC8}
      PCR Validation Profile:
        0, 2, 4, 8, 9, 10, 11
    Numerical Password:
      ID: {DFA26333-XXXX-402C-YYYY-A8C40AF3ZZZZ}
      Password:
        393943-22222-281721-555554-577984-77777-194700-99999
```
Jika perangkat telah dienkripsi sebelum pendaftaran di Intune, kunci pemulihan mungkin telah terkait dengan "akun Microsoft" (MSA) yang digunakan untuk masuk ke perangkat selama proses OOBE. Jika demikian, mengakses  https://onedrive.live.com/recoverykey dan masuk dengan bahwa MSA harus memperlihatkan perangkat yang disimpan.
 
Jika perangkat telah dienkripsi sebagai hasil dari konfigurasi melalui kebijakan grup domain, informasi pemulihan mungkin disimpan di direktori aktif di tempat.
 

