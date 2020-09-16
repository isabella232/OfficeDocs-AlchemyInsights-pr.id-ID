---
title: DataProtection-BitLocker
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
- "1802"
- "9000220"
ms.openlocfilehash: ab28162fcdf0a37060be3bdf15a78aceca7a48b1
ms.sourcegitcommit: c6692ce0fa1358ec3529e59ca0ecdfdea4cdc759
ms.translationtype: MT
ms.contentlocale: id-ID
ms.lasthandoff: 09/14/2020
ms.locfileid: "47731242"
---
# <a name="enabling-bitlocker-encryption-with-intune"></a><span data-ttu-id="2b44a-102">Mengaktifkan enkripsi BitLocker dengan Intune</span><span class="sxs-lookup"><span data-stu-id="2b44a-102">Enabling Bitlocker encryption with Intune</span></span>

 <span data-ttu-id="2b44a-103">Kebijakan proteksi titik akhir Intune dapat digunakan untuk mengonfigurasi pengaturan enkripsi BitLocker untuk perangkat Windows.</span><span class="sxs-lookup"><span data-stu-id="2b44a-103">Intune Endpoint Protection Policy can be used to configure Bitlocker encryption settings for Windows devices.</span></span> <span data-ttu-id="2b44a-104">Untuk informasi selengkapnya, lihat [pengaturan Windows 10 (dan yang lebih baru) untuk memproteksi perangkat menggunakan Intune](https://docs.microsoft.com/intune/endpoint-protection-windows-10#windows-encryption).</span><span class="sxs-lookup"><span data-stu-id="2b44a-104">For more information, see [Windows 10 (and later) settings to protect devices using Intune](https://docs.microsoft.com/intune/endpoint-protection-windows-10#windows-encryption).</span></span>
 
<span data-ttu-id="2b44a-105">Anda harus mengetahui bahwa banyak perangkat yang lebih baru yang menjalankan Windows 10 mendukung enkripsi BitLocker otomatis, yang dipicu tanpa penerapan kebijakan MDM.</span><span class="sxs-lookup"><span data-stu-id="2b44a-105">You should be aware that many newer devices running Windows 10 support automatic Bitlocker encryption, which is triggered without the application of MDM policy.</span></span> <span data-ttu-id="2b44a-106">Hal ini dapat berdampak pada penerapan kebijakan jika pengaturan non-default dikonfigurasikan.</span><span class="sxs-lookup"><span data-stu-id="2b44a-106">This may impact application of policy if non-default settings are configured.</span></span> <span data-ttu-id="2b44a-107">Lihat Tanya Jawab Umum berikut untuk detail selengkapnya.</span><span class="sxs-lookup"><span data-stu-id="2b44a-107">See the following FAQ for more detail.</span></span>
 
<span data-ttu-id="2b44a-108">Untuk informasi tentang pemecahan masalah BitLocker, lihat [memecahkan masalah kebijakan BitLocker di Microsoft Intune](https://docs.microsoft.com/intune/protect/troubleshoot-bitlocker-policies).</span><span class="sxs-lookup"><span data-stu-id="2b44a-108">For information about troubleshooting bitlocker issues, see [Troubleshoot BitLocker policies in Microsoft Intune](https://docs.microsoft.com/intune/protect/troubleshoot-bitlocker-policies).</span></span>
 
 
<span data-ttu-id="2b44a-109">**FAQ**</span><span class="sxs-lookup"><span data-stu-id="2b44a-109">**FAQ**</span></span>

 <span data-ttu-id="2b44a-110">P: yang edisi enkripsi perangkat dukungan Windows menggunakan kebijakan perlindungan titik akhir?</span><span class="sxs-lookup"><span data-stu-id="2b44a-110">Q: Which editions of Windows support device encryption using the Endpoint Protection Policy?</span></span><br>
 <span data-ttu-id="2b44a-111">A: pengaturan dalam kebijakan perlindungan titik akhir Intune diimplementasikan menggunakan [CSP CSP](https://docs.microsoft.com/windows/client-management/mdm/bitlocker-csp).</span><span class="sxs-lookup"><span data-stu-id="2b44a-111">A: The settings in Intune Endpoint Protection Policy  are implemented using the [Bitlocker CSP](https://docs.microsoft.com/windows/client-management/mdm/bitlocker-csp).</span></span> <span data-ttu-id="2b44a-112">Tidak semua edisi atau Build Windows mendukung BitLocker CSP.</span><span class="sxs-lookup"><span data-stu-id="2b44a-112">Not all editions or builds of Windows support the Bitlocker CSP.</span></span> <br><br>
      <span data-ttu-id="2b44a-113">Saat ini, edisi Windows berikut ini didukung: Enterprise, Education, Mobile, Mobile Enterprise, dan Professional (Build 1809 dan yang lebih baru).</span><span class="sxs-lookup"><span data-stu-id="2b44a-113">At this time, the following Windows editions are supported: Enterprise, Education, Mobile, Mobile Enterprise, and Professional (build 1809 and later).</span></span>
 
<span data-ttu-id="2b44a-114">P: jika perangkat telah dienkripsi dengan BitLocker menggunakan pengaturan default OS untuk metode enkripsi dan kekuatan cipher (XTS-AES-128), akan menerapkan kebijakan dengan pengaturan yang berbeda secara otomatis memicu enkripsi ulang drive dengan pengaturan baru?</span><span class="sxs-lookup"><span data-stu-id="2b44a-114">Q: If a device is already encrypted with Bitlocker using the OS default settings for encryption method and cipher strength (XTS-AES-128), will applying a policy with different settings automatically trigger re-encryption of the drive with the new settings?</span></span><br>
<span data-ttu-id="2b44a-115">J: Tidak.</span><span class="sxs-lookup"><span data-stu-id="2b44a-115">A: No.</span></span> <span data-ttu-id="2b44a-116">Untuk menerapkan pengaturan penyandian baru, drive harus didekripsi terlebih dahulu.</span><span class="sxs-lookup"><span data-stu-id="2b44a-116">To apply the new cipher settings, the drive must first be decrypted.</span></span><br><br>
<span data-ttu-id="2b44a-117">**Catatan:** Untuk perangkat yang terdaftar dengan autopilot, enkripsi otomatis yang akan terjadi selama OOBE tidak dipicu hingga kebijakan Intune dievaluasi, yang memungkinkan pengaturan berbasis kebijakan digunakan di tempat default OS.</span><span class="sxs-lookup"><span data-stu-id="2b44a-117">**Note:** For devices being enrolled with Autopilot, the automatic encryption that would occur during OOBE is not triggered until Intune policy is evaluated, which allows the policy-based settings to be used in place of the OS defaults.</span></span>
 
<span data-ttu-id="2b44a-118">P: jika perangkat dienkripsi sebagai hasil dari penerapan kebijakan Intune, Apakah perangkat akan didekripsi saat kebijakan tersebut dihapus?</span><span class="sxs-lookup"><span data-stu-id="2b44a-118">Q: If a device is encrypted as a result of the  application of Intune policy, will it be decrypted when that policy is removed?</span></span><br>
<span data-ttu-id="2b44a-119">A: penghapusan Kebijakan terkait enkripsi tidak mengakibatkan dekripsi drive yang dikonfigurasi.</span><span class="sxs-lookup"><span data-stu-id="2b44a-119">A: Removal of encryption-related policy does NOT result in decryption of the drives that were configured.</span></span>
 
<span data-ttu-id="2b44a-120">P: Mengapa kebijakan kepatuhan Intune memperlihatkan bahwa perangkat saya tidak memiliki BitLocker yang diaktifkan, meskipun itu?</span><span class="sxs-lookup"><span data-stu-id="2b44a-120">Q: Why does Intune Compliance Policy show that my device does not have Bitlocker enabled, even though it is?</span></span><br>
<span data-ttu-id="2b44a-121">A: Pengaturan "BitLocker enabled" dalam kebijakan Intune Compliance menggunakan klien Windows Device Health Attestation (DHA).</span><span class="sxs-lookup"><span data-stu-id="2b44a-121">A: The "Bitlocker enabled" setting in the Intune Compliance Policy utilizes the Windows Device Health Attestation  (DHA) client.</span></span> <span data-ttu-id="2b44a-122">Klien ini hanya mengukur status perangkat pada waktu boot.</span><span class="sxs-lookup"><span data-stu-id="2b44a-122">This client only measures device state at boot time.</span></span> <span data-ttu-id="2b44a-123">Jadi jika perangkat belum diboot ulang karena enkripsi BitLocker telah selesai, Layanan klien DHA tidak akan melaporkan BitLocker sebagai aktif.</span><span class="sxs-lookup"><span data-stu-id="2b44a-123">So if a device has not been rebooted since Bitlocker encryption was completed, the DHA client service will not report Bitlocker as being active.</span></span>
 
 