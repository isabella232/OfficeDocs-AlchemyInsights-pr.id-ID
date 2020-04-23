---
title: Pelambatan SharePoint online
ms.author: pebaum
author: pebaum
ms.date: 04/21/2020
ms.audience: ITPro
ms.topic: article
ROBOTS: NOINDEX, NOFOLLOW
localization_priority: Normal
ms.assetid: b376d8ea-50c4-47f0-9720-50d80aa3f7f1
ms.custom:
- "9000149"
- "1662"
- "3491"
ms.openlocfilehash: 50b2c29db1fd294abe6c9e60f067156109de392b
ms.sourcegitcommit: 631cbb5f03e5371f0995e976536d24e9d13746c3
ms.translationtype: MT
ms.contentlocale: id-ID
ms.lasthandoff: 04/22/2020
ms.locfileid: "43742212"
---
# <a name="sharepoint-online-throttling"></a><span data-ttu-id="0d5de-102">Pelambatan SharePoint online</span><span class="sxs-lookup"><span data-stu-id="0d5de-102">SharePoint Online Throttling</span></span>

<span data-ttu-id="0d5de-103">**Penting**: Selama masa-masa yang berat ini, kami mengambil langkah untuk memastikan bahwa SharePoint Online dan layanan OneDrive tetap memiliki ketersediaan yang tinggi. Silakan kunjungi [Penyesuaian Fitur Sementara SharePoint Online](https://aka.ms/ODSPAdjustments) untuk informasi selengkapnya.</span><span class="sxs-lookup"><span data-stu-id="0d5de-103">**Important**: During these unprecedented times, we are taking steps to ensure that SharePoint Online and OneDrive services remain highly available – Please visit [SharePoint Online Temporary Feature Adjustments](https://aka.ms/ODSPAdjustments) for more information.</span></span>

<span data-ttu-id="0d5de-104">**503 server sedang sibuk galat**</span><span class="sxs-lookup"><span data-stu-id="0d5de-104">**503 server is busy error**</span></span>

<span data-ttu-id="0d5de-105">Pengguna akan menerima 503 server sibuk galat saat berusaha menavigasi ke situs SharePoint atau OneDrive.</span><span class="sxs-lookup"><span data-stu-id="0d5de-105">Users may receive a 503 server is busy error when attempting to navigate to SharePoint or OneDrive sites.</span></span> 

<span data-ttu-id="0d5de-106">Galat ini dapat disebabkan oleh pelambatan dalam Layanan SharePoint.</span><span class="sxs-lookup"><span data-stu-id="0d5de-106">This error can be caused by throttling within the SharePoint service.</span></span> <span data-ttu-id="0d5de-107">SharePoint Online menerapkan pembatasan untuk mempertahankan kinerja yang optimal dan keandalan layanan SharePoint Online.</span><span class="sxs-lookup"><span data-stu-id="0d5de-107">SharePoint Online uses throttling to maintain optimal performance and reliability of the SharePoint Online service.</span></span> <span data-ttu-id="0d5de-108">Pembatasan membatasi jumlah tindakan pengguna atau panggilan serentak (berdasarkan skrip atau kode) untuk mencegah penggunaan sumber daya secara berlebihan.</span><span class="sxs-lookup"><span data-stu-id="0d5de-108">Throttling limits the number of user actions or concurrent calls (by script or code) to prevent overuse of resources.</span></span> 

<span data-ttu-id="0d5de-109">Untuk informasi lebih lanjut tentang pelambatan Lihat, [Hindari mendapatkan mengalami kelambatan atau diblokir di SharePoint online](https://docs.microsoft.com/sharepoint/dev/general-development/how-to-avoid-getting-throttled-or-blocked-in-sharepoint-online).</span><span class="sxs-lookup"><span data-stu-id="0d5de-109">For more information on throttling see, [Avoid getting throttled or blocked in SharePoint Online](https://docs.microsoft.com/sharepoint/dev/general-development/how-to-avoid-getting-throttled-or-blocked-in-sharepoint-online).</span></span>

<span data-ttu-id="0d5de-110">Jika Anda yakin galat ini tidak terkait dengan throttling, Anda dapat memeriksa apakah ada pemeliharaan aktif yang terjadi pada penyewa Anda dengan menavigasi ke [pusat pesan](https://portal.office.com/adminportal/home#/MessageCenter).</span><span class="sxs-lookup"><span data-stu-id="0d5de-110">If you believe this error is unrelated to throttling, you can check if there is active maintenance occurring on your tenant by navigating to the [Message center](https://portal.office.com/adminportal/home#/MessageCenter).</span></span>

 <span data-ttu-id="0d5de-111">Akhirnya, pastikan Anda mengunjungi halaman [layanan kesehatan](https://portal.office.com/adminportal/home#/servicehealth) untuk memeriksa setiap saran/insiden yang mungkin terjadi.</span><span class="sxs-lookup"><span data-stu-id="0d5de-111">Finally, ensure you visit the [Service Health](https://portal.office.com/adminportal/home#/servicehealth) page to check for any advisories/incidents that may be occurring.</span></span>

