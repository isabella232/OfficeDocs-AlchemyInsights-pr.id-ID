---
title: Aturan pengurangan permukaan serangan
ms.author: pebaum
author: pebaum
manager: scotv
ms.date: 05/25/2021
ms.audience: Admin
ms.topic: article
ms.service: o365-administration
ROBOTS: NOINDEX, NOFOLLOW
localization_priority: Priority
ms.collection: Adm_O365
ms.custom:
- "11228"
- "9005470"
ms.openlocfilehash: 99feaa5c3f35a0bb78b99f47ac2be88cf3e1b62a
ms.sourcegitcommit: 4b504650e11adb9894c37b6d8608b53f9d5fc13d
ms.translationtype: MT
ms.contentlocale: id-ID
ms.lasthandoff: 05/25/2021
ms.locfileid: "52676446"
---
# <a name="attack-surface-reduction-rules"></a><span data-ttu-id="302b0-102">Aturan pengurangan permukaan serangan</span><span class="sxs-lookup"><span data-stu-id="302b0-102">Attack surface reduction rules</span></span>

<span data-ttu-id="302b0-103">Tidak termasuk file atau folder yang dapat mengurangi tingkat proteksi yang diberikan oleh aturan pengurangan serangan permukaan.</span><span class="sxs-lookup"><span data-stu-id="302b0-103">Excluding files or folders can severely reduce the protection provided by attack surface reduction rules.</span></span> <span data-ttu-id="302b0-104">File yang diblokir oleh aturan diperbolehkan untuk berjalan, dan tidak ada laporan atau kejadian yang direkam.</span><span class="sxs-lookup"><span data-stu-id="302b0-104">Files that would have been blocked by a rule are allowed to run, and no report or event is recorded.</span></span> <span data-ttu-id="302b0-105">Pengecualian berlaku untuk semua aturan yang mengizinkan pengecualian.</span><span class="sxs-lookup"><span data-stu-id="302b0-105">An exclusion applies to all rules that allow exclusions.</span></span>

<span data-ttu-id="302b0-106">Pengecualian ASR menggunakan sintaks yang sama Antivirus Pertahanan Microsoft pengecualian.</span><span class="sxs-lookup"><span data-stu-id="302b0-106">ASR exclusions use the same syntax as Microsoft Defender Antivirus exclusions.</span></span> <span data-ttu-id="302b0-107">Untuk detailnya, [lihat Mengonfigurasi dan memvalidasi pengecualian Antivirus Pertahanan Microsoft dipindai.](/microsoft-365/security/defender-endpoint/configure-exclusions-microsoft-defender-antivirus)</span><span class="sxs-lookup"><span data-stu-id="302b0-107">For details, see [Configure and validate exclusions for Microsoft Defender Antivirus scans](/microsoft-365/security/defender-endpoint/configure-exclusions-microsoft-defender-antivirus).</span></span> <span data-ttu-id="302b0-108">Untuk menghindari masalah, [tinjau Kesalahan umum untuk dihindari ketika menetapkan pengecualian](/microsoft-365/security/defender-endpoint/common-exclusion-mistakes-microsoft-defender-antivirus).</span><span class="sxs-lookup"><span data-stu-id="302b0-108">To avoid problems, review [Common mistakes to avoid when defining exclusions](/microsoft-365/security/defender-endpoint/common-exclusion-mistakes-microsoft-defender-antivirus).</span></span>

