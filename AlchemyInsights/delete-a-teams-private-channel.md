---
title: Menghapus saluran pribadi teams
ms.author: pebaum
author: pebaum
manager: scotv
ms.date: 07/24/2020
ms.audience: Admin
ms.topic: article
ROBOTS: NOINDEX, NOFOLLOW
localization_priority: Priority
ms.collection: Adm_O365
ms.custom:
- "3781"
- "9001223"
ms.openlocfilehash: 2ee998f0c70973645c273a2a6609af2420a4f74b
ms.sourcegitcommit: b10cea11b4975354b91193327b58aa4740d34833
ms.translationtype: MT
ms.contentlocale: id-ID
ms.lasthandoff: 07/28/2020
ms.locfileid: "45439325"
---
# <a name="delete-a-teams-private-channel"></a><span data-ttu-id="b7d31-102">Menghapus saluran pribadi teams</span><span class="sxs-lookup"><span data-stu-id="b7d31-102">Delete a Teams private channel</span></span>

<span data-ttu-id="b7d31-103">Microsoft telah mengetahui masalah menghapus teams saluran pribadi jika Anda memiliki kebijakan retensi SharePoint diaktifkan untuk situs SharePoint dasar.</span><span class="sxs-lookup"><span data-stu-id="b7d31-103">Microsoft is aware of an issue deleting a Teams private channel if you have SharePoint Retention Policies enabled for the underlying SharePoint site.</span></span> <span data-ttu-id="b7d31-104">Microsoft bekerja pada perbaikan.</span><span class="sxs-lookup"><span data-stu-id="b7d31-104">Microsoft is working on a fix.</span></span> <span data-ttu-id="b7d31-105">Sementara itu, Anda dapat menggunakan penyelesaian masalah berikut untuk menghapus saluran pribadi.</span><span class="sxs-lookup"><span data-stu-id="b7d31-105">In the meantime, you can use the following workarounds to delete the private channel.</span></span>

<span data-ttu-id="b7d31-106">**Mengecualikan koleksi tim situs dari kebijakan retensi SharePoint.**</span><span class="sxs-lookup"><span data-stu-id="b7d31-106">**Exclude the Team/site collection from the Sharepoint retention policy.**</span></span>

1. <span data-ttu-id="b7d31-107">Buka portal admin Office 365, dan pilih **Tampilkan semua** di panel navigasi kiri.</span><span class="sxs-lookup"><span data-stu-id="b7d31-107">Go to the Office 365 admin portal, and select **Show all** in the left navigation pane.</span></span>
2. <span data-ttu-id="b7d31-108">Di **Pusat admin**, buka kebijakan **Security & Compliance**  >  **pencegahan kehilangan data**kepatuhan & keamanan  >  **Policy**.</span><span class="sxs-lookup"><span data-stu-id="b7d31-108">Under **Admin centers**, go to **Security & Compliance** > **Data Loss Prevention** > **Policy**.</span></span>
3. <span data-ttu-id="b7d31-109">Mengidentifikasi kebijakan yang berlaku untuk situs SharePoint, dan mengubah kebijakan sehingga situs SharePoint untuk tim yang berisi saluran pribadi tidak disertakan dalam kebijakan retensi.</span><span class="sxs-lookup"><span data-stu-id="b7d31-109">Identify any policy that applies to Sharepoint sites, and modify the policy so the Sharepoint site for the Team containing the private channel is NOT included under the retention policy.</span></span>
4. <span data-ttu-id="b7d31-110">Simpan kebijakan.</span><span class="sxs-lookup"><span data-stu-id="b7d31-110">Save the policy.</span></span>
    <span data-ttu-id="b7d31-111">Diperlukan waktu hingga 24 jam agar pengaturan kebijakan diterapkan.</span><span class="sxs-lookup"><span data-stu-id="b7d31-111">It can take up to 24 hours for policy settings to take effect.</span></span>
    <span data-ttu-id="b7d31-112">Setelah situs dikecualikan, Anda dapat menghapus saluran pribadi.</span><span class="sxs-lookup"><span data-stu-id="b7d31-112">After the site has been excluded, you can delete the private channel.</span></span>  
    
<span data-ttu-id="b7d31-113">Anda ***mungkin*** dapat menghapus saluran pribadi dengan menggunakan Microsoft teams di perangkat Android.</span><span class="sxs-lookup"><span data-stu-id="b7d31-113">You  ***might*** be able to delete the private channel by using Microsoft Teams on your Android device.</span></span> 

<span data-ttu-id="b7d31-114">Untuk informasi terkait SharePoint, lihat [tidak dapat menghapus item di SharePoint online atau OneDrive untuk bisnis](https://docs.microsoft.com/alchemyinsights/retention-policy-ediscovery-hold).</span><span class="sxs-lookup"><span data-stu-id="b7d31-114">For related SharePoint information, see [Unable to delete items in SharePoint Online or OneDrive for Business](https://docs.microsoft.com/alchemyinsights/retention-policy-ediscovery-hold).</span></span>