---
title: Indikator tidak berfungsi menggunakan browser Edge
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
- "11230"
- "9005470"
ms.openlocfilehash: df62d965e0dc2ddb656571af99b1e4c3cb52ea35
ms.sourcegitcommit: 4b504650e11adb9894c37b6d8608b53f9d5fc13d
ms.translationtype: MT
ms.contentlocale: id-ID
ms.lasthandoff: 05/25/2021
ms.locfileid: "52676470"
---
# <a name="indicators-dont-work-using-edge-browser"></a><span data-ttu-id="8e3f5-102">Indikator tidak berfungsi menggunakan browser Edge</span><span class="sxs-lookup"><span data-stu-id="8e3f5-102">Indicators don't work using Edge browser</span></span>

<span data-ttu-id="8e3f5-103">Setelah Anda membuat Indikator, Indikator tidak digunakan oleh Edge (Smartscreen).</span><span class="sxs-lookup"><span data-stu-id="8e3f5-103">After you created an Indicator, it's not honored by Edge (Smartscreen).</span></span> <span data-ttu-id="8e3f5-104">Untuk informasi selengkapnya, [lihat Membuat indikator untuk IP dan URL/domain](/microsoft-365/security/defender-endpoint/indicator-ip-domain).</span><span class="sxs-lookup"><span data-stu-id="8e3f5-104">For more information, see [Create indicators for IPs and URLs/domains](/microsoft-365/security/defender-endpoint/indicator-ip-domain).</span></span>

## <a name="step-1-ensure-the-following"></a><span data-ttu-id="8e3f5-105">Langkah 1: Pastikan hal berikut ini</span><span class="sxs-lookup"><span data-stu-id="8e3f5-105">Step 1: Ensure the following</span></span>

