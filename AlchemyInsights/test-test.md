---
title: Persyaratan yang hilang dari penyimpanan istilah SharePoint online
ms.author: pebaum
author: pebaum
ms.date: 04/21/2020
ms.audience: ITPro
ms.topic: article
ms.service: o365-administration
ROBOTS: NOINDEX, NOFOLLOW
localization_priority: Normal
ms.custom:
- "1243"
- "5200021"
ms.openlocfilehash: 06711c289365c0fcdf71cf9cccf3cfc53511495a
ms.sourcegitcommit: c6692ce0fa1358ec3529e59ca0ecdfdea4cdc759
ms.translationtype: MT
ms.contentlocale: id-ID
ms.lasthandoff: 09/14/2020
ms.locfileid: "47750454"
---
# <a name="enabling-bitlocker-encryption-with-intune"></a><span data-ttu-id="25ab6-102">Mengaktifkan enkripsi BitLocker dengan Intune</span><span class="sxs-lookup"><span data-stu-id="25ab6-102">Enabling Bitlocker Encryption with Intune</span></span>

<span data-ttu-id="25ab6-103">Kebijakan proteksi titik akhir Intune dapat digunakan untuk mengonfigurasi pengaturan enkripsi Boitlocker untuk perangkat Windows seperti yang diuraikan dalam pengaturan: Windows10 (and later) untuk memproteksi perangkat menggunakan Intune</span><span class="sxs-lookup"><span data-stu-id="25ab6-103">Intune Endpoint Protection Policy can be used to configure Boitlocker encryption settings for Windows devices as described in : Windows10 (and later) settings to protect devices using Intune</span></span>

<span data-ttu-id="25ab6-104">Anda harus menyadari bahwa banyak perangkat yang lebih baru yang menjalankan Windows 10 mendukung enkripsi BitLocker otomatis yang dipicu tanpa penerapan kebijakan MDM.</span><span class="sxs-lookup"><span data-stu-id="25ab6-104">You should be aware that many newer devices running Windows 10 support automatic bitlocker encryption which is triggered without the application of MDM policy.</span></span> <span data-ttu-id="25ab6-105">Hal ini dapat berdampak pada penerapan kebijakan jika pengaturan non default dikonfigurasikan.</span><span class="sxs-lookup"><span data-stu-id="25ab6-105">This may impact application of policy if non default settings are configured.</span></span> <span data-ttu-id="25ab6-106">Lihat Tanya Jawab Umum untuk detail selengkapnya.</span><span class="sxs-lookup"><span data-stu-id="25ab6-106">See FAQ for more detail.</span></span>


<span data-ttu-id="25ab6-107">Tanya Jawab Umum   p: yang edisi enkripsi perangkat dukungan Windows menggunakan kebijakan perlindungan titik akhir?</span><span class="sxs-lookup"><span data-stu-id="25ab6-107">FAQ  Q: Which editions of Windows support device encryption using the Endpoint Protection Policy?</span></span>
<span data-ttu-id="25ab6-108"> A: pengaturan dalam kebijakan perlindungan titik akhir Intune diimplementasikan menggunakan CSP CSP.</span><span class="sxs-lookup"><span data-stu-id="25ab6-108"> A: The settings in Intune Endpoint Protection Policy  are implemented using the Bitlocker CSP.</span></span><span data-ttu-id="25ab6-109">Tidak semua edisi maupun Build Windows mendukung BitLocker CSP. 
     </span><span class="sxs-lookup"><span data-stu-id="25ab6-109">  Not all editions nor builds of Windows support the Bitlocker CSP. 
     </span></span> <span data-ttu-id="25ab6-110">Pada saat ini edisi Windows: Enterprise; Pendidikan, seluler, Mobile Enterprise dan Professional (dari Build 1809 seterusnya) didukung.</span><span class="sxs-lookup"><span data-stu-id="25ab6-110">At this time Windows Editions: Enterprise; Education, Mobile, Mobile Enterprise and Professional (from build 1809 onwards) are supported.</span></span>




