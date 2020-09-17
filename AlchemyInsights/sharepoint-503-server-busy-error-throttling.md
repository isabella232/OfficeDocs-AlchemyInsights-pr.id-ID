---
title: Pembatasan SharePoint online
ms.author: pebaum
author: pebaum
ms.date: 04/21/2020
ms.audience: ITPro
ms.topic: article
ms.service: o365-administration
ROBOTS: NOINDEX, NOFOLLOW
localization_priority: Normal
ms.assetid: b376d8ea-50c4-47f0-9720-50d80aa3f7f1
ms.custom:
- "9000149"
- "1662"
- "3491"
ms.openlocfilehash: 21d0f8d0118d92562b425921742513157563b5fb
ms.sourcegitcommit: c6692ce0fa1358ec3529e59ca0ecdfdea4cdc759
ms.translationtype: MT
ms.contentlocale: id-ID
ms.lasthandoff: 09/15/2020
ms.locfileid: "47773850"
---
# <a name="sharepoint-online-throttling"></a><span data-ttu-id="1ee63-102">Pembatasan SharePoint online</span><span class="sxs-lookup"><span data-stu-id="1ee63-102">SharePoint Online Throttling</span></span>

<span data-ttu-id="1ee63-103">**Penting**: Selama masa-masa yang berat ini, kami mengambil langkah untuk memastikan bahwa SharePoint Online dan layanan OneDrive tetap memiliki ketersediaan yang tinggi. Silakan kunjungi [Penyesuaian Fitur Sementara SharePoint Online](https://aka.ms/ODSPAdjustments) untuk informasi selengkapnya.</span><span class="sxs-lookup"><span data-stu-id="1ee63-103">**Important**: During these unprecedented times, we are taking steps to ensure that SharePoint Online and OneDrive services remain highly available – Please visit [SharePoint Online Temporary Feature Adjustments](https://aka.ms/ODSPAdjustments) for more information.</span></span>

<span data-ttu-id="1ee63-104">**Server 503 adalah kesalahan sibuk**</span><span class="sxs-lookup"><span data-stu-id="1ee63-104">**503 server is busy error**</span></span>

<span data-ttu-id="1ee63-105">Pengguna mungkin menerima server 503 adalah kesalahan sibuk ketika mencoba menavigasi ke situs SharePoint atau OneDrive.</span><span class="sxs-lookup"><span data-stu-id="1ee63-105">Users may receive a 503 server is busy error when attempting to navigate to SharePoint or OneDrive sites.</span></span> 

<span data-ttu-id="1ee63-106">Kesalahan ini bisa disebabkan oleh pembatasan dalam Layanan SharePoint.</span><span class="sxs-lookup"><span data-stu-id="1ee63-106">This error can be caused by throttling within the SharePoint service.</span></span> <span data-ttu-id="1ee63-107">SharePoint Online menerapkan pembatasan untuk mempertahankan kinerja yang optimal dan keandalan layanan SharePoint Online.</span><span class="sxs-lookup"><span data-stu-id="1ee63-107">SharePoint Online uses throttling to maintain optimal performance and reliability of the SharePoint Online service.</span></span> <span data-ttu-id="1ee63-108">Pembatasan membatasi jumlah tindakan pengguna atau panggilan serentak (berdasarkan skrip atau kode) untuk mencegah penggunaan sumber daya secara berlebihan.</span><span class="sxs-lookup"><span data-stu-id="1ee63-108">Throttling limits the number of user actions or concurrent calls (by script or code) to prevent overuse of resources.</span></span> 

<span data-ttu-id="1ee63-109">Untuk informasi selengkapnya tentang pembatasan, [Hindari mendapatkan pembatasan atau diblokir di SharePoint online](https://docs.microsoft.com/sharepoint/dev/general-development/how-to-avoid-getting-throttled-or-blocked-in-sharepoint-online).</span><span class="sxs-lookup"><span data-stu-id="1ee63-109">For more information on throttling see, [Avoid getting throttled or blocked in SharePoint Online](https://docs.microsoft.com/sharepoint/dev/general-development/how-to-avoid-getting-throttled-or-blocked-in-sharepoint-online).</span></span>

<span data-ttu-id="1ee63-110">Jika Anda yakin kesalahan ini tidak terkait dengan pembatasan, Anda bisa memeriksa apakah ada pemeliharaan aktif yang terjadi pada penyewa Anda dengan menavigasi ke [pusat pesan](https://portal.office.com/adminportal/home#/MessageCenter).</span><span class="sxs-lookup"><span data-stu-id="1ee63-110">If you believe this error is unrelated to throttling, you can check if there is active maintenance occurring on your tenant by navigating to the [Message center](https://portal.office.com/adminportal/home#/MessageCenter).</span></span>

 <span data-ttu-id="1ee63-111">Terakhir, pastikan Anda mengunjungi halaman [Kesehatan Layanan](https://portal.office.com/adminportal/home#/servicehealth) untuk memeriksa setiap saran/kejadian yang mungkin terjadi.</span><span class="sxs-lookup"><span data-stu-id="1ee63-111">Finally, ensure you visit the [Service Health](https://portal.office.com/adminportal/home#/servicehealth) page to check for any advisories/incidents that may be occurring.</span></span>

