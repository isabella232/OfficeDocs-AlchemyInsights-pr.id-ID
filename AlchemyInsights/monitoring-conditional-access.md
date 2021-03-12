---
title: Memantau akses bersyarat
ms.author: pebaum
author: pebaum
ms.date: 04/21/2020
ms.audience: ITPro
ms.topic: article
ms.service: o365-administration
ROBOTS: NOINDEX, NOFOLLOW
localization_priority: Normal
ms.custom:
- "9003769"
- "6702"
ms.openlocfilehash: c3bf5dd9066685af2df7ba50f0eb3ba6e891c2a9
ms.sourcegitcommit: 0eb4f9bde53395b5fd4b5cd4ffc56ca96db91298
ms.translationtype: MT
ms.contentlocale: id-ID
ms.lasthandoff: 03/10/2021
ms.locfileid: "50708677"
---
# <a name="monitoring-conditional-access-for-exchange"></a><span data-ttu-id="b5296-102">Memantau akses bersyarat untuk Exchange</span><span class="sxs-lookup"><span data-stu-id="b5296-102">Monitoring Conditional Access for Exchange</span></span>

<span data-ttu-id="b5296-103">Pengguna yang ditargetkan dengan akses bersyarat akan menerima email pemberitahuan jika mereka tidak memenuhi persyaratan akses organisasi Anda.</span><span class="sxs-lookup"><span data-stu-id="b5296-103">Users targeted with conditional access will receive a notification email if they do not meet your organization's access requirements.</span></span> <span data-ttu-id="b5296-104">Untuk mengatasinya, kami menyarankan satu atau beberapa solusi berikut:</span><span class="sxs-lookup"><span data-stu-id="b5296-104">To resolve, we recommend one or more of the following solutions:</span></span>

- <span data-ttu-id="b5296-105">Jika perangkat dianggap terdaftar, Anjurkan pengguna untuk masuk ke aplikasi portal perusahaan dan memverifikasi bahwa perangkat tersebut muncul di portal perusahaan.</span><span class="sxs-lookup"><span data-stu-id="b5296-105">If the device is presumed to be enrolled, advise the user to go to the Company Portal app and verify that it appears in the Company Portal.</span></span> <span data-ttu-id="b5296-106">Jika tidak, pengguna harus mendaftarkan perangkat.</span><span class="sxs-lookup"><span data-stu-id="b5296-106">If it doesn't, the user should enroll the device.</span></span>
- <span data-ttu-id="b5296-107">Di portal Azure, masuk ke Intune > kepatuhan perangkat.</span><span class="sxs-lookup"><span data-stu-id="b5296-107">In the Azure portal go to Intune > Device compliance.</span></span> <span data-ttu-id="b5296-108">Di bawah monitor klik kepatuhan perangkat.</span><span class="sxs-lookup"><span data-stu-id="b5296-108">Under Monitor click Device compliance.</span></span> <span data-ttu-id="b5296-109">Tampilkan Laporan kepatuhan perangkat Anda untuk memverifikasi bahwa perangkat pengguna ditandai sebagai sesuai.</span><span class="sxs-lookup"><span data-stu-id="b5296-109">View your device compliance report to verify that the user's device is marked as compliant.</span></span>
- <span data-ttu-id="b5296-110">Di portal Azure, masuk ke Intune > kepatuhan perangkat.</span><span class="sxs-lookup"><span data-stu-id="b5296-110">In the Azure portal go to Intune > Device compliance.</span></span> <span data-ttu-id="b5296-111">Di bawah Kelola, klik kebijakan.</span><span class="sxs-lookup"><span data-stu-id="b5296-111">Under Manage, click Policies.</span></span> <span data-ttu-id="b5296-112">Dalam daftar kebijakan kepatuhan, verifikasi bahwa profil ditetapkan untuk perangkat pengguna Anda.</span><span class="sxs-lookup"><span data-stu-id="b5296-112">In the list of compliance policies, verify that a profile is assigned to your user's device.</span></span> <span data-ttu-id="b5296-113">Jika tidak ada profil yang ditetapkan, maka Intune tidak akan dapat mengonfirmasi status kepatuhan perangkat.</span><span class="sxs-lookup"><span data-stu-id="b5296-113">If no profile is assigned, then Intune will not be able to confirm the device's compliance status.</span></span>
- <span data-ttu-id="b5296-114">Mengedit penetapan akses bersyarat pengguna.</span><span class="sxs-lookup"><span data-stu-id="b5296-114">Edit the user's conditional access assignment.</span></span>

