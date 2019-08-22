---
title: Dynamics 365 - salah Dashboard menunjukkan dalam antarmuka yang bersatu Dynamics 365
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
ms.sourcegitcommit: 1d98db8acb9959aba3b5e308a567ade6b62da56c
ms.translationtype: MT
ms.contentlocale: id-ID
ms.lasthandoff: 08/22/2019
ms.locfileid: "36528554"
---
# <a name="wrong-dashboard-shows-in-dynamics-365-unified-interface"></a><span data-ttu-id="f5b17-102">Salah dashboard menunjukkan dalam antarmuka yang bersatu Dynamics 365</span><span class="sxs-lookup"><span data-stu-id="f5b17-102">Wrong dashboard shows in Dynamics 365 unified interface</span></span>

<span data-ttu-id="f5b17-103">Ada beberapa alasan mengapa Anda mungkin melihat sebuah dashboard yang berbeda daripada yang Anda harapkan:</span><span class="sxs-lookup"><span data-stu-id="f5b17-103">There are several reasons why you may see a different dashboard than the one you expect:</span></span>

## <a name="the-user-has-set-a-user-default-dashboard"></a><span data-ttu-id="f5b17-104">Pengguna telah menetapkan pengguna default dashboard</span><span class="sxs-lookup"><span data-stu-id="f5b17-104">The user has set a user default dashboard</span></span> 

<span data-ttu-id="f5b17-105">Biasanya Anda dapat mengidentifikasi pengguna default dashboard diatur jika tombol **Set sebagai Default** tidak menunjukkan di bilah perintah dashboard.</span><span class="sxs-lookup"><span data-stu-id="f5b17-105">Typically you can identify a user default dashboard is set if the **Set As Default** button does not show in the dashboard command bar.</span></span> <span data-ttu-id="f5b17-106">Pengguna default dashboard akan menimpa semua default dashboard, bahkan jika pengguna default dasbor tidak di app saat ini.</span><span class="sxs-lookup"><span data-stu-id="f5b17-106">The user default dashboard will override all other default dashboards, even if the user's default dashboard is not in the current app.</span></span>

<span data-ttu-id="f5b17-107">Menggunakan solusi berikut untuk unset dashboard default mereka.</span><span class="sxs-lookup"><span data-stu-id="f5b17-107">Use the following workaround to unset their default dashboard.</span></span>

1. <span data-ttu-id="f5b17-108">Membuat dashboard pribadi baru.</span><span class="sxs-lookup"><span data-stu-id="f5b17-108">Create a new personal dashboard.</span></span>

2. <span data-ttu-id="f5b17-109">Menetapkan dashboard yang baru sebagai default pengguna.</span><span class="sxs-lookup"><span data-stu-id="f5b17-109">Set that new dashboard as the user default.</span></span>

3. <span data-ttu-id="f5b17-110">Menghapus dashboard itu.</span><span class="sxs-lookup"><span data-stu-id="f5b17-110">Delete that dashboard.</span></span>

## <a name="the-dashboard-is-set-in-the-sitemap"></a><span data-ttu-id="f5b17-111">Dashboard terletak di sitemap</span><span class="sxs-lookup"><span data-stu-id="f5b17-111">The dashboard is set in the sitemap</span></span>

<span data-ttu-id="f5b17-112">Anda dapat menetapkan dashboard default organisasi dengan memilih sebuah dashboard dan memilih 'Set sebagai Default' di bawah 'Menyesuaikan sistem'.</span><span class="sxs-lookup"><span data-stu-id="f5b17-112">You may have set an organization default dashboard by selecting a dashboard and choosing 'Set As Default' under 'Customize The System'.</span></span> <span data-ttu-id="f5b17-113">Tapi dashboard didefinisikan dalam desain sitemap akan mengambil alih dashboard ini, jika pengguna memiliki akses ke sana.</span><span class="sxs-lookup"><span data-stu-id="f5b17-113">But the dashboard defined in the sitemap designer will take precedence over this dashboard, if the user has access to it.</span></span>

<span data-ttu-id="f5b17-114">Agar pengguna melihat dashboard Anda tetapkan sebagai default organisasi, Anda dapat:</span><span class="sxs-lookup"><span data-stu-id="f5b17-114">To have users see the dashboard you've set as the organization default, you can either:</span></span>

* <span data-ttu-id="f5b17-115">Menetapkan bahwa dashboard dalam sitemap</span><span class="sxs-lookup"><span data-stu-id="f5b17-115">Set that dashboard in the sitemap</span></span>

* <span data-ttu-id="f5b17-116">Menghapus akses ke dashboard sitemap yang ditetapkan bagi para pengguna</span><span class="sxs-lookup"><span data-stu-id="f5b17-116">Remove access to the sitemap defined dashboard for those users</span></span>