- <span data-ttu-id="8e3f5-106">Pastikan bahwa indikator sudah benar (tidak ada kesalahan ketik dalam IP/URL, tindakan yang benar, grup RBAC yang benar).</span><span class="sxs-lookup"><span data-stu-id="8e3f5-106">Verify that the indicator is correct (no typos in IP/URL, correct action, the correct RBAC groups).</span></span>
- <span data-ttu-id="8e3f5-107">Tunggu setidaknya 2 jam setelah membuat indikator untuk memperhitungkan latensi yang mungkin.</span><span class="sxs-lookup"><span data-stu-id="8e3f5-107">Wait the minimum 2 hours after creating the indicator to take into account any possible latency.</span></span>
- <span data-ttu-id="8e3f5-108">Konfirmasi bahwa sistem telah onboarded ke Pertahanan Microsoft untuk Titik Akhir.</span><span class="sxs-lookup"><span data-stu-id="8e3f5-108">Confirm that the system(s) are onboarded to Microsoft Defender for Endpoint.</span></span>
- <span data-ttu-id="8e3f5-109">Verifikasi bahwa sistem dapat berkomunikasi dengan Awan.</span><span class="sxs-lookup"><span data-stu-id="8e3f5-109">Verify that system(s) can communicate with the Cloud.</span></span>
- <span data-ttu-id="8e3f5-110">Pastikan bahwa Smartscreen telah diaktifkan dan dapat dijangkau dengan masuk ke [situs uji](https://demo.smartscreen.msft.net).</span><span class="sxs-lookup"><span data-stu-id="8e3f5-110">Verify that Smartscreen is enabled and reachable by going to the [test site](https://demo.smartscreen.msft.net).</span></span>

## <a name="step-2-troubleshoot-the-potential-issue"></a><span data-ttu-id="8e3f5-111">Langkah 2: Memecahkan masalah yang potensial</span><span class="sxs-lookup"><span data-stu-id="8e3f5-111">Step 2: Troubleshoot the potential issue</span></span>

- <span data-ttu-id="8e3f5-112">Pastikan klien memenuhi persyaratan.</span><span class="sxs-lookup"><span data-stu-id="8e3f5-112">Make sure the client meets the requirements.</span></span> <span data-ttu-id="8e3f5-113">Untuk detailnya, [lihat Membuat indikator untuk IP dan URL/domain](/microsoft-365/security/defender-endpoint/indicator-ip-domain).</span><span class="sxs-lookup"><span data-stu-id="8e3f5-113">For details, see [Create indicators for IPs and URLs/domains](/microsoft-365/security/defender-endpoint/indicator-ip-domain).</span></span>
- <span data-ttu-id="8e3f5-114">Pastikan Anda menjalankan versi terbaru browser Edge.</span><span class="sxs-lookup"><span data-stu-id="8e3f5-114">Make sure you're running the latest version of the Edge browser.</span></span> <span data-ttu-id="8e3f5-115">Untuk mencari tahu versi terbaru, lihat [Mencari tahu versi uji Microsoft Edge Anda miliki](https://support.microsoft.com/microsoft-edge/find-out-which-version-of-microsoft-edge-you-have-c726bee8-c42e-e472-e954-4cf5123497eb).</span><span class="sxs-lookup"><span data-stu-id="8e3f5-115">To find out the latest version, see [Find out which version of Microsoft Edge you have](https://support.microsoft.com/microsoft-edge/find-out-which-version-of-microsoft-edge-you-have-c726bee8-c42e-e472-e954-4cf5123497eb).</span></span>
- <span data-ttu-id="8e3f5-116">Mulai ulang browser Edge.</span><span class="sxs-lookup"><span data-stu-id="8e3f5-116">Restart the Edge browser.</span></span>
- <span data-ttu-id="8e3f5-117">Navigasikan ke situs di mana Anda telah menyiapkan indikator.</span><span class="sxs-lookup"><span data-stu-id="8e3f5-117">Navigate to the site for which you have setup an indicator.</span></span> <span data-ttu-id="8e3f5-118">Jika situs tidak muncul seperti yang diharapkan, lanjutkan ke Langkah 3.</span><span class="sxs-lookup"><span data-stu-id="8e3f5-118">If the site does not appear as expected, continue to Step 3.</span></span> 

## <a name="step-3-collect-data"></a><span data-ttu-id="8e3f5-119">Langkah 3: Kumpulkan data</span><span class="sxs-lookup"><span data-stu-id="8e3f5-119">Step 3: Collect data</span></span>

- <span data-ttu-id="8e3f5-120">Kumpulkan data **diagnostik MDEClientAnalyzer.**</span><span class="sxs-lookup"><span data-stu-id="8e3f5-120">Collect **MDEClientAnalyzer** diagnostic data.</span></span> <span data-ttu-id="8e3f5-121">Untuk instruksinya, [lihat Masalah dengan mesin onboarding ke Pertahanan Microsoft untuk Titik Akhir](issues-with-onboarding-machines.md).</span><span class="sxs-lookup"><span data-stu-id="8e3f5-121">For instructions, see [Issues with onboarding machines to Microsoft Defender for Endpoint](issues-with-onboarding-machines.md).</span></span>
- <span data-ttu-id="8e3f5-122">Jika Anda telah nyaman menginstal dan mengumpulkan jejak Fiddler, lihat [Telerik Fiddler](http://www.telerik.com/fiddler).</span><span class="sxs-lookup"><span data-stu-id="8e3f5-122">If you are comfortable installing and collecting a Fiddler trace, see [Telerik Fiddler](http://www.telerik.com/fiddler).</span></span>
- <span data-ttu-id="8e3f5-123">Jika Anda lebih memilih panduan dari Dukungan Microsoft, pilih ikon Dukungan di bawah ini untuk membuka kasus dukungan.</span><span class="sxs-lookup"><span data-stu-id="8e3f5-123">If you prefer guidance from Microsoft Support, select the Support icon below to open a support case.</span></span>
