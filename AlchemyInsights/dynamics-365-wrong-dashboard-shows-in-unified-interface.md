---
title: Dynamics 365-dasbor yang salah ditampilkan di antarmuka terpadu Dynamics 365
ms.author: pebaum
author: pebaum
ms.audience: ITPro
ms.topic: article
ms.service: o365-administration
ROBOTS: NOINDEX, NOFOLLOW
localization_priority: Normal
ms.custom:
- "1484"
- "6200024"
ms.openlocfilehash: 02e33c7dbdfe9b7d2ad7a04f154cf067fba0aab2
ms.sourcegitcommit: c6692ce0fa1358ec3529e59ca0ecdfdea4cdc759
ms.translationtype: MT
ms.contentlocale: id-ID
ms.lasthandoff: 09/14/2020
ms.locfileid: "47711278"
---
# <a name="wrong-dashboard-shows-in-dynamics-365-unified-interface"></a><span data-ttu-id="84c48-102">Dasbor yang salah ditampilkan di antarmuka terpadu Dynamics 365</span><span class="sxs-lookup"><span data-stu-id="84c48-102">Wrong dashboard shows in Dynamics 365 unified interface</span></span>

<span data-ttu-id="84c48-103">Ada beberapa alasan mengapa Anda melihat dasbor yang berbeda dari yang Anda duga:</span><span class="sxs-lookup"><span data-stu-id="84c48-103">There are several reasons why you may see a different dashboard than the one you expect:</span></span>

## <a name="the-user-has-set-a-user-default-dashboard"></a><span data-ttu-id="84c48-104">Pengguna telah mengatur dasbor default pengguna</span><span class="sxs-lookup"><span data-stu-id="84c48-104">The user has set a user default dashboard</span></span> 

<span data-ttu-id="84c48-105">Biasanya Anda bisa mengidentifikasi dasbor default pengguna diatur jika tombol **Atur sebagai default** tidak muncul di bilah perintah dasbor.</span><span class="sxs-lookup"><span data-stu-id="84c48-105">Typically you can identify a user default dashboard is set if the **Set As Default** button does not show in the dashboard command bar.</span></span> <span data-ttu-id="84c48-106">Dasbor default pengguna akan menimpa semua dasbor default lainnya, meskipun dasbor default pengguna tidak ada di aplikasi saat ini.</span><span class="sxs-lookup"><span data-stu-id="84c48-106">The user default dashboard will override all other default dashboards, even if the user's default dashboard is not in the current app.</span></span>

<span data-ttu-id="84c48-107">Gunakan solusi berikut untuk membuka dasbor default mereka.</span><span class="sxs-lookup"><span data-stu-id="84c48-107">Use the following workaround to unset their default dashboard.</span></span>

1. <span data-ttu-id="84c48-108">Membuat dasbor pribadi baru.</span><span class="sxs-lookup"><span data-stu-id="84c48-108">Create a new personal dashboard.</span></span>

2. <span data-ttu-id="84c48-109">Setel dasbor baru sebagai default pengguna.</span><span class="sxs-lookup"><span data-stu-id="84c48-109">Set that new dashboard as the user default.</span></span>

3. <span data-ttu-id="84c48-110">Hapus dasbor tersebut.</span><span class="sxs-lookup"><span data-stu-id="84c48-110">Delete that dashboard.</span></span>

## <a name="the-dashboard-is-set-in-the-sitemap"></a><span data-ttu-id="84c48-111">Dasbor diatur dalam peta situs</span><span class="sxs-lookup"><span data-stu-id="84c48-111">The dashboard is set in the sitemap</span></span>

<span data-ttu-id="84c48-112">Anda mungkin telah menetapkan dasbor default organisasi dengan memilih dasbor dan memilih ' setel sebagai default ' di bawah ' kustomisasi sistem '.</span><span class="sxs-lookup"><span data-stu-id="84c48-112">You may have set an organization default dashboard by selecting a dashboard and choosing 'Set As Default' under 'Customize The System'.</span></span> <span data-ttu-id="84c48-113">Tapi dasbor yang ditentukan dalam desainer Sitemap akan lebih diutamakan daripada dasbor ini, jika pengguna memiliki akses ke dasbor tersebut.</span><span class="sxs-lookup"><span data-stu-id="84c48-113">But the dashboard defined in the sitemap designer will take precedence over this dashboard, if the user has access to it.</span></span>

<span data-ttu-id="84c48-114">Untuk meminta pengguna melihat dasbor yang telah Anda setel sebagai default organisasi, Anda bisa:</span><span class="sxs-lookup"><span data-stu-id="84c48-114">To have users see the dashboard you've set as the organization default, you can either:</span></span>

* <span data-ttu-id="84c48-115">Mengatur dasbor tersebut dalam peta situs</span><span class="sxs-lookup"><span data-stu-id="84c48-115">Set that dashboard in the sitemap</span></span>

* <span data-ttu-id="84c48-116">Menghapus akses ke dasbor yang ditentukan Sitemap untuk pengguna tersebut</span><span class="sxs-lookup"><span data-stu-id="84c48-116">Remove access to the sitemap defined dashboard for those users</span></span>
