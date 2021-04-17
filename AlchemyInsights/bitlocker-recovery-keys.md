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
ms.openlocfilehash: ec90e412302c74748e253f2e5430fa4205466f0d
ms.sourcegitcommit: 8bc60ec34bc1e40685e3976576e04a2623f63a7c
ms.translationtype: MT
ms.contentlocale: id-ID
ms.lasthandoff: 04/15/2021
ms.locfileid: "51820289"
---
# <a name="accessing-bitlocker-recovery-keys"></a><span data-ttu-id="24a87-102">Mengakses kunci pemulihan Bitlocker</span><span class="sxs-lookup"><span data-stu-id="24a87-102">Accessing Bitlocker recovery keys</span></span>

<span data-ttu-id="24a87-103">Saat mengonfigurasi pengaturan Bitlocker DalamTune Endpoint Protection Policy, Anda dapat menentukan apakah informasi pemulihan Bitlocker harus disimpan di Azure Active Directory.</span><span class="sxs-lookup"><span data-stu-id="24a87-103">When configuring Bitlocker settings Intune Endpoint Protection Policy, it is possible to define whether Bitlocker recovery information should be stored in Azure Active Directory.</span></span>

<span data-ttu-id="24a87-104">Jika pengaturan tersebut dikonfigurasi, data pemulihan yang disimpan akan terlihat oleh admin Intune sebagai bagian dari data rekaman perangkat di blade Perangkat Intune dalam dua cara:</span><span class="sxs-lookup"><span data-stu-id="24a87-104">If that setting is configured, the stored recovery data should be visible to an Intune admin as part of the device record data in Intune Devices blade in two ways:</span></span>

<span data-ttu-id="24a87-105">Perangkat - Perangkat Azure AD -> "Perangkat" OR Perangkat -> Semua Perangkat -> "Perangkat" -> Tombol Pemulihan</span><span class="sxs-lookup"><span data-stu-id="24a87-105">Devices - Azure AD devices -> "Device"  OR Devices -> All Devices -> "Device" -> Recovery keys</span></span>

<span data-ttu-id="24a87-106">Sebagai alternatif, jika terdapat akses administratif ke perangkat itu sendiri, kunci pemulihan (Kata Sandi) dapat dilihat dengan menjalankan perintah berikut dari prompt perintah yang ditinggikan:</span><span class="sxs-lookup"><span data-stu-id="24a87-106">Alternatively, if there is administrative access to the device itself, the recovery key (Password) can be seen by running the following command from an elevated command prompt:</span></span>

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
<span data-ttu-id="24a87-107">Jika perangkat dienkripsi sebelum masuk ke Intune, kunci pemulihan mungkin telah dikaitkan dengan "Akun Microsoft" (MSA) yang digunakan untuk masuk ke perangkat selama proses OOBE.</span><span class="sxs-lookup"><span data-stu-id="24a87-107">If the device was encrypted prior to enrolment in Intune, the recovery key may have been associated with the "Microsoft Account" (MSA) used to sign in to the device during the OOBE process.</span></span> <span data-ttu-id="24a87-108">Jika itu kasusnya, mengakses  https://onedrive.live.com/recoverykey dan masuk dengan MSA tersebut akan memperlihatkan perangkat yang menyimpan kunci pemulihannya.</span><span class="sxs-lookup"><span data-stu-id="24a87-108">If that was the case, accessing  https://onedrive.live.com/recoverykey and signing in with that MSA should show the devices for which recovery keys were stored.</span></span>
 
<span data-ttu-id="24a87-109">Jika perangkat dienkripsi sebagai akibat dari konfigurasi melalui kebijakan grup berbasis domain, informasi pemulihan dapat disimpan di Direktori Aktif di tempat.</span><span class="sxs-lookup"><span data-stu-id="24a87-109">If the device was encrypted as a result of configuration through domain-based group policy, the recovery information may be stored in the on-premise Active Directory.</span></span>

<span data-ttu-id="24a87-110">Jika telah mengonfigurasi Kebijakan proteksi titik akhir untuk menyimpan kunci pemulihan di Azure Active Directory, tetapi kunci untuk perangkat tertentu belum diunggah, Anda dapat memicu unggahan dengan memutar kunci pemulihan untuk perangkat tersebut dari konsol MEM.</span><span class="sxs-lookup"><span data-stu-id="24a87-110">If you have configured Endpoint protection policy to store the recovery key in Azure Active Directory but the key for a specific device has not been uploaded, you can trigger the upload by rotating the recovery key for that device from the MEM console.</span></span> <span data-ttu-id="24a87-111">Untuk detailnya, [lihat Memutar kunci pemulihan BitLocker.](https://docs.microsoft.com/mem/intune/protect/encrypt-devices#view-details-for-recovery-keys)</span><span class="sxs-lookup"><span data-stu-id="24a87-111">For details, see [Rotate BitLocker recovery keys](https://docs.microsoft.com/mem/intune/protect/encrypt-devices#view-details-for-recovery-keys).</span></span>

