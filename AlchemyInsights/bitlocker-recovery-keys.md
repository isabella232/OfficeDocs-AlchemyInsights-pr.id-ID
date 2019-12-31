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
# <a name="accessing-bitlocker-recovery-keys"></a><span data-ttu-id="86365-102">Mengakses kunci pemulihan BitLocker</span><span class="sxs-lookup"><span data-stu-id="86365-102">Accessing Bitlocker recovery keys</span></span>

<span data-ttu-id="86365-103">Saat mengonfigurasi pengaturan BitLocker kebijakan perlindungan akhir Intune, dimungkinkan untuk menentukan apakah informasi pemulihan BitLocker harus disimpan di Azure Active Directory.</span><span class="sxs-lookup"><span data-stu-id="86365-103">When configuring Bitlocker settings Intune Endpoint Protection Policy, it is possible to define whether Bitlocker recovery information should be stored in Azure Active Directory.</span></span>

<span data-ttu-id="86365-104">Jika pengaturan yang dikonfigurasi, data pemulihan disimpan harus terlihat admin Intune sebagai bagian dari perangkat data catatan di Intune perangkat pisau dalam dua cara:</span><span class="sxs-lookup"><span data-stu-id="86365-104">If that setting is configured, the stored recovery data should be visible to an Intune admin as part of the device record data in Intune Devices blade in two ways:</span></span>

<span data-ttu-id="86365-105">Perangkat-perangkat Azure AD-> "perangkat" atau perangkat-> semua perangkat-> "perangkat"-> tombol pemulihan</span><span class="sxs-lookup"><span data-stu-id="86365-105">Devices - Azure AD devices -> "Device"  OR Devices -> All Devices -> "Device" -> Recovery keys</span></span>

<span data-ttu-id="86365-106">Selain itu, jika ada akses administratif ke perangkat itu sendiri, kunci pemulihan (sandi) dapat dilihat dengan menjalankan perintah berikut ini dari wantian perintah yang ditampilkan:</span><span class="sxs-lookup"><span data-stu-id="86365-106">Alternatively, if there is administrative access to the device itself, the recovery key (Password) can be seen by running the following command from an elevated command prompt:</span></span>

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
<span data-ttu-id="86365-107">Jika perangkat dienkripsi sebelum pendaftaran di Intune, kunci pemulihan mungkin telah dikaitkan dengan "akun Microsoft" (MSA) yang digunakan untuk masuk ke perangkat selama proses OOBE.</span><span class="sxs-lookup"><span data-stu-id="86365-107">If the device was encrypted prior to enrolment in Intune, the recovery key may have been associated with the "Microsoft Account" (MSA) used to sign in to the device during the OOBE process.</span></span> <span data-ttu-id="86365-108">Jika itu masalahnya, mengakses https://onedrive.live.com/recoverykey dan masuk dengan MSA tersebut harus menampilkan perangkat yang menyimpan kunci pemulihan.</span><span class="sxs-lookup"><span data-stu-id="86365-108">If that was the case, accessing  https://onedrive.live.com/recoverykey and signing in with that MSA should show the devices for which recovery keys were stored.</span></span>
 
<span data-ttu-id="86365-109">Jika perangkat dienkripsi sebagai akibat dari konfigurasi melalui kebijakan grup berbasis domain, informasi pemulihan dapat disimpan di direktori aktif di tempat.</span><span class="sxs-lookup"><span data-stu-id="86365-109">If the device was encrypted as a result of configuration through domain-based group policy, the recovery information may be stored in the on-premise Active Directory.</span></span>
 

