---
title: Pemantauan akses bersyarat
ms.author: pebaum
author: pebaum
ms.date: 8/1/2018
ms.audience: ITPro
ms.topic: article
ROBOTS: NOINDEX, NOFOLLOW
localization_priority: Priority
ms.assetid: dcb86c54-769e-4832-9f88-bc45f1e5f36c
ms.openlocfilehash: f4153f8a87a138d548c133142b0d48a319bd4b71
ms.sourcegitcommit: 0ae6cbb8cf2836da98300767ed81b411d6551bee
ms.translationtype: MT
ms.contentlocale: id-ID
ms.lasthandoff: 01/30/2019
ms.locfileid: "29656570"
---
# <a name="monitoring-conditional-access"></a><span data-ttu-id="87aa0-102">Pemantauan akses bersyarat</span><span class="sxs-lookup"><span data-stu-id="87aa0-102">Monitoring Conditional Access</span></span>

<span data-ttu-id="87aa0-p101">Pengguna dengan akses bersyarat yang ditargetkan akan menerima email pemberitahuan jika mereka tidak memenuhi persyaratan akses organisasi Anda. Untuk menyelesaikan, kami merekomendasikan satu atau lebih solusi berikut:</span><span class="sxs-lookup"><span data-stu-id="87aa0-p101">Users targeted with conditional access will receive a notification email if they do not meet your organization's access requirements. To resolve, we recommend one or more of the following solutions:</span></span>
  
- <span data-ttu-id="87aa0-p102">Jika perangkat dianggap diterima, menyarankan pengguna untuk pergi ke app Portal perusahaan dan memverifikasi bahwa itu muncul di Portal perusahaan. Jika tidak, pengguna harus mendaftarkan perangkat.</span><span class="sxs-lookup"><span data-stu-id="87aa0-p102">If the device is presumed to be enrolled, advise the user to go to the Company Portal app and verify that it appears in the Company Portal. If it doesn't, the user should enroll the device.</span></span>
    
- <span data-ttu-id="87aa0-p103">Di Azure portal pergi ke **Intune \> kepatuhan perangkat**. Di bawah **Monitor** klik **perangkat kepatuhan**. Lihat laporan kepatuhan perangkat Anda untuk memverifikasi bahwa perangkat pengguna ditandai sebagai compliant.</span><span class="sxs-lookup"><span data-stu-id="87aa0-p103">In the Azure portal go to **Intune \> Device compliance**. Under **Monitor** click **Device compliance**. View your device compliance report to verify that the user's device is marked as compliant.</span></span> 
    
- <span data-ttu-id="87aa0-p104">Di Azure portal pergi ke **Intune \> kepatuhan perangkat**. Dalam **mengelola**, klik **kebijakan**. Dalam daftar kebijakan kepatuhan, pastikan bahwa profil yang ditetapkan ke perangkat pengguna Anda. Jika profil tidak ditetapkan, maka Intune tidak akan bisa mengkonfirmasi perangkat kepatuhan status.</span><span class="sxs-lookup"><span data-stu-id="87aa0-p104">In the Azure portal go to **Intune \> Device compliance**. Under **Manage**, click **Policies**. In the list of compliance policies, verify that a profile is assigned to your user's device. If no profile is assigned, then Intune will not be able to confirm the device's compliance status.</span></span> 
    
- <span data-ttu-id="87aa0-114">Mengedit tugas bersyarat akses pengguna.</span><span class="sxs-lookup"><span data-stu-id="87aa0-114">Edit the user's conditional access assignment.</span></span>
    
1. <span data-ttu-id="87aa0-115">Di Azure portal pergi ke **Intune \> akses bersyarat \> kebijakan**</span><span class="sxs-lookup"><span data-stu-id="87aa0-115">In the Azure portal go to **Intune \> Conditional access \> Policies**</span></span>
    
2. <span data-ttu-id="87aa0-116">Pilih kebijakan dari daftar</span><span class="sxs-lookup"><span data-stu-id="87aa0-116">Select a policy from the list</span></span>
    
3. <span data-ttu-id="87aa0-117">Klik **pengguna dan grup**</span><span class="sxs-lookup"><span data-stu-id="87aa0-117">Click **Users and groups**</span></span>
    
4. <span data-ttu-id="87aa0-p105">Untuk menargetkan kebijakan tertentu pada seseorang, menambahkan mereka ke daftar **termasuk** . Untuk memastikan bahwa orang yang dihilangkan dari kebijakan, menambahkannya ke **mengecualikan** daftar.</span><span class="sxs-lookup"><span data-stu-id="87aa0-p105">To target a certain policy at someone, add them to the **Include** list. To ensure that a person is omitted from the policy, add them to the **Exclude** list.</span></span> 
    
<span data-ttu-id="87aa0-120">Baca lebih lanjut: [bagaimana perangkat akses bersyarat Monitor](https://docs.microsoft.com/intune/conditional-access-exchange-monitor)</span><span class="sxs-lookup"><span data-stu-id="87aa0-120">Read more: [How to Monitor Conditional Access devices](https://docs.microsoft.com/intune/conditional-access-exchange-monitor)</span></span>
  

