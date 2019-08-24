---
title: Read-Only untuk pemeliharaan pesan saat mencoba untuk menggunakan SharePoint atau OneDrive
ms.author: efrene
author: efrene
manager: pamgreen
ms.audience: Admin
ms.topic: article
ROBOTS: NOINDEX, NOFOLLOW
localization_priority: Normal
ms.collection: Adm_O365
ms.custom:
- "127"
- "128"
ms.assetid: de7b6877-f3f9-4402-8072-c73783aaccaa
ms.openlocfilehash: 5b1e56253d6deeb0f9ba2f753eff5c00ff9c51a2
ms.sourcegitcommit: cd79ecca88b2cb166f78f44ab8bc4e8136729418
ms.translationtype: MT
ms.contentlocale: id-ID
ms.lasthandoff: 08/23/2019
ms.locfileid: "36620726"
---
# <a name="read-only-for-maintenance-message-when-attempting-to-use-sharepoint-or-onedrive"></a><span data-ttu-id="79dc4-102">Read-Only untuk pemeliharaan pesan saat mencoba untuk menggunakan SharePoint atau OneDrive</span><span class="sxs-lookup"><span data-stu-id="79dc4-102">Read-Only for Maintenance message when attempting to use SharePoint or OneDrive</span></span>

<span data-ttu-id="79dc4-103">Pengguna dapat menerima pesan **Read-Only untuk pemeliharaan** saat mencoba untuk menggunakan SharePoint atau OneDrive untuk salah satu skenario berikut.</span><span class="sxs-lookup"><span data-stu-id="79dc4-103">Users may receive a **Read-Only for Maintenance** message when attempting to use SharePoint or OneDrive for one of the following scenarios.</span></span> 

-   <span data-ttu-id="79dc4-104">Kegiatan pemeliharaan direncanakan atau aktif.</span><span class="sxs-lookup"><span data-stu-id="79dc4-104">A planned or active maintenance activity.</span></span>  <span data-ttu-id="79dc4-105">Memeriksa mereka dengan menavigasi ke [Pusat pesan](https://portal.office.com/adminportal/home#/messagecenter).</span><span class="sxs-lookup"><span data-stu-id="79dc4-105">Check for them by navigating to the [Message Center](https://portal.office.com/adminportal/home#/messagecenter).</span></span>
-   <span data-ttu-id="79dc4-106">Layanan aktif prioritas tinggi, insiden yang mungkin terjadi.</span><span class="sxs-lookup"><span data-stu-id="79dc4-106">A high-priority, active service incident that may be occurring.</span></span> <span data-ttu-id="79dc4-107">Periksa setiap nasihat/insiden dengan menavigasi ke [Layanan kesehatan](https://portal.office.com/adminportal/home#/servicehealth).</span><span class="sxs-lookup"><span data-stu-id="79dc4-107">Check for any advisories/incidents by navigating to [Service Health](https://portal.office.com/adminportal/home#/servicehealth).</span></span>
-   <span data-ttu-id="79dc4-108">Kecil menyembuhkan pemulihan skenario yang mungkin terjadi karena setiap kejadian tak terduga di server yang mungkin bertahan selama kurang dari 30 menit atau lebih.</span><span class="sxs-lookup"><span data-stu-id="79dc4-108">A minor auto-healing recovery scenario that could be happening due to any unexpected events on the servers which might last for less than 30 min or so.</span></span> 
    
    <span data-ttu-id="79dc4-109">Ada tidak ada pusat pesan atau jasa kesehatan posts untuk pemulihan ini kecil tapi Anda harus kembali ke normal segera.</span><span class="sxs-lookup"><span data-stu-id="79dc4-109">There are no Message Center or Service Health posts for these minor recoveries but you should be back to normal very soon.</span></span>

<span data-ttu-id="79dc4-110">Pada beberapa kesempatan kami mengamati bahwa salah satu dari tiga skenario yang tercantum di atas telah menjadi penyebab, dan layanan telah dikembalikan, tetapi cache browser pengguna belum dibersihkan.</span><span class="sxs-lookup"><span data-stu-id="79dc4-110">On very few occasions we observed that one of the three scenarios listed above have been the cause, and service has been restored, but the users browser cache hasn’t been cleared up.</span></span>

<span data-ttu-id="79dc4-111">Silakan mencoba membersihkan browser cache sebelum menavigasi ke situs.</span><span class="sxs-lookup"><span data-stu-id="79dc4-111">Please attempt to clear the browser cache before navigating to the site.</span></span>

1. <span data-ttu-id="79dc4-112">Di peramban Microsoft Edge, pilih **pengaturan**, dan kemudian pilih **privasi dan keamanan**.</span><span class="sxs-lookup"><span data-stu-id="79dc4-112">In your Microsoft Edge browser, select **Settings**, and then select **Privacy and Security**.</span></span>
2. <span data-ttu-id="79dc4-113">**Jelas browsing**, pilih **memilih apa yang harus jelas**.</span><span class="sxs-lookup"><span data-stu-id="79dc4-113">Under **Clear browsing**, select **Choose what to clear**.</span></span>
3. <span data-ttu-id="79dc4-114">Pilih **kuki dan data situs web tersimpan**, dan pilih **jelas**.</span><span class="sxs-lookup"><span data-stu-id="79dc4-114">Select **Cookies and saved website data**, and select **Clear**.</span></span>

>[!Note] 
> <span data-ttu-id="79dc4-115">Langkah-langkah ini mungkin berbeda dengan menggunakan peramban lainnya, seperti Mozilla Firefox atau Google Chrome.</span><span class="sxs-lookup"><span data-stu-id="79dc4-115">These steps may differ when using other browsers such as Mozilla Firefox or Google Chrome.</span></span>

>[!Note] 
> <span data-ttu-id="79dc4-116">Pilihan lain adalah untuk membuka situs SharePoint atau OneDrive di jendela InPrivate baru.</span><span class="sxs-lookup"><span data-stu-id="79dc4-116">Another option would be to open your SharePoint site or OneDrive in a new InPrivate window.</span></span>