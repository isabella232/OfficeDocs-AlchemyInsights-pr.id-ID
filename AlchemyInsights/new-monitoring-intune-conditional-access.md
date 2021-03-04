---
title: Memantau akses bersyarat Intune
ms.author: v-aiyengar
author: AshaIyengar21
manager: dansimp
ms.date: 02/25/2021
ms.audience: Admin
ms.topic: article
ms.service: o365-administration
ROBOTS: NOINDEX, NOFOLLOW
localization_priority: Normal
ms.collection: Adm_O365
ms.custom:
- "9004636"
- "8386"
ms.openlocfilehash: e2803a49aaf087ac55b1fd62056e2b0af3fcd919
ms.sourcegitcommit: 229bd519ec1c14c65a243226a94eee23e117a7fc
ms.translationtype: MT
ms.contentlocale: id-ID
ms.lasthandoff: 03/03/2021
ms.locfileid: "50427921"
---
# <a name="monitor-intune-conditional-access"></a><span data-ttu-id="7efc0-102">Memantau akses bersyarat Intune</span><span class="sxs-lookup"><span data-stu-id="7efc0-102">Monitor Intune Conditional Access</span></span>

<span data-ttu-id="7efc0-103">Pengguna yang ditargetkan dengan akses bersyarat akan menerima email pemberitahuan jika mereka tidak memenuhi persyaratan akses organisasi Anda.</span><span class="sxs-lookup"><span data-stu-id="7efc0-103">Users targeted with conditional access will receive a notification email if they do not meet your organization's access requirements.</span></span> <span data-ttu-id="7efc0-104">Untuk mengatasinya, kami menyarankan satu atau beberapa solusi berikut:</span><span class="sxs-lookup"><span data-stu-id="7efc0-104">To resolve, we recommend one or more of the following solutions:</span></span>

1. <span data-ttu-id="7efc0-105">Jika perangkat dianggap terdaftar, Anjurkan pengguna untuk masuk ke aplikasi portal perusahaan dan memverifikasi bahwa perangkat tersebut muncul di portal perusahaan.</span><span class="sxs-lookup"><span data-stu-id="7efc0-105">If the device is presumed to be enrolled, advise the user to go to the Company Portal app and verify that it appears in the Company Portal.</span></span> <span data-ttu-id="7efc0-106">Jika tidak, pengguna harus mendaftarkan perangkat.</span><span class="sxs-lookup"><span data-stu-id="7efc0-106">If it doesn't, the user must enroll the device.</span></span>
1. <span data-ttu-id="7efc0-107">Di portal Azure, masuk ke **Intune**  >  **Device Compliance**.</span><span class="sxs-lookup"><span data-stu-id="7efc0-107">In the Azure portal go to **Intune** > **Device compliance**.</span></span> 
1. <span data-ttu-id="7efc0-108">Untuk menampilkan laporan kepatuhan perangkat untuk memverifikasi bahwa perangkat pengguna ditandai sebagai sesuai, di bawah **monitor**, klik **kepatuhan perangkat**.</span><span class="sxs-lookup"><span data-stu-id="7efc0-108">To view your device compliance report to verify that the user's device is marked as compliant, under **Monitor**, click **Device compliance**.</span></span>
1. <span data-ttu-id="7efc0-109">Di portal Azure, masuk ke **Intune**  >  **Device Compliance**.</span><span class="sxs-lookup"><span data-stu-id="7efc0-109">In the Azure portal go to **Intune** > **Device compliance**.</span></span> <span data-ttu-id="7efc0-110">Di bawah **Kelola,** klik **kebijakan**.</span><span class="sxs-lookup"><span data-stu-id="7efc0-110">Under **Manage,** click **Policies**.</span></span> <span data-ttu-id="7efc0-111">Dalam daftar kebijakan kepatuhan, verifikasi bahwa profil ditetapkan untuk perangkat pengguna Anda.</span><span class="sxs-lookup"><span data-stu-id="7efc0-111">In the list of compliance policies, verify that a profile is assigned to your user's device.</span></span> <span data-ttu-id="7efc0-112">Jika tidak ada profil yang ditetapkan, maka Intune tidak akan dapat mengonfirmasi status kepatuhan perangkat.</span><span class="sxs-lookup"><span data-stu-id="7efc0-112">If no profile is assigned, then Intune will not be able to confirm the device's compliance status.</span></span>
1. <span data-ttu-id="7efc0-113">Mengedit penetapan akses bersyarat pengguna.</span><span class="sxs-lookup"><span data-stu-id="7efc0-113">Edit the user's conditional access assignment.</span></span>
1. <span data-ttu-id="7efc0-114">Di portal Azure, navigasikan ke   >  **kebijakan akses bersyarat** Intune  >  , pilih kebijakan dari daftar, dan klik **pengguna dan grup**.</span><span class="sxs-lookup"><span data-stu-id="7efc0-114">In the Azure portal, navigate to **Intune** > **Conditional access** > **Policies**, select a policy from the list, and click **Users and groups**.</span></span>
1. <span data-ttu-id="7efc0-115">Untuk menargetkan kebijakan tertentu pada seseorang, tambahkan ke **Daftar sertakan**.</span><span class="sxs-lookup"><span data-stu-id="7efc0-115">To target a certain policy at someone, add them to the **Include list**.</span></span> <span data-ttu-id="7efc0-116">Untuk memastikan bahwa seseorang dihilangkan dari kebijakan, tambahkan ke **Daftar Kecualikan**.</span><span class="sxs-lookup"><span data-stu-id="7efc0-116">To ensure that a person is omitted from the policy, add them to the **Exclude list**.</span></span>

