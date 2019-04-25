---
title: Pemantauan akses bersyarat
ms.author: pebaum
author: pebaum
ms.date: 8/1/2018
ms.audience: ITPro
ms.topic: article
ROBOTS: NOINDEX, NOFOLLOW
localization_priority: Normal
ms.assetid: dcb86c54-769e-4832-9f88-bc45f1e5f36c
ms.openlocfilehash: 756c5e98ed3e9cedd0152b5747ea6bf1ed31778e
ms.sourcegitcommit: 9d78905c512192ffc4675468abd2efc5f2e4baf4
ms.translationtype: MT
ms.contentlocale: id-ID
ms.lasthandoff: 04/23/2019
ms.locfileid: "32418472"
---
# <a name="monitoring-conditional-access"></a><span data-ttu-id="270da-102">Pemantauan akses bersyarat</span><span class="sxs-lookup"><span data-stu-id="270da-102">Monitoring Conditional Access</span></span>

<span data-ttu-id="270da-103">Pengguna dengan akses bersyarat yang ditargetkan akan menerima email pemberitahuan jika mereka tidak memenuhi persyaratan akses organisasi Anda.</span><span class="sxs-lookup"><span data-stu-id="270da-103">Users targeted with conditional access will receive a notification email if they do not meet your organization's access requirements.</span></span> <span data-ttu-id="270da-104">Untuk menyelesaikan, kami merekomendasikan satu atau lebih solusi berikut:</span><span class="sxs-lookup"><span data-stu-id="270da-104">To resolve, we recommend one or more of the following solutions:</span></span>
  
- <span data-ttu-id="270da-105">Jika perangkat dianggap diterima, menyarankan pengguna untuk pergi ke app Portal perusahaan dan memverifikasi bahwa itu muncul di Portal perusahaan.</span><span class="sxs-lookup"><span data-stu-id="270da-105">If the device is presumed to be enrolled, advise the user to go to the Company Portal app and verify that it appears in the Company Portal.</span></span> <span data-ttu-id="270da-106">Jika tidak, pengguna harus mendaftarkan perangkat.</span><span class="sxs-lookup"><span data-stu-id="270da-106">If it doesn't, the user should enroll the device.</span></span>
    
- <span data-ttu-id="270da-107">Di Azure portal pergi ke **Intune \> kepatuhan perangkat**.</span><span class="sxs-lookup"><span data-stu-id="270da-107">In the Azure portal go to **Intune \> Device compliance**.</span></span> <span data-ttu-id="270da-108">Di bawah **Monitor** klik **perangkat kepatuhan**.</span><span class="sxs-lookup"><span data-stu-id="270da-108">Under **Monitor** click **Device compliance**.</span></span> <span data-ttu-id="270da-109">Lihat laporan kepatuhan perangkat Anda untuk memverifikasi bahwa perangkat pengguna ditandai sebagai compliant.</span><span class="sxs-lookup"><span data-stu-id="270da-109">View your device compliance report to verify that the user's device is marked as compliant.</span></span> 
    
- <span data-ttu-id="270da-110">Di Azure portal pergi ke **Intune \> kepatuhan perangkat**.</span><span class="sxs-lookup"><span data-stu-id="270da-110">In the Azure portal go to **Intune \> Device compliance**.</span></span> <span data-ttu-id="270da-111">Dalam **mengelola**, klik **kebijakan**.</span><span class="sxs-lookup"><span data-stu-id="270da-111">Under **Manage**, click **Policies**.</span></span> <span data-ttu-id="270da-112">Dalam daftar kebijakan kepatuhan, pastikan bahwa profil yang ditetapkan ke perangkat pengguna Anda.</span><span class="sxs-lookup"><span data-stu-id="270da-112">In the list of compliance policies, verify that a profile is assigned to your user's device.</span></span> <span data-ttu-id="270da-113">Jika profil tidak ditetapkan, maka Intune tidak akan bisa mengkonfirmasi perangkat kepatuhan status.</span><span class="sxs-lookup"><span data-stu-id="270da-113">If no profile is assigned, then Intune will not be able to confirm the device's compliance status.</span></span> 
    
- <span data-ttu-id="270da-114">Mengedit tugas bersyarat akses pengguna.</span><span class="sxs-lookup"><span data-stu-id="270da-114">Edit the user's conditional access assignment.</span></span>
    
1. <span data-ttu-id="270da-115">Di Azure portal pergi ke **Intune \> akses bersyarat \> kebijakan**</span><span class="sxs-lookup"><span data-stu-id="270da-115">In the Azure portal go to **Intune \> Conditional access \> Policies**</span></span>
    
2. <span data-ttu-id="270da-116">Pilih kebijakan dari daftar</span><span class="sxs-lookup"><span data-stu-id="270da-116">Select a policy from the list</span></span>
    
3. <span data-ttu-id="270da-117">Klik **pengguna dan grup**</span><span class="sxs-lookup"><span data-stu-id="270da-117">Click **Users and groups**</span></span>
    
4. <span data-ttu-id="270da-118">Untuk menargetkan kebijakan tertentu pada seseorang, menambahkan mereka ke daftar **termasuk** .</span><span class="sxs-lookup"><span data-stu-id="270da-118">To target a certain policy at someone, add them to the **Include** list.</span></span> <span data-ttu-id="270da-119">Untuk memastikan bahwa orang yang dihilangkan dari kebijakan, menambahkannya ke **mengecualikan** daftar.</span><span class="sxs-lookup"><span data-stu-id="270da-119">To ensure that a person is omitted from the policy, add them to the **Exclude** list.</span></span> 
    
<span data-ttu-id="270da-120">Baca lebih lanjut: [bagaimana perangkat akses bersyarat Monitor](https://docs.microsoft.com/intune/conditional-access-exchange-monitor)</span><span class="sxs-lookup"><span data-stu-id="270da-120">Read more: [How to Monitor Conditional Access devices](https://docs.microsoft.com/intune/conditional-access-exchange-monitor)</span></span>
  

