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
ms.assetid: dcb86c54-769e-4832-9f88-bc45f1e5f36c
ms.openlocfilehash: 6083fc427e3791fdb0907198b525337a0c987c4e
ms.sourcegitcommit: c6692ce0fa1358ec3529e59ca0ecdfdea4cdc759
ms.translationtype: MT
ms.contentlocale: id-ID
ms.lasthandoff: 09/14/2020
ms.locfileid: "47702906"
---
# <a name="monitoring-conditional-access-for-exchange"></a><span data-ttu-id="7ae06-102">Memantau akses bersyarat untuk Exchange</span><span class="sxs-lookup"><span data-stu-id="7ae06-102">Monitoring Conditional Access for Exchange</span></span>

<span data-ttu-id="7ae06-103">Pengguna yang ditargetkan dengan akses bersyarat akan menerima email pemberitahuan jika mereka tidak memenuhi persyaratan akses organisasi Anda.</span><span class="sxs-lookup"><span data-stu-id="7ae06-103">Users targeted with conditional access will receive a notification email if they do not meet your organization's access requirements.</span></span> <span data-ttu-id="7ae06-104">Untuk mengatasinya, kami menyarankan satu atau beberapa solusi berikut:</span><span class="sxs-lookup"><span data-stu-id="7ae06-104">To resolve, we recommend one or more of the following solutions:</span></span>
  
- <span data-ttu-id="7ae06-105">Jika perangkat dianggap terdaftar, Anjurkan pengguna untuk masuk ke aplikasi portal perusahaan dan memverifikasi bahwa perangkat tersebut muncul di portal perusahaan.</span><span class="sxs-lookup"><span data-stu-id="7ae06-105">If the device is presumed to be enrolled, advise the user to go to the Company Portal app and verify that it appears in the Company Portal.</span></span> <span data-ttu-id="7ae06-106">Jika tidak, pengguna harus mendaftarkan perangkat.</span><span class="sxs-lookup"><span data-stu-id="7ae06-106">If it doesn't, the user should enroll the device.</span></span>
    
- <span data-ttu-id="7ae06-107">Di portal Azure, masuk ke **Intune \> Device Compliance**.</span><span class="sxs-lookup"><span data-stu-id="7ae06-107">In the Azure portal go to **Intune \> Device compliance**.</span></span> <span data-ttu-id="7ae06-108">Di bawah **monitor** klik **kepatuhan perangkat**.</span><span class="sxs-lookup"><span data-stu-id="7ae06-108">Under **Monitor** click **Device compliance**.</span></span> <span data-ttu-id="7ae06-109">Tampilkan Laporan kepatuhan perangkat Anda untuk memverifikasi bahwa perangkat pengguna ditandai sebagai sesuai.</span><span class="sxs-lookup"><span data-stu-id="7ae06-109">View your device compliance report to verify that the user's device is marked as compliant.</span></span> 
    
- <span data-ttu-id="7ae06-110">Di portal Azure, masuk ke **Intune \> Device Compliance**.</span><span class="sxs-lookup"><span data-stu-id="7ae06-110">In the Azure portal go to **Intune \> Device compliance**.</span></span> <span data-ttu-id="7ae06-111">Di bawah **Kelola**, klik **kebijakan**.</span><span class="sxs-lookup"><span data-stu-id="7ae06-111">Under **Manage**, click **Policies**.</span></span> <span data-ttu-id="7ae06-112">Dalam daftar kebijakan kepatuhan, verifikasi bahwa profil ditetapkan untuk perangkat pengguna Anda.</span><span class="sxs-lookup"><span data-stu-id="7ae06-112">In the list of compliance policies, verify that a profile is assigned to your user's device.</span></span> <span data-ttu-id="7ae06-113">Jika tidak ada profil yang ditetapkan, maka Intune tidak akan dapat mengonfirmasi status kepatuhan perangkat.</span><span class="sxs-lookup"><span data-stu-id="7ae06-113">If no profile is assigned, then Intune will not be able to confirm the device's compliance status.</span></span> 
    
- <span data-ttu-id="7ae06-114">Mengedit penetapan akses bersyarat pengguna.</span><span class="sxs-lookup"><span data-stu-id="7ae06-114">Edit the user's conditional access assignment.</span></span>
    
1. <span data-ttu-id="7ae06-115">Di Azure portal masuk ke \*\* \> \> kebijakan akses bersyarat Intune\*\*</span><span class="sxs-lookup"><span data-stu-id="7ae06-115">In the Azure portal go to **Intune \> Conditional access \> Policies**</span></span>
    
2. <span data-ttu-id="7ae06-116">Memilih kebijakan dari daftar</span><span class="sxs-lookup"><span data-stu-id="7ae06-116">Select a policy from the list</span></span>
    
3. <span data-ttu-id="7ae06-117">Klik **pengguna dan grup**</span><span class="sxs-lookup"><span data-stu-id="7ae06-117">Click **Users and groups**</span></span>
    
4. <span data-ttu-id="7ae06-118">Untuk menargetkan kebijakan tertentu pada seseorang, tambahkan ke daftar **sertakan** .</span><span class="sxs-lookup"><span data-stu-id="7ae06-118">To target a certain policy at someone, add them to the **Include** list.</span></span> <span data-ttu-id="7ae06-119">Untuk memastikan bahwa seseorang dihilangkan dari kebijakan, tambahkan ke daftar **Kecualikan** .</span><span class="sxs-lookup"><span data-stu-id="7ae06-119">To ensure that a person is omitted from the policy, add them to the **Exclude** list.</span></span> 
    
<span data-ttu-id="7ae06-120">Baca selengkapnya: [cara memantau perangkat akses bersyarat](https://docs.microsoft.com/intune/conditional-access-exchange-monitor)</span><span class="sxs-lookup"><span data-stu-id="7ae06-120">Read more: [How to Monitor Conditional Access devices](https://docs.microsoft.com/intune/conditional-access-exchange-monitor)</span></span>
  

