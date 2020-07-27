---
title: Kebijakan perlindungan aplikasi
ms.author: pebaum
author: pebaum
manager: scotv
ms.date: 07/22/2020
ms.audience: Admin
ms.topic: article
ROBOTS: NOINDEX, NOFOLLOW
localization_priority: Priority
ms.collection: Adm_O365
ms.custom:
- "1073"
- "6700006"
ms.openlocfilehash: 7fed65e6749f72e6264070b360a52e72968fc8da
ms.sourcegitcommit: 6f7cbf1dc28c0693009ddf03d9768c1c65018964
ms.translationtype: MT
ms.contentlocale: id-ID
ms.lasthandoff: 07/22/2020
ms.locfileid: "45423597"
---
# <a name="application-protection-policy"></a><span data-ttu-id="52878-102">Kebijakan perlindungan aplikasi</span><span class="sxs-lookup"><span data-stu-id="52878-102">Application protection policy</span></span>

<span data-ttu-id="52878-103">Jika Anda baru menggunakan kebijakan perlindungan aplikasi (APP), lihat [Ikhtisar kebijakan perlindungan aplikasi](https://docs.microsoft.com/intune/apps/app-protection-policy).</span><span class="sxs-lookup"><span data-stu-id="52878-103">If you're new to Application protection policy (APP), check out the [App protection policies overview](https://docs.microsoft.com/intune/apps/app-protection-policy).</span></span>

<span data-ttu-id="52878-104">Untuk mulai menggunakan APP, lihat [cara membuat dan menetapkan kebijakan perlindungan aplikasi](https://docs.microsoft.com/intune/app-protection-policies).</span><span class="sxs-lookup"><span data-stu-id="52878-104">To start using APP, see [How to create and assign app protection policies](https://docs.microsoft.com/intune/app-protection-policies).</span></span>

<span data-ttu-id="52878-105">Persyaratan kebijakan perlindungan aplikasi:</span><span class="sxs-lookup"><span data-stu-id="52878-105">Application protection policy requirements:</span></span>

- <span data-ttu-id="52878-106">Pengguna memiliki lisensi Intune atau EMS.</span><span class="sxs-lookup"><span data-stu-id="52878-106">User has an Intune or EMS license.</span></span>
- <span data-ttu-id="52878-107">Pengguna milik grup yang ditargetkan oleh kebijakan perlindungan aplikasi.</span><span class="sxs-lookup"><span data-stu-id="52878-107">User belongs to a group targeted by application protection policies.</span></span>
- <span data-ttu-id="52878-108">Hanya satu pengguna korporat yang masuk ke aplikasi yang dilindungi pada perangkat.</span><span class="sxs-lookup"><span data-stu-id="52878-108">Only one corporate user is signed into protected apps on a device.</span></span>
- <span data-ttu-id="52878-109">Aplikasi telah menerapkan [INTUNE SDK](https://docs.microsoft.com/intune/app-sdk-get-started).</span><span class="sxs-lookup"><span data-stu-id="52878-109">The application has implemented the [Intune SDK](https://docs.microsoft.com/intune/app-sdk-get-started).</span></span> <span data-ttu-id="52878-110">Untuk daftar aplikasi yang mendukung SDK, lihat [aplikasi yang dilindungi Microsoft Intune](https://docs.microsoft.com/intune/apps-supported-intune-apps).</span><span class="sxs-lookup"><span data-stu-id="52878-110">For a list of apps that support the SDK, see [Microsoft Intune protected apps](https://docs.microsoft.com/intune/apps-supported-intune-apps).</span></span>

<span data-ttu-id="52878-111">Kebijakan berlaku setelah pengguna yang memenuhi persyaratan di atas tanda ke Intune SDK diaktifkan aplikasi.</span><span class="sxs-lookup"><span data-stu-id="52878-111">Policies apply after a user who meets the above requirements signs into an Intune SDK enabled app.</span></span> <span data-ttu-id="52878-112">Cara termudah untuk menentukan apakah kebijakan diterapkan adalah dengan mewajibkan pengguna menetapkan pin dalam kebijakan.</span><span class="sxs-lookup"><span data-stu-id="52878-112">The easiest way to determine if a policy is applied is by requiring that the user set a pin in the policy.</span></span> 

<span data-ttu-id="52878-113">Untuk informasi selengkapnya, lihat:</span><span class="sxs-lookup"><span data-stu-id="52878-113">For more information, see:</span></span>

[<span data-ttu-id="52878-114">FAQ pemecahan masalah APP/MAM</span><span class="sxs-lookup"><span data-stu-id="52878-114">APP/MAM troubleshooting FAQ</span></span>](https://docs.microsoft.com/intune/apps/troubleshoot-mam)  

[<span data-ttu-id="52878-115">Cara memvalidasi penyiapan kebijakan perlindungan aplikasi</span><span class="sxs-lookup"><span data-stu-id="52878-115">How to validate your app protection policy setup</span></span>](https://docs.microsoft.com/intune/app-protection-policies-validate)

[<span data-ttu-id="52878-116">Memahami waktu pengiriman kebijakan perlindungan aplikasi</span><span class="sxs-lookup"><span data-stu-id="52878-116">Understand App Protection Policy delivery timing</span></span>](https://docs.microsoft.com/intune/app-protection-policy-delivery)  

[<span data-ttu-id="52878-117">Cara memantau kebijakan perlindungan aplikasi</span><span class="sxs-lookup"><span data-stu-id="52878-117">How to monitor app protection policies</span></span>](https://docs.microsoft.com/intune/app-protection-policies-monitor)