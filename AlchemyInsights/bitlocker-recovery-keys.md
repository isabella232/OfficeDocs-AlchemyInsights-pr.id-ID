---
title: Kunci pemulihan BitLocker
ms.author: pebaum
author: pebaum
manager: mnirkhe
ms.audience: Admin
ms.topic: article
ROBOTS: NOINDEX, NOFOLLOW
localization_priority: Normal
ms.collection: Adm_O365
ms.custom:
- "1922"
- "9000220"
ms.openlocfilehash: 4e06e0e43b63836b9e9cf923e554dd474b82c671
ms.sourcegitcommit: 123e9fe46e99719dd271e75a66555861e968f4a2
ms.translationtype: MT
ms.contentlocale: id-ID
ms.lasthandoff: 12/30/2019
ms.locfileid: "40908818"
---
# <a name="accessing-bitlocker-recovery-keys"></a>Mengakses kunci pemulihan BitLocker

Saat mengonfigurasi pengaturan BitLocker kebijakan perlindungan akhir Intune, dimungkinkan untuk menentukan apakah informasi pemulihan BitLocker harus disimpan di Azure Active Directory.

Jika pengaturan yang dikonfigurasi, data pemulihan disimpan harus terlihat admin Intune sebagai bagian dari perangkat data catatan di Intune perangkat pisau dalam dua cara:

Perangkat-perangkat Azure AD-> "perangkat" atau perangkat-> semua perangkat-> "perangkat"-> tombol pemulihan

Selain itu, jika ada akses administratif ke perangkat itu sendiri, kunci pemulihan (sandi) dapat dilihat dengan menjalankan perintah berikut ini dari wantian perintah yang ditampilkan:

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
Jika perangkat dienkripsi sebelum pendaftaran di Intune, kunci pemulihan mungkin telah dikaitkan dengan "akun Microsoft" (MSA) yang digunakan untuk masuk ke perangkat selama proses OOBE. Jika itu masalahnya, mengakses https://onedrive.live.com/recoverykey dan masuk dengan MSA tersebut harus menampilkan perangkat yang menyimpan kunci pemulihan.
 
Jika perangkat dienkripsi sebagai akibat dari konfigurasi melalui kebijakan grup berbasis domain, informasi pemulihan dapat disimpan di direktori aktif di tempat.
 

