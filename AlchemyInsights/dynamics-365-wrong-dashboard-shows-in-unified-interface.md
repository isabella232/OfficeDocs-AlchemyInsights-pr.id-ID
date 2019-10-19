---
title: Dynamics 365-salah Dasbor menunjukkan di Dynamics 365 antarmuka terpadu
ms.author: pebaum
author: pebaum
ms.audience: ITPro
ms.topic: article
ROBOTS: NOINDEX, NOFOLLOW
localization_priority: Normal
ms.custom:
- "1484"
- "6200024"
ms.openlocfilehash: 3d7258bdd7366f679b048e93926ab7dfe0b956d9
ms.sourcegitcommit: 037331d71f06750d972c0b6278b23bb15c4806ca
ms.translationtype: MT
ms.contentlocale: id-ID
ms.lasthandoff: 10/18/2019
ms.locfileid: "36528554"
---
# <a name="wrong-dashboard-shows-in-dynamics-365-unified-interface"></a><span data-ttu-id="51ec5-102">Salah dashboard menunjukkan di antarmuka terpadu Dynamics 365</span><span class="sxs-lookup"><span data-stu-id="51ec5-102">Wrong dashboard shows in Dynamics 365 unified interface</span></span>

<span data-ttu-id="51ec5-103">Ada beberapa alasan mengapa Anda mungkin melihat dasbor yang berbeda dari yang Anda harapkan:</span><span class="sxs-lookup"><span data-stu-id="51ec5-103">There are several reasons why you may see a different dashboard than the one you expect:</span></span>

## <a name="the-user-has-set-a-user-default-dashboard"></a><span data-ttu-id="51ec5-104">Pengguna telah menetapkan dashboard default pengguna</span><span class="sxs-lookup"><span data-stu-id="51ec5-104">The user has set a user default dashboard</span></span> 

<span data-ttu-id="51ec5-105">Biasanya Anda dapat mengidentifikasi dashboard default pengguna diatur jika **ditetapkan sebagai default** tombol tidak muncul di bilah perintah dasbor.</span><span class="sxs-lookup"><span data-stu-id="51ec5-105">Typically you can identify a user default dashboard is set if the **Set As Default** button does not show in the dashboard command bar.</span></span> <span data-ttu-id="51ec5-106">Dasbor default pengguna akan menimpa semua dasbor default lainnya, meskipun dasbor default pengguna tidak ada di aplikasi saat ini.</span><span class="sxs-lookup"><span data-stu-id="51ec5-106">The user default dashboard will override all other default dashboards, even if the user's default dashboard is not in the current app.</span></span>

<span data-ttu-id="51ec5-107">Gunakan solusi berikut untuk Unset dashboard default mereka.</span><span class="sxs-lookup"><span data-stu-id="51ec5-107">Use the following workaround to unset their default dashboard.</span></span>

1. <span data-ttu-id="51ec5-108">Buat dasbor pribadi baru.</span><span class="sxs-lookup"><span data-stu-id="51ec5-108">Create a new personal dashboard.</span></span>

2. <span data-ttu-id="51ec5-109">Setel dasbor baru sebagai default pengguna.</span><span class="sxs-lookup"><span data-stu-id="51ec5-109">Set that new dashboard as the user default.</span></span>

3. <span data-ttu-id="51ec5-110">Hapus dasbor tersebut.</span><span class="sxs-lookup"><span data-stu-id="51ec5-110">Delete that dashboard.</span></span>

## <a name="the-dashboard-is-set-in-the-sitemap"></a><span data-ttu-id="51ec5-111">Dasbor diatur dalam peta situs</span><span class="sxs-lookup"><span data-stu-id="51ec5-111">The dashboard is set in the sitemap</span></span>

<span data-ttu-id="51ec5-112">Anda mungkin telah menetapkan dashboard default organisasi dengan memilih dashboard dan memilih ' set AS default ' di bawah ' Customize The System '.</span><span class="sxs-lookup"><span data-stu-id="51ec5-112">You may have set an organization default dashboard by selecting a dashboard and choosing 'Set As Default' under 'Customize The System'.</span></span> <span data-ttu-id="51ec5-113">Namun dasbor yang ditetapkan dalam perancang peta situs akan diutamakan daripada dasbor ini, jika pengguna memiliki akses ke dashboard tersebut.</span><span class="sxs-lookup"><span data-stu-id="51ec5-113">But the dashboard defined in the sitemap designer will take precedence over this dashboard, if the user has access to it.</span></span>

<span data-ttu-id="51ec5-114">Agar pengguna melihat dasbor yang Anda tetapkan sebagai default organisasi, Anda dapat:</span><span class="sxs-lookup"><span data-stu-id="51ec5-114">To have users see the dashboard you've set as the organization default, you can either:</span></span>

* <span data-ttu-id="51ec5-115">Menyetel dasbor di peta situs</span><span class="sxs-lookup"><span data-stu-id="51ec5-115">Set that dashboard in the sitemap</span></span>

* <span data-ttu-id="51ec5-116">Hapus akses ke dasbor yang ditetapkan peta situs untuk pengguna tersebut</span><span class="sxs-lookup"><span data-stu-id="51ec5-116">Remove access to the sitemap defined dashboard for those users</span></span>