<span data-ttu-id="7efc0-117">**Link yang berguna:**</span><span class="sxs-lookup"><span data-stu-id="7efc0-117">**Helpful links:**</span></span>

- [<span data-ttu-id="7efc0-118">Gambaran umum kepatuhan perangkat</span><span class="sxs-lookup"><span data-stu-id="7efc0-118">Device compliance overview</span></span>](https://docs.microsoft.com/intune/device-compliance-get-started)
- [<span data-ttu-id="7efc0-119">Pemecahan masalah CA</span><span class="sxs-lookup"><span data-stu-id="7efc0-119">Troubleshooting CA</span></span>](https://docs.microsoft.com/intune/troubleshoot-conditional-access)
- [<span data-ttu-id="7efc0-120">Kebijakan pemecahan masalah</span><span class="sxs-lookup"><span data-stu-id="7efc0-120">Troubleshooting policy</span></span>](https://docs.microsoft.com/intune/troubleshoot-policies-in-microsoft-intune)
- [<span data-ttu-id="7efc0-121">Monitoring Intune Device Compliance</span><span class="sxs-lookup"><span data-stu-id="7efc0-121">Monitoring Intune device compliance</span></span>](https://docs.microsoft.com/intune/compliance-policy-monitor)

> [!NOTE]
> <span data-ttu-id="7efc0-122">Langkah-langkah ini hanya membantu dalam pemecahan masalah akses bersyarat fitur direktori aktif Azure.</span><span class="sxs-lookup"><span data-stu-id="7efc0-122">These steps are only helpful in troubleshooting the Azure Active Directory feature Conditional Access.</span></span> <span data-ttu-id="7efc0-123">Memungkinkan untuk mengkarantina perangkat yang memblokir akses email itu dengan kebijakan Exchange.</span><span class="sxs-lookup"><span data-stu-id="7efc0-123">It is also possible to quarantine a device blocking it's email access with Exchange policy.</span></span> <span data-ttu-id="7efc0-124">Informasi selengkapnya tentang manajemen perangkat Exchange bisa ditemukan [**di sini**](https://docs.microsoft.com/previous-versions/office/exchange-server-2010/ff959225(v=exchg.141)).</span><span class="sxs-lookup"><span data-stu-id="7efc0-124">More information on Exchange device management can be found [**here**](https://docs.microsoft.com/previous-versions/office/exchange-server-2010/ff959225(v=exchg.141)).</span></span>
