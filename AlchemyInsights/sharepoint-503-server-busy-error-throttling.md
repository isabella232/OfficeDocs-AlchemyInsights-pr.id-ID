---
title: Pelambatan SharePoint online
ms.author: pebaum
author: Techwriter40
ms.date: 9/17/2018
ms.audience: ITPro
ms.topic: article
ROBOTS: NOINDEX, NOFOLLOW
localization_priority: Normal
ms.assetid: b376d8ea-50c4-47f0-9720-50d80aa3f7f1
ms.openlocfilehash: d9e1400697b1e6435fea78703d2ecadc6733a57f
ms.sourcegitcommit: a65d196d00adb70045af5caca9828fe44b951f61
ms.translationtype: MT
ms.contentlocale: id-ID
ms.lasthandoff: 09/04/2019
ms.locfileid: "36751891"
---
# <a name="sharepoint-online-throttling"></a><span data-ttu-id="c420d-102">Pelambatan SharePoint online</span><span class="sxs-lookup"><span data-stu-id="c420d-102">SharePoint Online Throttling</span></span>

<span data-ttu-id="c420d-103">Pengguna akan menerima 503 server sibuk galat saat berusaha menavigasi ke situs SharePoint atau OneDrive.</span><span class="sxs-lookup"><span data-stu-id="c420d-103">Users may receive a 503 server is busy error when attempting to navigate to SharePoint or OneDrive sites.</span></span> 

<span data-ttu-id="c420d-104">Galat ini dapat disebabkan oleh pelambatan dalam Layanan SharePoint.</span><span class="sxs-lookup"><span data-stu-id="c420d-104">This error can be caused by throttling within the SharePoint service.</span></span> <span data-ttu-id="c420d-105">SharePoint Online menggunakan pelambatan untuk mempertahankan kinerja optimal dan keandalan Layanan SharePoint online.</span><span class="sxs-lookup"><span data-stu-id="c420d-105">SharePoint Online uses throttling to maintain optimal performance and reliability of the SharePoint Online service.</span></span> <span data-ttu-id="c420d-106">Pelambatan membatasi jumlah tindakan pengguna atau panggilan bersamaan (dengan skrip atau kode) untuk mencegah penggunaan sumber daya berlebihan.</span><span class="sxs-lookup"><span data-stu-id="c420d-106">Throttling limits the number of user actions or concurrent calls (by script or code) to prevent overuse of resources.</span></span> <span data-ttu-id="c420d-107">Jika Anda mendapatkan throttled, 99% dari waktu itu karena kode kustom.</span><span class="sxs-lookup"><span data-stu-id="c420d-107">If you do get throttled, 99% of the time it is because of custom code.</span></span>

<span data-ttu-id="c420d-108">Untuk informasi lebih lanjut tentang pelambatan Lihat, [Hindari mendapatkan mengalami kelambatan atau diblokir di SharePoint online](https://docs.microsoft.com/sharepoint/dev/general-development/how-to-avoid-getting-throttled-or-blocked-in-sharepoint-online).</span><span class="sxs-lookup"><span data-stu-id="c420d-108">For more information on throttling see, [Avoid getting throttled or blocked in SharePoint Online](https://docs.microsoft.com/sharepoint/dev/general-development/how-to-avoid-getting-throttled-or-blocked-in-sharepoint-online).</span></span>

<span data-ttu-id="c420d-109">Jika Anda yakin galat ini tidak terkait dengan throttling, Anda dapat memeriksa apakah ada pemeliharaan aktif yang terjadi pada penyewa Anda dengan menavigasi ke [pusat pesan](https://portal.office.com/adminportal/home#/MessageCenter).</span><span class="sxs-lookup"><span data-stu-id="c420d-109">If you believe this error is unrelated to throttling, you can check if there is active maintenance occurring on your tenant by navigating to the [Message center](https://portal.office.com/adminportal/home#/MessageCenter).</span></span>

 <span data-ttu-id="c420d-110">Akhirnya, pastikan Anda mengunjungi halaman [layanan kesehatan](https://portal.office.com/adminportal/home#/servicehealth) untuk memeriksa setiap saran/insiden yang mungkin terjadi.</span><span class="sxs-lookup"><span data-stu-id="c420d-110">Finally, ensure you visit the [Service Health](https://portal.office.com/adminportal/home#/servicehealth) page to check for any advisories/incidents that may be occurring.</span></span>

