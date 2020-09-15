---
title: Baca-saja untuk pemeliharaan pesan ketika mencoba menggunakan SharePoint atau OneDrive
ms.author: pebaum
author: pebaum
manager: pamgreen
ms.audience: Admin
ms.topic: article
ms.service: o365-administration
ROBOTS: NOINDEX, NOFOLLOW
localization_priority: Normal
ms.collection: Adm_O365
ms.custom:
- "127"
- "128"
ms.assetid: de7b6877-f3f9-4402-8072-c73783aaccaa
ms.openlocfilehash: a3d313816beefcefa4d93528d3ad9a684e60390e
ms.sourcegitcommit: c6692ce0fa1358ec3529e59ca0ecdfdea4cdc759
ms.translationtype: MT
ms.contentlocale: id-ID
ms.lasthandoff: 09/14/2020
ms.locfileid: "47670835"
---
# <a name="read-only-for-maintenance-message-when-attempting-to-use-sharepoint-or-onedrive"></a><span data-ttu-id="4ee10-102">Baca-saja untuk pemeliharaan pesan ketika mencoba menggunakan SharePoint atau OneDrive</span><span class="sxs-lookup"><span data-stu-id="4ee10-102">Read-Only for Maintenance message when attempting to use SharePoint or OneDrive</span></span>

<span data-ttu-id="4ee10-103">Pengguna mungkin menerima pesan **baca-saja untuk pemeliharaan** saat mencoba menggunakan SharePoint atau OneDrive untuk salah satu skenario berikut ini.</span><span class="sxs-lookup"><span data-stu-id="4ee10-103">Users may receive a **Read-Only for Maintenance** message when attempting to use SharePoint or OneDrive for one of the following scenarios.</span></span> 

-   <span data-ttu-id="4ee10-104">Aktivitas pemeliharaan terencana atau aktif.</span><span class="sxs-lookup"><span data-stu-id="4ee10-104">A planned or active maintenance activity.</span></span>  <span data-ttu-id="4ee10-105">Periksalah dengan menavigasi ke [pusat pesan](https://portal.office.com/adminportal/home#/messagecenter).</span><span class="sxs-lookup"><span data-stu-id="4ee10-105">Check for them by navigating to the [Message Center](https://portal.office.com/adminportal/home#/messagecenter).</span></span>
-   <span data-ttu-id="4ee10-106">Insiden Layanan aktif prioritas tinggi yang mungkin terjadi.</span><span class="sxs-lookup"><span data-stu-id="4ee10-106">A high-priority, active service incident that may be occurring.</span></span> <span data-ttu-id="4ee10-107">Periksa saran/insiden dengan menavigasi ke [Kesehatan Layanan](https://portal.office.com/adminportal/home#/servicehealth).</span><span class="sxs-lookup"><span data-stu-id="4ee10-107">Check for any advisories/incidents by navigating to [Service Health](https://portal.office.com/adminportal/home#/servicehealth).</span></span>
-   <span data-ttu-id="4ee10-108">Skenario pemulihan otomatis yang kurang penyembuhan yang mungkin terjadi karena kejadian yang tidak diharapkan di server yang mungkin berlangsung kurang dari 30 menit atau lebih.</span><span class="sxs-lookup"><span data-stu-id="4ee10-108">A minor auto-healing recovery scenario that could be happening due to any unexpected events on the servers which might last for less than 30 min or so.</span></span> 
    
    <span data-ttu-id="4ee10-109">Tidak ada pusat pesan atau postingan Kesehatan Layanan untuk pemulihan kecil ini tetapi Anda harus kembali normal secepatnya.</span><span class="sxs-lookup"><span data-stu-id="4ee10-109">There are no Message Center or Service Health posts for these minor recoveries but you should be back to normal very soon.</span></span>

<span data-ttu-id="4ee10-110">Pada beberapa kesempatan kami mengamati bahwa salah satu dari tiga skenario yang tercantum di atas telah menjadi penyebabnya, dan layanan telah dipulihkan, namun tembolok browser pengguna belum dibersihkan.</span><span class="sxs-lookup"><span data-stu-id="4ee10-110">On very few occasions we observed that one of the three scenarios listed above have been the cause, and service has been restored, but the users browser cache hasn’t been cleared up.</span></span>

<span data-ttu-id="4ee10-111">Coba Kosongkan tembolok browser sebelum menavigasi ke situs.</span><span class="sxs-lookup"><span data-stu-id="4ee10-111">Please attempt to clear the browser cache before navigating to the site.</span></span>

1. <span data-ttu-id="4ee10-112">Di browser Microsoft Edge, pilih **pengaturan**, lalu pilih **privasi dan keamanan**.</span><span class="sxs-lookup"><span data-stu-id="4ee10-112">In your Microsoft Edge browser, select **Settings**, and then select **Privacy and Security**.</span></span>
2. <span data-ttu-id="4ee10-113">Di bawah **Hapus penelusuran**, pilih **pilih apa yang harus dihapus**.</span><span class="sxs-lookup"><span data-stu-id="4ee10-113">Under **Clear browsing**, select **Choose what to clear**.</span></span>
3. <span data-ttu-id="4ee10-114">Pilih **cookie dan data situs web yang disimpan**, lalu pilih **Hapus**.</span><span class="sxs-lookup"><span data-stu-id="4ee10-114">Select **Cookies and saved website data**, and select **Clear**.</span></span>

>[!Note] 
> <span data-ttu-id="4ee10-115">Langkah ini mungkin berbeda ketika menggunakan browser lain seperti Mozilla Firefox atau Google Chrome.</span><span class="sxs-lookup"><span data-stu-id="4ee10-115">These steps may differ when using other browsers such as Mozilla Firefox or Google Chrome.</span></span>

>[!Note] 
> <span data-ttu-id="4ee10-116">Opsi lainnya adalah membuka situs SharePoint atau OneDrive di jendela InPrivate yang baru.</span><span class="sxs-lookup"><span data-stu-id="4ee10-116">Another option would be to open your SharePoint site or OneDrive in a new InPrivate window.</span></span>