<span data-ttu-id="302b0-109">Tidak semua aturan ASR mendukung pengecualian.</span><span class="sxs-lookup"><span data-stu-id="302b0-109">Not all ASR rules support exclusions.</span></span> <span data-ttu-id="302b0-110">Untuk memvalidasi jika aturan Anda mendukung pengecualian, lihat tabel [Aturan pengurangan permukaan serangan](/microsoft-365/security/defender-endpoint/attack-surface-reduction#attack-surface-reduction-rules).</span><span class="sxs-lookup"><span data-stu-id="302b0-110">To validate if your rule supports exclusions, see the table [Attack surface reduction rules](/microsoft-365/security/defender-endpoint/attack-surface-reduction#attack-surface-reduction-rules).</span></span>

## <a name="attack-surface-reduction-rules"></a><span data-ttu-id="302b0-111">Aturan pengurangan permukaan serangan</span><span class="sxs-lookup"><span data-stu-id="302b0-111">Attack surface reduction rules</span></span>

<span data-ttu-id="302b0-112">Permukaan serangan organisasi Anda mencakup semua tempat di mana penyerang bisa membahayakan perangkat atau jaringan organisasi.</span><span class="sxs-lookup"><span data-stu-id="302b0-112">Your organization attack surface includes all the places where an attacker could compromise organization devices or networks.</span></span> <span data-ttu-id="302b0-113">Mengurangi tingkat serangan Anda berarti melindungi perangkat dan jaringan organisasi, yang meninggalkan penyerang dengan lebih sedikit cara untuk melakukan serangan.</span><span class="sxs-lookup"><span data-stu-id="302b0-113">Reducing your attack surface means protecting the organization devices and network, which leaves attackers with fewer ways to perform attacks.</span></span> <span data-ttu-id="302b0-114">Mengonfigurasi aturan pengurangan permukaan serangan di Pertahanan Microsoft untuk Titik Akhir dapat membantu.</span><span class="sxs-lookup"><span data-stu-id="302b0-114">Configuring attack surface reduction rules in Microsoft Defender for Endpoint can help.</span></span>

<span data-ttu-id="302b0-115">Untuk informasi selengkapnya, lihat:</span><span class="sxs-lookup"><span data-stu-id="302b0-115">For more information, see:</span></span>

- [<span data-ttu-id="302b0-116">Memetakan GUID aturan ASR ke nama</span><span class="sxs-lookup"><span data-stu-id="302b0-116">Map ASR rule GUID to name</span></span>](/microsoft-365/security/defender-endpoint/attack-surface-reduction#attack-surface-reduction-rules)
- <span data-ttu-id="302b0-117">Persyaratan aturan ASR:</span><span class="sxs-lookup"><span data-stu-id="302b0-117">ASR rules requirements:</span></span>
    - [<span data-ttu-id="302b0-118">Windows 10 Pro, versi 1709 atau lebih baru</span><span class="sxs-lookup"><span data-stu-id="302b0-118">Windows 10 Pro, version 1709 or later</span></span>](/windows/whats-new/whats-new-windows-10-version-1709)
    - [<span data-ttu-id="302b0-119">Windows 10 Enterprise, versi 1709 atau lebih baru</span><span class="sxs-lookup"><span data-stu-id="302b0-119">Windows 10 Enterprise, version 1709 or later</span></span>](/windows/whats-new/whats-new-windows-10-version-1709)
    - [<span data-ttu-id="302b0-120">Windows Server, versi 1803 (Saluran Semi Tahunan) atau yang lebih baru</span><span class="sxs-lookup"><span data-stu-id="302b0-120">Windows Server, version 1803 (Semi-Annual Channel) or later</span></span>](/windows-server/get-started/whats-new-in-windows-server-1803)

## <a name="identify-the-correct-exclusion-to-apply"></a><span data-ttu-id="302b0-121">Identifikasi pengecualian yang benar untuk diterapkan</span><span class="sxs-lookup"><span data-stu-id="302b0-121">Identify the correct exclusion to apply</span></span>

1. <span data-ttu-id="302b0-122">Cari ID kejadian 1121 atau 1122 dalam log Microsoft-Windows-Pertahanan Windows/Operational.</span><span class="sxs-lookup"><span data-stu-id="302b0-122">Look for eventID 1121 or 1122 in the Microsoft-Windows-Windows Defender/Operational log.</span></span>

1. <span data-ttu-id="302b0-123">Evaluasi skenario dan konteks blokir dan konfirmasi bahwa skenario ini perlu dibuka blokirnya.</span><span class="sxs-lookup"><span data-stu-id="302b0-123">Evaluate the block scenario and context and confirm that this scenario needs to be unblocked.</span></span>

1. <span data-ttu-id="302b0-124">Baca nilai Jalur dalam detail kejadian, yang merupakan nilai yang menentukan pengecualian.</span><span class="sxs-lookup"><span data-stu-id="302b0-124">Read the Path value in the event details, which is the value that defines the exclusion.</span></span>
    - <span data-ttu-id="302b0-125">Buat pengecualian tersebut sedada mungkin.</span><span class="sxs-lookup"><span data-stu-id="302b0-125">Make the exclusion as strict as possible.</span></span>
    - <span data-ttu-id="302b0-126">Terapkan wildcard jika diperlukan (misalnya, ganti Variabel pengguna).</span><span class="sxs-lookup"><span data-stu-id="302b0-126">Apply a wildcard where needed (for example, replace User variable).</span></span>

1. <span data-ttu-id="302b0-127">Terapkan pengecualian sesuai kebutuhan penggunaan Anda.</span><span class="sxs-lookup"><span data-stu-id="302b0-127">Apply the exclusion according to your deployment needs.</span></span> <span data-ttu-id="302b0-128">Untuk detailnya, [lihat Mengustomisasi aturan pengurangan serangan permukaan.](/microsoft-365/security/defender-endpoint/customize-attack-surface-reduction)</span><span class="sxs-lookup"><span data-stu-id="302b0-128">For details, see [Customize attack surface reduction rules](/microsoft-365/security/defender-endpoint/customize-attack-surface-reduction).</span></span>

## <a name="exclusion-is-not-honored"></a><span data-ttu-id="302b0-129">Pengecualian tidak dilakukan</span><span class="sxs-lookup"><span data-stu-id="302b0-129">Exclusion is not honored</span></span>

1. <span data-ttu-id="302b0-130">Tentukan apakah aturan mendukung pengecualian.</span><span class="sxs-lookup"><span data-stu-id="302b0-130">Determine whether the rule support exclusions.</span></span> <span data-ttu-id="302b0-131">Untuk detailnya, [lihat Aturan pengurangan serangan permukaan.](/microsoft-365/security/defender-endpoint/attack-surface-reduction#attack-surface-reduction-rules)</span><span class="sxs-lookup"><span data-stu-id="302b0-131">For details, see [Attack surface reduction rules](/microsoft-365/security/defender-endpoint/attack-surface-reduction#attack-surface-reduction-rules).</span></span>

1. <span data-ttu-id="302b0-132">Tinjau pengecualian yang diterapkan dan verifikasi dengan data kejadian kesalahan ketik atau salah interpretasi wildcard.</span><span class="sxs-lookup"><span data-stu-id="302b0-132">Review the exclusions applied and verify with the event data for typos or misinterpreted wildcards.</span></span> <span data-ttu-id="302b0-133">Untuk informasi selengkapnya, lihat [Tipe pengecualian yang didukung](/microsoft-365/security/defender-endpoint/mac-exclusions#supported-exclusion-types)</span><span class="sxs-lookup"><span data-stu-id="302b0-133">For more info, see [Supported exclusion types](/microsoft-365/security/defender-endpoint/mac-exclusions#supported-exclusion-types)</span></span>

1. <span data-ttu-id="302b0-134">jika dampak aturan terlalu tinggi, pertimbangkan untuk memindahkan aturan (kembali) ke mode Audit untuk melakukan validasi lebih lanjut.</span><span class="sxs-lookup"><span data-stu-id="302b0-134">if the impact of the rule it too high, consider moving the rule (back) to Audit mode to perform further validation.</span></span> <span data-ttu-id="302b0-135">Untuk detailnya, [lihat Menguji cara fitur Titik Akhir pertahanan Microsoft berfungsi dalam mode audit.](/microsoft-365/security/defender-endpoint/audit-windows-defender)</span><span class="sxs-lookup"><span data-stu-id="302b0-135">For details, see [Test how Microsoft Defender for Endpoint features work in audit mode](/microsoft-365/security/defender-endpoint/audit-windows-defender).</span></span>

1. <span data-ttu-id="302b0-136">Mengumpulkan data dukungan untuk membuka kasus dukungan dengan menggunakan perintah ini:</span><span class="sxs-lookup"><span data-stu-id="302b0-136">Collect support data to open a support case by using this command:</span></span>
    
   <span data-ttu-id="302b0-137">\*\* MDEClientAnalyzer.cmd -v\*\*</span><span class="sxs-lookup"><span data-stu-id="302b0-137">\*\* MDEClientAnalyzer.cmd -v\*\*</span></span>

    <span data-ttu-id="302b0-138">Untuk informasi selengkapnya, [lihat Masalah mesin onboarding ke Pertahanan Microsoft untuk Titik Akhir](issues-with-onboarding-machines.md).</span><span class="sxs-lookup"><span data-stu-id="302b0-138">For more information, see [Issues with onboarding machines to Microsoft Defender for Endpoints](issues-with-onboarding-machines.md).</span></span>
