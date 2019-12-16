---
title: Baca-saja untuk pemeliharaan pesan saat berusaha menggunakan SharePoint atau OneDrive
ms.author: pebaum
author: pebaum
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
ms.openlocfilehash: 02cf1aa7abae365a3d317af9e785648d1c1517e1
ms.sourcegitcommit: 0f0186044a3597e42ad14c32ca58e7224344dcfa
ms.translationtype: MT
ms.contentlocale: id-ID
ms.lasthandoff: 12/15/2019
ms.locfileid: "40051284"
---
# <a name="read-only-for-maintenance-message-when-attempting-to-use-sharepoint-or-onedrive"></a><span data-ttu-id="d30de-102">Baca-saja untuk pemeliharaan pesan saat berusaha menggunakan SharePoint atau OneDrive</span><span class="sxs-lookup"><span data-stu-id="d30de-102">Read-Only for Maintenance message when attempting to use SharePoint or OneDrive</span></span>

<span data-ttu-id="d30de-103">Pengguna akan menerima **baca-saja untuk pesan pemeliharaan** saat mencoba menggunakan SharePoint atau OneDrive untuk salah satu dari skenario berikut ini.</span><span class="sxs-lookup"><span data-stu-id="d30de-103">Users may receive a **Read-Only for Maintenance** message when attempting to use SharePoint or OneDrive for one of the following scenarios.</span></span> 

-   <span data-ttu-id="d30de-104">Kegiatan pemeliharaan yang direncanakan atau aktif.</span><span class="sxs-lookup"><span data-stu-id="d30de-104">A planned or active maintenance activity.</span></span>  <span data-ttu-id="d30de-105">Periksa untuk mereka dengan menavigasi ke [pusat pesan](https://portal.office.com/adminportal/home#/messagecenter).</span><span class="sxs-lookup"><span data-stu-id="d30de-105">Check for them by navigating to the [Message Center](https://portal.office.com/adminportal/home#/messagecenter).</span></span>
-   <span data-ttu-id="d30de-106">Sebuah kejadian layanan yang aktif dan prioritas tinggi yang mungkin terjadi.</span><span class="sxs-lookup"><span data-stu-id="d30de-106">A high-priority, active service incident that may be occurring.</span></span> <span data-ttu-id="d30de-107">Periksa apakah ada saran/insiden dengan menavigasi ke [layanan kesehatan](https://portal.office.com/adminportal/home#/servicehealth).</span><span class="sxs-lookup"><span data-stu-id="d30de-107">Check for any advisories/incidents by navigating to [Service Health](https://portal.office.com/adminportal/home#/servicehealth).</span></span>
-   <span data-ttu-id="d30de-108">Sebuah minor pemulihan Auto-penyembuhan skenario yang dapat terjadi karena setiap kejadian tak terduga pada server yang mungkin berlangsung selama kurang dari 30 menit atau lebih.</span><span class="sxs-lookup"><span data-stu-id="d30de-108">A minor auto-healing recovery scenario that could be happening due to any unexpected events on the servers which might last for less than 30 min or so.</span></span> 
    
    <span data-ttu-id="d30de-109">Ada tidak ada pusat pesan atau layanan kesehatan posting untuk pemulihan kecil ini tetapi Anda harus kembali normal segera.</span><span class="sxs-lookup"><span data-stu-id="d30de-109">There are no Message Center or Service Health posts for these minor recoveries but you should be back to normal very soon.</span></span>

<span data-ttu-id="d30de-110">Pada beberapa kesempatan kami mengamati bahwa salah satu dari tiga skenario yang tercantum di atas telah penyebabnya, dan layanan telah dipulihkan, tetapi cache browser pengguna belum dibersihkan.</span><span class="sxs-lookup"><span data-stu-id="d30de-110">On very few occasions we observed that one of the three scenarios listed above have been the cause, and service has been restored, but the users browser cache hasn’t been cleared up.</span></span>

<span data-ttu-id="d30de-111">Silakan mencoba untuk menghapus cache browser sebelum menavigasi ke situs.</span><span class="sxs-lookup"><span data-stu-id="d30de-111">Please attempt to clear the browser cache before navigating to the site.</span></span>

1. <span data-ttu-id="d30de-112">Di browser Microsoft Edge Anda, pilih **pengaturan**, dan kemudian pilih **privasi dan keamanan**.</span><span class="sxs-lookup"><span data-stu-id="d30de-112">In your Microsoft Edge browser, select **Settings**, and then select **Privacy and Security**.</span></span>
2. <span data-ttu-id="d30de-113">Di bawah **browsing yang jelas**, pilih **pilih apa yang harus jelas**.</span><span class="sxs-lookup"><span data-stu-id="d30de-113">Under **Clear browsing**, select **Choose what to clear**.</span></span>
3. <span data-ttu-id="d30de-114">Pilih **cookie dan data situs web yang disimpan**, lalu pilih **Hapus**.</span><span class="sxs-lookup"><span data-stu-id="d30de-114">Select **Cookies and saved website data**, and select **Clear**.</span></span>

>[!Note] 
> <span data-ttu-id="d30de-115">Langkah ini mungkin berbeda ketika menggunakan browser lain seperti Mozilla Firefox atau Google Chrome.</span><span class="sxs-lookup"><span data-stu-id="d30de-115">These steps may differ when using other browsers such as Mozilla Firefox or Google Chrome.</span></span>

>[!Note] 
> <span data-ttu-id="d30de-116">Pilihan lain akan membuka situs SharePoint atau OneDrive di jendela InPrivate baru.</span><span class="sxs-lookup"><span data-stu-id="d30de-116">Another option would be to open your SharePoint site or OneDrive in a new InPrivate window.</span></span>