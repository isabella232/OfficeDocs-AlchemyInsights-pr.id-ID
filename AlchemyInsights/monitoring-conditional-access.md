---
title: Pemantauan akses bersyarat
ms.author: pebaum
author: pebaum
ms.date: 04/21/2020
ms.audience: ITPro
ms.topic: article
ROBOTS: NOINDEX, NOFOLLOW
localization_priority: Normal
ms.assetid: dcb86c54-769e-4832-9f88-bc45f1e5f36c
ms.openlocfilehash: 8b76d58791408037b5704b421d7afa166e3ea0be
ms.sourcegitcommit: 55eff703a17e500681d8fa6a87eb067019ade3cc
ms.translationtype: MT
ms.contentlocale: id-ID
ms.lasthandoff: 04/22/2020
ms.locfileid: "43713721"
---
# <a name="monitoring-conditional-access-for-exchange"></a><span data-ttu-id="6f5f6-102">Pemantauan akses bersyarat untuk Exchange</span><span class="sxs-lookup"><span data-stu-id="6f5f6-102">Monitoring Conditional Access for Exchange</span></span>

<span data-ttu-id="6f5f6-103">Pengguna yang ditargetkan dengan akses bersyarat akan menerima email pemberitahuan jika mereka tidak memenuhi persyaratan akses organisasi Anda.</span><span class="sxs-lookup"><span data-stu-id="6f5f6-103">Users targeted with conditional access will receive a notification email if they do not meet your organization's access requirements.</span></span> <span data-ttu-id="6f5f6-104">Untuk menyelesaikan, kami merekomendasikan satu atau lebih solusi berikut:</span><span class="sxs-lookup"><span data-stu-id="6f5f6-104">To resolve, we recommend one or more of the following solutions:</span></span>
  
- <span data-ttu-id="6f5f6-105">Jika perangkat diduga terdaftar, menyarankan pengguna untuk pergi ke aplikasi portal perusahaan dan verifikasi bahwa ditampilkan di portal perusahaan.</span><span class="sxs-lookup"><span data-stu-id="6f5f6-105">If the device is presumed to be enrolled, advise the user to go to the Company Portal app and verify that it appears in the Company Portal.</span></span> <span data-ttu-id="6f5f6-106">Jika tidak, pengguna harus mendaftarkan perangkat.</span><span class="sxs-lookup"><span data-stu-id="6f5f6-106">If it doesn't, the user should enroll the device.</span></span>
    
- <span data-ttu-id="6f5f6-107">Di portal Azure pergi ke \*\* \> Intune kepatuhan perangkat\*\*.</span><span class="sxs-lookup"><span data-stu-id="6f5f6-107">In the Azure portal go to **Intune \> Device compliance**.</span></span> <span data-ttu-id="6f5f6-108">Di bawah **monitor** , klik **perangkat kepatuhan**.</span><span class="sxs-lookup"><span data-stu-id="6f5f6-108">Under **Monitor** click **Device compliance**.</span></span> <span data-ttu-id="6f5f6-109">Lihat laporan kepatuhan perangkat untuk memverifikasi bahwa perangkat pengguna ditandai sebagai sesuai.</span><span class="sxs-lookup"><span data-stu-id="6f5f6-109">View your device compliance report to verify that the user's device is marked as compliant.</span></span> 
    
- <span data-ttu-id="6f5f6-110">Di portal Azure pergi ke \*\* \> Intune kepatuhan perangkat\*\*.</span><span class="sxs-lookup"><span data-stu-id="6f5f6-110">In the Azure portal go to **Intune \> Device compliance**.</span></span> <span data-ttu-id="6f5f6-111">Di bawah **Kelola**, klik **kebijakan**.</span><span class="sxs-lookup"><span data-stu-id="6f5f6-111">Under **Manage**, click **Policies**.</span></span> <span data-ttu-id="6f5f6-112">Dalam daftar kebijakan kepatuhan, Verifikasikan bahwa profil ditetapkan ke perangkat pengguna Anda.</span><span class="sxs-lookup"><span data-stu-id="6f5f6-112">In the list of compliance policies, verify that a profile is assigned to your user's device.</span></span> <span data-ttu-id="6f5f6-113">Jika tidak ada profil yang ditetapkan, maka Intune tidak akan dapat mengkonfirmasi status kepatuhan perangkat.</span><span class="sxs-lookup"><span data-stu-id="6f5f6-113">If no profile is assigned, then Intune will not be able to confirm the device's compliance status.</span></span> 
    
- <span data-ttu-id="6f5f6-114">Mengedit penetapan akses bersyarat pengguna.</span><span class="sxs-lookup"><span data-stu-id="6f5f6-114">Edit the user's conditional access assignment.</span></span>
    
1. <span data-ttu-id="6f5f6-115">Di portal Azure pergi ke **Intune \> kebijakan akses \> bersyarat**</span><span class="sxs-lookup"><span data-stu-id="6f5f6-115">In the Azure portal go to **Intune \> Conditional access \> Policies**</span></span>
    
2. <span data-ttu-id="6f5f6-116">Pilih kebijakan dari daftar</span><span class="sxs-lookup"><span data-stu-id="6f5f6-116">Select a policy from the list</span></span>
    
3. <span data-ttu-id="6f5f6-117">Klik **pengguna dan grup**</span><span class="sxs-lookup"><span data-stu-id="6f5f6-117">Click **Users and groups**</span></span>
    
4. <span data-ttu-id="6f5f6-118">Untuk menargetkan kebijakan tertentu pada seseorang, menambahkannya ke daftar **sertakan** .</span><span class="sxs-lookup"><span data-stu-id="6f5f6-118">To target a certain policy at someone, add them to the **Include** list.</span></span> <span data-ttu-id="6f5f6-119">Untuk memastikan seseorang diabaikan dari kebijakan, tambahkan ke daftar **Kecualikan** .</span><span class="sxs-lookup"><span data-stu-id="6f5f6-119">To ensure that a person is omitted from the policy, add them to the **Exclude** list.</span></span> 
    
<span data-ttu-id="6f5f6-120">Baca lebih lanjut: [Bagaimana memonitor perangkat akses bersyarat](https://docs.microsoft.com/intune/conditional-access-exchange-monitor)</span><span class="sxs-lookup"><span data-stu-id="6f5f6-120">Read more: [How to Monitor Conditional Access devices](https://docs.microsoft.com/intune/conditional-access-exchange-monitor)</span></span>
  

