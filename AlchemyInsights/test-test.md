---
title: Persyaratan yang hilang dari SharePoint online Term Store
ms.author: pebaum
author: Techwriter40
ms.date: 10/30/2018
ms.audience: ITPro
ms.topic: article
ROBOTS: NOINDEX, NOFOLLOW
localization_priority: Normal
ms.custom:
- "1243"
- "5200021"
ms.openlocfilehash: 0f9efe980987c9ffc64fcf9d5d72a67f0a622867
ms.sourcegitcommit: 23772ebd25a86a879ced40b10566a35e76a79eb5
ms.translationtype: MT
ms.contentlocale: id-ID
ms.lasthandoff: 09/05/2019
ms.locfileid: "36762067"
---
# <a name="enabling-bitlocker-encryption-with-intune"></a><span data-ttu-id="94440-102">Mengaktifkan enkripsi BitLocker dengan Intune</span><span class="sxs-lookup"><span data-stu-id="94440-102">Enabling Bitlocker Encryption with Intune</span></span>

<span data-ttu-id="94440-103">Intune Endpoint Protection Policy dapat digunakan untuk mengonfigurasi pengaturan enkripsi Boitlocker untuk perangkat Windows seperti yang dijelaskan dalam pengaturan: Windows10 (dan yang lebih baru) untuk melindungi perangkat menggunakan Intune</span><span class="sxs-lookup"><span data-stu-id="94440-103">Intune Endpoint Protection Policy can be used to configure Boitlocker encryption settings for Windows devices as described in : Windows10 (and later) settings to protect devices using Intune</span></span>

<span data-ttu-id="94440-104">Anda harus menyadari bahwa banyak perangkat yang lebih baru yang menjalankan Windows 10 dukungan otomatis BitLocker enkripsi yang dipicu tanpa penerapan kebijakan MDM.</span><span class="sxs-lookup"><span data-stu-id="94440-104">You should be aware that many newer devices running Windows 10 support automatic bitlocker encryption which is triggered without the application of MDM policy.</span></span> <span data-ttu-id="94440-105">Hal ini dapat mempengaruhi penerapan kebijakan jika pengaturan non default dikonfigurasi.</span><span class="sxs-lookup"><span data-stu-id="94440-105">This may impact application of policy if non default settings are configured.</span></span> <span data-ttu-id="94440-106">Lihat FAQ untuk lebih jelasnya.</span><span class="sxs-lookup"><span data-stu-id="94440-106">See FAQ for more detail.</span></span>


<span data-ttu-id="94440-107">FAQ  Q: yang edisi Windows dukungan perangkat enkripsi menggunakan kebijakan perlindungan Endpoint?</span><span class="sxs-lookup"><span data-stu-id="94440-107">FAQ  Q: Which editions of Windows support device encryption using the Endpoint Protection Policy?</span></span>
<span data-ttu-id="94440-108"> A: tataan di Intune Endpoint Protection kebijakan diterapkan menggunakan BitLocker CSP.</span><span class="sxs-lookup"><span data-stu-id="94440-108"> A: The settings in Intune Endpoint Protection Policy  are implemented using the Bitlocker CSP.</span></span><span data-ttu-id="94440-109">Tidak semua edisi atau Build Windows mendukung BitLocker CSP. 
     </span><span class="sxs-lookup"><span data-stu-id="94440-109">  Not all editions nor builds of Windows support the Bitlocker CSP. 
     </span></span> <span data-ttu-id="94440-110">Pada saat ini edisi Windows: Enterprise; Pendidikan, Mobile, Mobile Enterprise dan profesional (dari membangun 1809 dan seterusnya) yang didukung.</span><span class="sxs-lookup"><span data-stu-id="94440-110">At this time Windows Editions: Enterprise; Education, Mobile, Mobile Enterprise and Professional (from build 1809 onwards) are supported.</span></span>




<span data-ttu-id="94440-111">Q: jika perangkat sudah dienkripsi dengan BitLocker menggunakan pengaturan default OS untuk metode enkripsi dan kekuatan cipher (XTS-AES-128) akan menerapkan kebijakan dengan pengaturan yang berbeda secara otomatis memicu Re-enkripsi drive dengan pengaturan baru?</span><span class="sxs-lookup"><span data-stu-id="94440-111">Q: If a device is already encrypted with Bitlocker using the OS default settings for encryption method and cipher strength (XTS-AES-128)  will applying a policy with different settings automatically trigger re-encryption of the drive with the new settings?</span></span>

<span data-ttu-id="94440-112">A: tidak.</span><span class="sxs-lookup"><span data-stu-id="94440-112">A: No.</span></span> <span data-ttu-id="94440-113">Untuk menerapkan pengaturan penyandian baru, kandar harus didekripsi terlebih dahulu.</span><span class="sxs-lookup"><span data-stu-id="94440-113">In order to apply the new cipher settings the drive must first be decrypted.</span></span>

<span data-ttu-id="94440-114">Catatan untuk perangkat yang terdaftar dengan autopilot enkripsi otomatis yang akan terjadi selama OOBE tidak dipicu hingga Intune kebijakan dievaluasi yang memungkinkan pengaturan berbasis kebijakan untuk digunakan di tempat default OS</span><span class="sxs-lookup"><span data-stu-id="94440-114">Note For devices being enrolled with Autopilot the automatic encryption that would occur during OOBE is not triggered until Intune policy is evaluated which allows the policy based settings to be used in place of the OS defaults</span></span>




<span data-ttu-id="94440-115">Q jika perangkat dienkripsi sebagai akibat dari penerapan kebijakan Intune akan didekripsi ketika kebijakan yang dihapus?</span><span class="sxs-lookup"><span data-stu-id="94440-115">Q If a device is encrypted as a result of the  application of Intune policy will it be decrypted when that policy is removed?</span></span>

<span data-ttu-id="94440-116">A: penghapusan Kebijakan enkripsi terkait tidak mengakibatkan dekripsi kandar yang dikonfigurasi.</span><span class="sxs-lookup"><span data-stu-id="94440-116">A: Removal of encryption related policy does NOT result in decryption of the drives which were configured.</span></span>




<span data-ttu-id="94440-117">T: Mengapa Intune kebijakan kepatuhan menunjukkan bahwa perangkat saya tidak memiliki "BitLocker diaktifkan" tapi itu?</span><span class="sxs-lookup"><span data-stu-id="94440-117">Q: Why does intune Compliance policy show that my device does not have "Bitlocker Enabled" but it is?</span></span>

<span data-ttu-id="94440-118">A: "BitLocker diaktifkan" pengaturan di Intune kepatuhan kebijakan menggunakan klien Windows perangkat kesehatan Attestation (DHA).</span><span class="sxs-lookup"><span data-stu-id="94440-118">A: The "Bitlocker enabled" setting in intune compliance policy utilizes the Windows Device Health Attestation  (DHA) client.</span></span> <span data-ttu-id="94440-119">Klien ini hanya mengukur status perangkat pada saat boot.</span><span class="sxs-lookup"><span data-stu-id="94440-119">This client only measures device state at boot time.</span></span> <span data-ttu-id="94440-120">Jadi, jika perangkat belum reboot sejak enkripsi BitLocker selesai layanan klien DHA tidak akan melaporkan BitLocker sebagai aktif.</span><span class="sxs-lookup"><span data-stu-id="94440-120">So if a device has not been rebooted since bitlocker encryption was completed the DHA client service will not report bitlocker as being active.</span></span>