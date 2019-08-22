---
title: SharePoint Online Throttling
ms.author: kirks
author: Techwriter40
ms.date: 9/17/2018
ms.audience: ITPro
ms.topic: article
ROBOTS: NOINDEX, NOFOLLOW
localization_priority: Normal
ms.assetid: b376d8ea-50c4-47f0-9720-50d80aa3f7f1
ms.openlocfilehash: c7881c0c7331e0aa74fcc439f52157bb75a56160
ms.sourcegitcommit: 1d98db8acb9959aba3b5e308a567ade6b62da56c
ms.translationtype: MT
ms.contentlocale: id-ID
ms.lasthandoff: 08/22/2019
ms.locfileid: "36559844"
---
# <a name="sharepoint-online-throttling"></a><span data-ttu-id="3ff81-102">SharePoint Online Throttling</span><span class="sxs-lookup"><span data-stu-id="3ff81-102">SharePoint Online Throttling</span></span>

<span data-ttu-id="3ff81-103">Pengguna dapat menerima 503 server adalah sibuk kesalahan ketika mencoba untuk menavigasi ke situs SharePoint atau OneDrive.</span><span class="sxs-lookup"><span data-stu-id="3ff81-103">Users may receive a 503 server is busy error when attempting to navigate to SharePoint or OneDrive sites.</span></span> 

<span data-ttu-id="3ff81-104">Kesalahan ini dapat disebabkan oleh throttling dalam Layanan SharePoint.</span><span class="sxs-lookup"><span data-stu-id="3ff81-104">This error can be caused by throttling within the SharePoint service.</span></span> <span data-ttu-id="3ff81-105">SharePoint Online menggunakan throttling untuk mempertahankan kinerja yang optimal dan keandalan Layanan SharePoint Online.</span><span class="sxs-lookup"><span data-stu-id="3ff81-105">SharePoint Online uses throttling to maintain optimal performance and reliability of the SharePoint Online service.</span></span> <span data-ttu-id="3ff81-106">Throttling batas jumlah tindakan pengguna atau bersamaan panggilan (oleh script atau kode) untuk mencegah penggunaan berlebihan sumber daya.</span><span class="sxs-lookup"><span data-stu-id="3ff81-106">Throttling limits the number of user actions or concurrent calls (by script or code) to prevent overuse of resources.</span></span> <span data-ttu-id="3ff81-107">Jika Anda mendapatkan mencekik, 99% dari waktu karena kode kustom.</span><span class="sxs-lookup"><span data-stu-id="3ff81-107">If you do get throttled, 99% of the time it is because of custom code.</span></span>

<span data-ttu-id="3ff81-108">Untuk informasi lebih lanjut tentang throttling Lihat, [Hindari mendapatkan mencekik atau diblokir di SharePoint Online](https://docs.microsoft.com/sharepoint/dev/general-development/how-to-avoid-getting-throttled-or-blocked-in-sharepoint-online).</span><span class="sxs-lookup"><span data-stu-id="3ff81-108">For more information on throttling see, [Avoid getting throttled or blocked in SharePoint Online](https://docs.microsoft.com/sharepoint/dev/general-development/how-to-avoid-getting-throttled-or-blocked-in-sharepoint-online).</span></span>

<span data-ttu-id="3ff81-109">Jika Anda percaya kesalahan ini tidak berhubungan dengan throttling, Anda dapat memeriksa jika ada pemeliharaan aktif yang terjadi pada penyewa Anda dengan menavigasi ke [pusat pesan](https://portal.office.com/adminportal/home#/MessageCenter).</span><span class="sxs-lookup"><span data-stu-id="3ff81-109">If you believe this error is unrelated to throttling, you can check if there is active maintenance occurring on your tenant by navigating to the [Message center](https://portal.office.com/adminportal/home#/MessageCenter).</span></span>

 <span data-ttu-id="3ff81-110">Akhirnya, pastikan Anda mengunjungi halaman [Layanan kesehatan](https://portal.office.com/adminportal/home#/servicehealth) untuk memeriksa setiap nasihat/insiden yang mungkin terjadi.</span><span class="sxs-lookup"><span data-stu-id="3ff81-110">Finally, ensure you visit the [Service Health](https://portal.office.com/adminportal/home#/servicehealth) page to check for any advisories/incidents that may be occurring.</span></span>