1. <span data-ttu-id="b5296-115">Di portal Azure, masuk ke   >  **kebijakan akses bersyarat** Intune  >  .</span><span class="sxs-lookup"><span data-stu-id="b5296-115">In the Azure portal go to **Intune** > **Conditional access** > **Policies**.</span></span>
2. <span data-ttu-id="b5296-116">Pilih kebijakan dari daftar.</span><span class="sxs-lookup"><span data-stu-id="b5296-116">Select a policy from the list.</span></span>
3. <span data-ttu-id="b5296-117">Klik pengguna dan grup.</span><span class="sxs-lookup"><span data-stu-id="b5296-117">Click Users and groups.</span></span>
4. <span data-ttu-id="b5296-118">Untuk menargetkan kebijakan tertentu pada seseorang, tambahkan ke daftar sertakan.</span><span class="sxs-lookup"><span data-stu-id="b5296-118">To target a certain policy at someone, add them to the Include list.</span></span> <span data-ttu-id="b5296-119">Untuk memastikan bahwa seseorang dihilangkan dari kebijakan, tambahkan ke daftar Kecualikan.</span><span class="sxs-lookup"><span data-stu-id="b5296-119">To ensure that a person is omitted from the policy, add them to the Exclude list.</span></span>

<span data-ttu-id="b5296-120">Link yang berguna:</span><span class="sxs-lookup"><span data-stu-id="b5296-120">Helpful links:</span></span>

[<span data-ttu-id="b5296-121">Gambaran umum kepatuhan perangkat</span><span class="sxs-lookup"><span data-stu-id="b5296-121">Device compliance overview</span></span>](https://docs.microsoft.com/intune/device-compliance-get-started)

[<span data-ttu-id="b5296-122">Pemecahan masalah CA</span><span class="sxs-lookup"><span data-stu-id="b5296-122">Troubleshooting CA</span></span>](https://docs.microsoft.com/intune/troubleshoot-conditional-access)

[<span data-ttu-id="b5296-123">Kebijakan pemecahan masalah</span><span class="sxs-lookup"><span data-stu-id="b5296-123">Troubleshooting policy</span></span>](https://docs.microsoft.com/troubleshoot/mem/intune/troubleshoot-policies-in-microsoft-intune)

[<span data-ttu-id="b5296-124">Monitoring Intune Device Compliance</span><span class="sxs-lookup"><span data-stu-id="b5296-124">Monitoring Intune device compliance</span></span>](https://docs.microsoft.com/intune/compliance-policy-monitor)

<span data-ttu-id="b5296-125">Catatan: langkah-langkah ini hanya membantu dalam pemecahan masalah akses bersyarat fitur direktori aktif Azure.</span><span class="sxs-lookup"><span data-stu-id="b5296-125">Note: these steps are only helpful in troubleshooting the Azure Active Directory feature Conditional Access.</span></span> <span data-ttu-id="b5296-126">Memungkinkan untuk mengkarantina perangkat yang memblokir akses email itu dengan kebijakan Exchange.</span><span class="sxs-lookup"><span data-stu-id="b5296-126">It is also possible to quarantine a device blocking it's email access with Exchange policy.</span></span> <span data-ttu-id="b5296-127">Informasi selengkapnya tentang manajemen perangkat Exchange bisa ditemukan [di sini] ( https://docs.microsoft.com/previous-versions/office/exchange-server-2010/ff959225(v=exchg.141) .</span><span class="sxs-lookup"><span data-stu-id="b5296-127">More information on Exchange device management can be found [here](https://docs.microsoft.com/previous-versions/office/exchange-server-2010/ff959225(v=exchg.141).</span></span>