<span data-ttu-id="25ab6-111">P: jika perangkat telah dienkripsi dengan BitLocker menggunakan pengaturan default OS untuk metode enkripsi dan kekuatan penyandian (XTS-AES-128) akan menerapkan kebijakan dengan pengaturan berbeda secara otomatis memicu enkripsi ulang drive dengan pengaturan baru?</span><span class="sxs-lookup"><span data-stu-id="25ab6-111">Q: If a device is already encrypted with Bitlocker using the OS default settings for encryption method and cipher strength (XTS-AES-128)  will applying a policy with different settings automatically trigger re-encryption of the drive with the new settings?</span></span>

<span data-ttu-id="25ab6-112">J: Tidak.</span><span class="sxs-lookup"><span data-stu-id="25ab6-112">A: No.</span></span> <span data-ttu-id="25ab6-113">Untuk menerapkan pengaturan cipher baru, drive harus didekripsi terlebih dahulu.</span><span class="sxs-lookup"><span data-stu-id="25ab6-113">In order to apply the new cipher settings the drive must first be decrypted.</span></span>

<span data-ttu-id="25ab6-114">Catatan untuk perangkat yang terdaftar dengan autopilot enkripsi otomatis yang akan terjadi selama OOBE tidak dipicu hingga kebijakan Intune dievaluasi yang memungkinkan pengaturan berbasis kebijakan digunakan di tempat default OS</span><span class="sxs-lookup"><span data-stu-id="25ab6-114">Note For devices being enrolled with Autopilot the automatic encryption that would occur during OOBE is not triggered until Intune policy is evaluated which allows the policy based settings to be used in place of the OS defaults</span></span>




<span data-ttu-id="25ab6-115">P jika perangkat dienkripsi sebagai hasil dari penerapan kebijakan Intune akan didekripsi saat kebijakan tersebut dihapus?</span><span class="sxs-lookup"><span data-stu-id="25ab6-115">Q If a device is encrypted as a result of the  application of Intune policy will it be decrypted when that policy is removed?</span></span>

<span data-ttu-id="25ab6-116">J: penghapusan Kebijakan terkait enkripsi tidak mengakibatkan dekripsi drive yang dikonfigurasi.</span><span class="sxs-lookup"><span data-stu-id="25ab6-116">A: Removal of encryption related policy does NOT result in decryption of the drives which were configured.</span></span>




<span data-ttu-id="25ab6-117">P: Mengapa kebijakan kepatuhan Intune memperlihatkan bahwa perangkat saya tidak memiliki "BitLocker diaktifkan" tapi itu?</span><span class="sxs-lookup"><span data-stu-id="25ab6-117">Q: Why does intune Compliance policy show that my device does not have "Bitlocker Enabled" but it is?</span></span>

<span data-ttu-id="25ab6-118">A: Pengaturan "BitLocker enabled" dalam kebijakan kepatuhan Intune menggunakan klien Windows Device Health Attestation (DHA).</span><span class="sxs-lookup"><span data-stu-id="25ab6-118">A: The "Bitlocker enabled" setting in intune compliance policy utilizes the Windows Device Health Attestation  (DHA) client.</span></span> <span data-ttu-id="25ab6-119">Klien ini hanya mengukur status perangkat pada waktu boot.</span><span class="sxs-lookup"><span data-stu-id="25ab6-119">This client only measures device state at boot time.</span></span> <span data-ttu-id="25ab6-120">Jadi jika perangkat belum diboot ulang karena enkripsi BitLocker telah selesai, Layanan klien DHA tidak akan melaporkan BitLocker sebagai aktif.</span><span class="sxs-lookup"><span data-stu-id="25ab6-120">So if a device has not been rebooted since bitlocker encryption was completed the DHA client service will not report bitlocker as being active.</span></span>