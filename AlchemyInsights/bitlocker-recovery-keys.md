---
title: Kunci pemulihan Bitlocker
ms.author: pebaum
author: pebaum
manager: scotv
ms.audience: Admin
ms.topic: article
ms.service: o365-administration
ROBOTS: NOINDEX, NOFOLLOW
localization_priority: Normal
ms.collection: Adm_O365
ms.custom:
- "1922"
- "9000220"
ms.openlocfilehash: f71fae0aabda3fc48f20d5ea1e6909475f0c17ff5cdf98b58b1403bd2e291c19
ms.sourcegitcommit: b5f7da89a650d2915dc652449623c78be6247175
ms.translationtype: MT
ms.contentlocale: id-ID
ms.lasthandoff: 08/05/2021
ms.locfileid: "54060067"
---
# <a name="accessing-bitlocker-recovery-keys"></a>Mengakses kunci pemulihan Bitlocker

Saat mengonfigurasi pengaturan Bitlocker DalamTune Endpoint Protection Policy, Anda dapat menentukan apakah informasi pemulihan Bitlocker harus disimpan di Azure Active Directory.

Jika pengaturan tersebut dikonfigurasi, data pemulihan yang disimpan akan terlihat oleh admin Intune sebagai bagian dari data rekaman perangkat di blade Perangkat Intune dalam dua cara:

Perangkat - Perangkat Azure AD -> "Perangkat" OR Perangkat -> Semua Perangkat -> "Perangkat" -> Tombol Pemulihan

Sebagai alternatif, jika terdapat akses administratif ke perangkat itu sendiri, kunci pemulihan (Kata Sandi) dapat dilihat dengan menjalankan perintah berikut dari prompt perintah yang ditinggikan:

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
Jika perangkat dienkripsi sebelum masuk ke Intune, kunci pemulihan mungkin telah dikaitkan dengan "Akun Microsoft" (MSA) yang digunakan untuk masuk ke perangkat selama proses OOBE. Jika itu kasusnya, mengakses  https://onedrive.live.com/recoverykey dan masuk dengan MSA tersebut akan memperlihatkan perangkat yang menyimpan kunci pemulihannya.
 
Jika perangkat dienkripsi sebagai akibat dari konfigurasi melalui kebijakan grup berbasis domain, informasi pemulihan dapat disimpan di Direktori Aktif di tempat.

Jika telah mengonfigurasi Kebijakan proteksi titik akhir untuk menyimpan kunci pemulihan di Azure Active Directory tetapi kunci untuk perangkat tertentu belum diunggah, Anda dapat memicu unggahan dengan memutar kunci pemulihan untuk perangkat tersebut dari konsol MEM. Untuk detailnya, [lihat Memutar kunci pemulihan BitLocker.](https://docs.microsoft.com/mem/intune/protect/encrypt-devices#view-details-for-recovery-keys)

