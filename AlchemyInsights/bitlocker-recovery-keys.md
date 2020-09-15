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
# <a name="accessing-bitlocker-recovery-keys"></a><span data-ttu-id="198db-102">Mengakses tombol pemulihan BitLocker</span><span class="sxs-lookup"><span data-stu-id="198db-102">Accessing Bitlocker recovery keys</span></span>

<span data-ttu-id="198db-103">Saat mengonfigurasi pengaturan BitLocker kebijakan proteksi titik akhir, dimungkinkan untuk menentukan apakah informasi pemulihan BitLocker akan disimpan dalam direktori aktif Azure.</span><span class="sxs-lookup"><span data-stu-id="198db-103">When configuring Bitlocker settings Intune Endpoint Protection Policy, it is possible to define whether Bitlocker recovery information should be stored in Azure Active Directory.</span></span>

<span data-ttu-id="198db-104">Jika pengaturan tersebut dikonfigurasi, data pemulihan yang disimpan harus terlihat oleh admin Intune sebagai bagian dari data catatan perangkat di Intune Device Blade dengan dua cara:</span><span class="sxs-lookup"><span data-stu-id="198db-104">If that setting is configured, the stored recovery data should be visible to an Intune admin as part of the device record data in Intune Devices blade in two ways:</span></span>

<span data-ttu-id="198db-105">Perangkat-perangkat Azure AD-> "perangkat" atau perangkat-> semua perangkat-> "perangkat"-> tombol pemulihan</span><span class="sxs-lookup"><span data-stu-id="198db-105">Devices - Azure AD devices -> "Device"  OR Devices -> All Devices -> "Device" -> Recovery keys</span></span>

<span data-ttu-id="198db-106">Alternatifnya, jika ada akses administratif ke perangkat itu sendiri, kunci pemulihan (kata sandi) dapat dilihat dengan menjalankan perintah berikut ini dari wantian perintah yang ditinggikan:</span><span class="sxs-lookup"><span data-stu-id="198db-106">Alternatively, if there is administrative access to the device itself, the recovery key (Password) can be seen by running the following command from an elevated command prompt:</span></span>

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
<span data-ttu-id="198db-107">Jika perangkat telah dienkripsi sebelum pendaftaran di Intune, kunci pemulihan mungkin telah terkait dengan "akun Microsoft" (MSA) yang digunakan untuk masuk ke perangkat selama proses OOBE.</span><span class="sxs-lookup"><span data-stu-id="198db-107">If the device was encrypted prior to enrolment in Intune, the recovery key may have been associated with the "Microsoft Account" (MSA) used to sign in to the device during the OOBE process.</span></span> <span data-ttu-id="198db-108">Jika demikian, mengakses  https://onedrive.live.com/recoverykey dan masuk dengan bahwa MSA harus memperlihatkan perangkat yang disimpan.</span><span class="sxs-lookup"><span data-stu-id="198db-108">If that was the case, accessing  https://onedrive.live.com/recoverykey and signing in with that MSA should show the devices for which recovery keys were stored.</span></span>
 
<span data-ttu-id="198db-109">Jika perangkat telah dienkripsi sebagai hasil dari konfigurasi melalui kebijakan grup domain, informasi pemulihan mungkin disimpan di direktori aktif di tempat.</span><span class="sxs-lookup"><span data-stu-id="198db-109">If the device was encrypted as a result of configuration through domain-based group policy, the recovery information may be stored in the on-premise Active Directory.</span></span>
 

