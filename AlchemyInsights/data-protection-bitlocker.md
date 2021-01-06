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
ms.openlocfilehash: 0b305931a7279d8f1085c411cc9b47c991e1ee44
ms.sourcegitcommit: 9c4b4853ff53f21c0177d48821846070bb00637c
ms.translationtype: MT
ms.contentlocale: id-ID
ms.lasthandoff: 01/06/2021
ms.locfileid: "49768820"
---
# <a name="enabling-bitlocker-encryption-with-intune"></a><span data-ttu-id="421b6-102">Mengaktifkan enkripsi BitLocker dengan Intune</span><span class="sxs-lookup"><span data-stu-id="421b6-102">Enabling Bitlocker encryption with Intune</span></span>

 <span data-ttu-id="421b6-103">Kebijakan proteksi titik akhir Intune dapat digunakan untuk mengonfigurasi pengaturan enkripsi BitLocker untuk perangkat Windows.</span><span class="sxs-lookup"><span data-stu-id="421b6-103">Intune Endpoint Protection Policy can be used to configure Bitlocker encryption settings for Windows devices.</span></span> <span data-ttu-id="421b6-104">Untuk informasi selengkapnya, lihat [pengaturan Windows 10 (dan yang lebih baru) untuk memproteksi perangkat menggunakan Intune](https://docs.microsoft.com/intune/endpoint-protection-windows-10#windows-encryption).</span><span class="sxs-lookup"><span data-stu-id="421b6-104">For more information, see [Windows 10 (and later) settings to protect devices using Intune](https://docs.microsoft.com/intune/endpoint-protection-windows-10#windows-encryption).</span></span>
 
<span data-ttu-id="421b6-105">Anda harus mengetahui bahwa banyak perangkat yang lebih baru yang menjalankan Windows 10 mendukung enkripsi BitLocker otomatis, yang dipicu tanpa penerapan kebijakan MDM.</span><span class="sxs-lookup"><span data-stu-id="421b6-105">You should be aware that many newer devices running Windows 10 support automatic Bitlocker encryption, which is triggered without the application of MDM policy.</span></span> <span data-ttu-id="421b6-106">Hal ini dapat berdampak pada penerapan kebijakan jika pengaturan non-default dikonfigurasikan.</span><span class="sxs-lookup"><span data-stu-id="421b6-106">This may impact application of policy if non-default settings are configured.</span></span> <span data-ttu-id="421b6-107">Lihat Tanya Jawab Umum berikut untuk detail selengkapnya.</span><span class="sxs-lookup"><span data-stu-id="421b6-107">See the following FAQ for more detail.</span></span>
 
<span data-ttu-id="421b6-108">Untuk informasi tentang pemecahan masalah BitLocker, lihat [memecahkan masalah kebijakan BitLocker di Microsoft Intune](https://docs.microsoft.com/intune/protect/troubleshoot-bitlocker-policies).</span><span class="sxs-lookup"><span data-stu-id="421b6-108">For information about troubleshooting bitlocker issues, see [Troubleshoot BitLocker policies in Microsoft Intune](https://docs.microsoft.com/intune/protect/troubleshoot-bitlocker-policies).</span></span>
 
 
<span data-ttu-id="421b6-109">**FAQ**</span><span class="sxs-lookup"><span data-stu-id="421b6-109">**FAQ**</span></span>

<span data-ttu-id="421b6-110">P: yang edisi enkripsi perangkat dukungan Windows menggunakan kebijakan perlindungan titik akhir?</span><span class="sxs-lookup"><span data-stu-id="421b6-110">Q: Which editions of Windows support device encryption using the Endpoint Protection Policy?</span></span><br>
<span data-ttu-id="421b6-111">A: pengaturan dalam kebijakan perlindungan titik akhir Intune diimplementasikan menggunakan [CSP CSP](https://docs.microsoft.com/windows/client-management/mdm/bitlocker-csp).</span><span class="sxs-lookup"><span data-stu-id="421b6-111">A: The settings in Intune Endpoint Protection Policy are implemented using the [Bitlocker CSP](https://docs.microsoft.com/windows/client-management/mdm/bitlocker-csp).</span></span> <span data-ttu-id="421b6-112">Tidak semua edisi atau Build Windows mendukung BitLocker CSP.</span><span class="sxs-lookup"><span data-stu-id="421b6-112">Not all editions or builds of Windows support the Bitlocker CSP.</span></span> <br><br>

<span data-ttu-id="421b6-113">P: Bagaimana cara BitLocker diaktifkan di perangkat tanpa memerlukan interaksi pengguna akhir?</span><span class="sxs-lookup"><span data-stu-id="421b6-113">Q: How can Bitlocker be enabled on devices without requiring end user interaction?</span></span><br>
<span data-ttu-id="421b6-114">A: selama prasyarat yang diperlukan terpenuhi, dimungkinkan untuk mengaktifkan BitLocker "Silent Encryption" melalui Intune.</span><span class="sxs-lookup"><span data-stu-id="421b6-114">A: So long as the necessary pre-requisites are met it is possible to enable Bitlocker "Silent Encryption" through Intune.</span></span> <span data-ttu-id="421b6-115">Lihat detail persyaratan perangkat dan pengaturan kebijakan contoh untuk mengaktifkan enkripsi hening dalam dokumen berikut: [mengaktifkan diam-diam enkripsi BitLocker](https://docs.microsoft.com/mem/intune/protect/encrypt-devices#silently-enable-bitlocker-on-devices).</span><span class="sxs-lookup"><span data-stu-id="421b6-115">See the details of the device requirements and example policy settings to enable silent encryption in the following doc: [Silently Enable Bitlocker Encryption](https://docs.microsoft.com/mem/intune/protect/encrypt-devices#silently-enable-bitlocker-on-devices).</span></span> <br><br>

<span data-ttu-id="421b6-116">P: jika perangkat telah dienkripsi dengan BitLocker menggunakan pengaturan default OS untuk metode enkripsi dan kekuatan cipher (XTS-AES-128), akan menerapkan kebijakan dengan pengaturan yang berbeda secara otomatis memicu enkripsi ulang drive dengan pengaturan baru?</span><span class="sxs-lookup"><span data-stu-id="421b6-116">Q: If a device is already encrypted with Bitlocker using the OS default settings for encryption method and cipher strength (XTS-AES-128), will applying a policy with different settings automatically trigger re-encryption of the drive with the new settings?</span></span><br>
<span data-ttu-id="421b6-117">J: Tidak.</span><span class="sxs-lookup"><span data-stu-id="421b6-117">A: No.</span></span> <span data-ttu-id="421b6-118">Untuk menerapkan pengaturan penyandian baru, drive harus didekripsi terlebih dahulu.</span><span class="sxs-lookup"><span data-stu-id="421b6-118">To apply the new cipher settings, the drive must first be decrypted.</span></span><br><br>
<span data-ttu-id="421b6-119">**Catatan:** Untuk perangkat yang terdaftar dengan autopilot, enkripsi otomatis yang akan terjadi selama OOBE tidak dipicu hingga kebijakan Intune dievaluasi, yang memungkinkan pengaturan berbasis kebijakan digunakan di tempat default OS.</span><span class="sxs-lookup"><span data-stu-id="421b6-119">**Note:** For devices being enrolled with Autopilot, the automatic encryption that would occur during OOBE is not triggered until Intune policy is evaluated, which allows the policy-based settings to be used in place of the OS defaults.</span></span>
 
<span data-ttu-id="421b6-120">P: jika perangkat dienkripsi sebagai hasil dari penerapan kebijakan Intune, Apakah perangkat akan didekripsi saat kebijakan tersebut dihapus?</span><span class="sxs-lookup"><span data-stu-id="421b6-120">Q: If a device is encrypted as a result of the  application of Intune policy, will it be decrypted when that policy is removed?</span></span><br>
<span data-ttu-id="421b6-121">A: penghapusan Kebijakan terkait enkripsi tidak mengakibatkan dekripsi drive yang dikonfigurasi.</span><span class="sxs-lookup"><span data-stu-id="421b6-121">A: Removal of encryption-related policy does NOT result in decryption of the drives that were configured.</span></span>
 
<span data-ttu-id="421b6-122">P: Mengapa kebijakan kepatuhan Intune memperlihatkan bahwa perangkat saya tidak memiliki BitLocker yang diaktifkan, meskipun itu?</span><span class="sxs-lookup"><span data-stu-id="421b6-122">Q: Why does Intune Compliance Policy show that my device does not have Bitlocker enabled, even though it is?</span></span><br>
<span data-ttu-id="421b6-123">A: Pengaturan "BitLocker enabled" dalam kebijakan Intune Compliance menggunakan klien Windows Device Health Attestation (DHA).</span><span class="sxs-lookup"><span data-stu-id="421b6-123">A: The "Bitlocker enabled" setting in the Intune Compliance Policy utilizes the Windows Device Health Attestation  (DHA) client.</span></span> <span data-ttu-id="421b6-124">Klien ini hanya mengukur status perangkat pada waktu boot.</span><span class="sxs-lookup"><span data-stu-id="421b6-124">This client only measures device state at boot time.</span></span> <span data-ttu-id="421b6-125">Jadi jika perangkat belum diboot ulang karena enkripsi BitLocker telah selesai, Layanan klien DHA tidak akan melaporkan BitLocker sebagai aktif.</span><span class="sxs-lookup"><span data-stu-id="421b6-125">So if a device has not been rebooted since Bitlocker encryption was completed, the DHA client service will not report Bitlocker as being active.</span></span>
 
 