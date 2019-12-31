---
title: DataProtection-BitLocker
ms.author: pebaum
author: pebaum
manager: mnirkhe
ms.audience: Admin
ms.topic: article
ROBOTS: NOINDEX, NOFOLLOW
localization_priority: Normal
ms.collection: Adm_O365
ms.custom:
- "1802"
- "9000220"
ms.openlocfilehash: c23a2a2bde240900119382a9c1185a6e02520149
ms.sourcegitcommit: 123e9fe46e99719dd271e75a66555861e968f4a2
ms.translationtype: MT
ms.contentlocale: id-ID
ms.lasthandoff: 12/30/2019
ms.locfileid: "40908713"
---
# <a name="enabling-bitlocker-encryption-with-intune"></a><span data-ttu-id="ff0ba-102">Mengaktifkan enkripsi BitLocker dengan Intune</span><span class="sxs-lookup"><span data-stu-id="ff0ba-102">Enabling Bitlocker encryption with Intune</span></span>

 <span data-ttu-id="ff0ba-103">Intune Endpoint Protection Policy dapat digunakan untuk mengkonfigurasi pengaturan enkripsi BitLocker untuk perangkat Windows.</span><span class="sxs-lookup"><span data-stu-id="ff0ba-103">Intune Endpoint Protection Policy can be used to configure Bitlocker encryption settings for Windows devices.</span></span> <span data-ttu-id="ff0ba-104">Untuk informasi selengkapnya, lihat [pengaturan Windows 10 (dan yang lebih baru) untuk melindungi perangkat yang menggunakan Intune](https://docs.microsoft.com/intune/endpoint-protection-windows-10#windows-encryption).</span><span class="sxs-lookup"><span data-stu-id="ff0ba-104">For more information, see [Windows 10 (and later) settings to protect devices using Intune](https://docs.microsoft.com/intune/endpoint-protection-windows-10#windows-encryption).</span></span>
 
<span data-ttu-id="ff0ba-105">Anda harus menyadari bahwa banyak perangkat yang lebih baru yang menjalankan Windows 10 dukungan otomatis BitLocker enkripsi, yang dipicu tanpa penerapan kebijakan MDM.</span><span class="sxs-lookup"><span data-stu-id="ff0ba-105">You should be aware that many newer devices running Windows 10 support automatic Bitlocker encryption, which is triggered without the application of MDM policy.</span></span> <span data-ttu-id="ff0ba-106">Hal ini dapat mempengaruhi penerapan kebijakan jika pengaturan non-default dikonfigurasi.</span><span class="sxs-lookup"><span data-stu-id="ff0ba-106">This may impact application of policy if non-default settings are configured.</span></span> <span data-ttu-id="ff0ba-107">Lihat FAQ berikut untuk detail selengkapnya.</span><span class="sxs-lookup"><span data-stu-id="ff0ba-107">See the following FAQ for more detail.</span></span>
 
<span data-ttu-id="ff0ba-108">Untuk informasi tentang pemecahan masalah BitLocker, lihat [memecahkan masalah BitLocker kebijakan di Microsoft Intune](https://docs.microsoft.com/intune/protect/troubleshoot-bitlocker-policies).</span><span class="sxs-lookup"><span data-stu-id="ff0ba-108">For information about troubleshooting bitlocker issues, see [Troubleshoot BitLocker policies in Microsoft Intune](https://docs.microsoft.com/intune/protect/troubleshoot-bitlocker-policies).</span></span>
 
 
<span data-ttu-id="ff0ba-109">**Faq**</span><span class="sxs-lookup"><span data-stu-id="ff0ba-109">**FAQ**</span></span>

 <span data-ttu-id="ff0ba-110">Q: yang edisi Windows dukungan perangkat enkripsi menggunakan kebijakan perlindungan Endpoint?</span><span class="sxs-lookup"><span data-stu-id="ff0ba-110">Q: Which editions of Windows support device encryption using the Endpoint Protection Policy?</span></span><br>
 <span data-ttu-id="ff0ba-111">A: pengaturan pada kebijakan perlindungan akhir Intune diterapkan menggunakan [BITLOCKER CSP](https://docs.microsoft.com/windows/client-management/mdm/bitlocker-csp).</span><span class="sxs-lookup"><span data-stu-id="ff0ba-111">A: The settings in Intune Endpoint Protection Policy  are implemented using the [Bitlocker CSP](https://docs.microsoft.com/windows/client-management/mdm/bitlocker-csp).</span></span> <span data-ttu-id="ff0ba-112">Tidak semua edisi atau versi Windows mendukung BitLocker CSP.</span><span class="sxs-lookup"><span data-stu-id="ff0ba-112">Not all editions or builds of Windows support the Bitlocker CSP.</span></span> <br><br>
      <span data-ttu-id="ff0ba-113">Saat ini, berikut edisi Windows yang didukung: perusahaan, pendidikan, Mobile, Mobile Enterprise, dan profesional (membangun 1809 dan yang lebih baru).</span><span class="sxs-lookup"><span data-stu-id="ff0ba-113">At this time, the following Windows editions are supported: Enterprise, Education, Mobile, Mobile Enterprise, and Professional (build 1809 and later).</span></span>
 
<span data-ttu-id="ff0ba-114">Q: jika perangkat sudah dienkripsi dengan BitLocker menggunakan pengaturan default OS untuk metode enkripsi dan kekuatan cipher (XTS-AES-128), akan menerapkan kebijakan dengan pengaturan yang berbeda secara otomatis memicu Re-enkripsi drive dengan pengaturan baru?</span><span class="sxs-lookup"><span data-stu-id="ff0ba-114">Q: If a device is already encrypted with Bitlocker using the OS default settings for encryption method and cipher strength (XTS-AES-128), will applying a policy with different settings automatically trigger re-encryption of the drive with the new settings?</span></span><br>
<span data-ttu-id="ff0ba-115">A: tidak.</span><span class="sxs-lookup"><span data-stu-id="ff0ba-115">A: No.</span></span> <span data-ttu-id="ff0ba-116">Untuk menerapkan pengaturan penyandian baru, kandar harus didekripsi terlebih dahulu.</span><span class="sxs-lookup"><span data-stu-id="ff0ba-116">To apply the new cipher settings, the drive must first be decrypted.</span></span><br><br>
<span data-ttu-id="ff0ba-117">**Catatan:** Untuk perangkat yang terdaftar dengan autopilot, enkripsi otomatis yang akan terjadi selama OOBE tidak dipicu hingga Intune kebijakan dievaluasi, yang memungkinkan pengaturan berbasis kebijakan untuk digunakan di tempat OS asali.</span><span class="sxs-lookup"><span data-stu-id="ff0ba-117">**Note:** For devices being enrolled with Autopilot, the automatic encryption that would occur during OOBE is not triggered until Intune policy is evaluated, which allows the policy-based settings to be used in place of the OS defaults.</span></span>
 
<span data-ttu-id="ff0ba-118">Q: jika perangkat dienkripsi sebagai akibat dari penerapan kebijakan Intune, akan didekripsi ketika kebijakan yang dihapus?</span><span class="sxs-lookup"><span data-stu-id="ff0ba-118">Q: If a device is encrypted as a result of the  application of Intune policy, will it be decrypted when that policy is removed?</span></span><br>
<span data-ttu-id="ff0ba-119">A: penghapusan Kebijakan terkait enkripsi tidak mengakibatkan dekripsi kandar yang dikonfigurasi.</span><span class="sxs-lookup"><span data-stu-id="ff0ba-119">A: Removal of encryption-related policy does NOT result in decryption of the drives that were configured.</span></span>
 
<span data-ttu-id="ff0ba-120">T: Mengapa kebijakan kepatuhan Intune menunjukkan bahwa perangkat saya tidak memiliki BitLocker diaktifkan, meskipun itu?</span><span class="sxs-lookup"><span data-stu-id="ff0ba-120">Q: Why does Intune Compliance Policy show that my device does not have Bitlocker enabled, even though it is?</span></span><br>
<span data-ttu-id="ff0ba-121">A: "BitLocker diaktifkan" pengaturan kebijakan kepatuhan Intune menggunakan klien Windows perangkat kesehatan Attestation (DHA).</span><span class="sxs-lookup"><span data-stu-id="ff0ba-121">A: The "Bitlocker enabled" setting in the Intune Compliance Policy utilizes the Windows Device Health Attestation  (DHA) client.</span></span> <span data-ttu-id="ff0ba-122">Klien ini hanya mengukur status perangkat pada saat boot.</span><span class="sxs-lookup"><span data-stu-id="ff0ba-122">This client only measures device state at boot time.</span></span> <span data-ttu-id="ff0ba-123">Jadi, jika perangkat belum reboot sejak enkripsi BitLocker selesai, Layanan klien DHA tidak akan melaporkan BitLocker sebagai aktif.</span><span class="sxs-lookup"><span data-stu-id="ff0ba-123">So if a device has not been rebooted since Bitlocker encryption was completed, the DHA client service will not report Bitlocker as being active.</span></span>
 
 