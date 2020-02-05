---
title: Penundaan dalam menerima SharePoint dan OneDrive peringatan
ms.author: v-todmc
author: todmccoy
manager: mnirkhe
ms.date: 02/04/2020
ms.audience: Admin
ms.topic: article
ROBOTS: NOINDEX, NOFOLLOW
localization_priority: Normal
ms.collection: Adm_O365
ms.custom:
- "9000118"
- "2642"
ms.openlocfilehash: 0bc9f614047e06e8654a9b3ff64e87427f33139f
ms.sourcegitcommit: 317eeed39c7777a922442992d67733726c41d9e1
ms.translationtype: MT
ms.contentlocale: id-ID
ms.lasthandoff: 02/04/2020
ms.locfileid: "41771218"
---
# <a name="delays-in-receiving-sharepoint-and-onedrive-alerts"></a><span data-ttu-id="dfa21-102">Penundaan dalam menerima SharePoint dan OneDrive peringatan</span><span class="sxs-lookup"><span data-stu-id="dfa21-102">Delays in receiving SharePoint and OneDrive alerts</span></span>

- <span data-ttu-id="dfa21-103">Pertama, periksa folder junk atau spam di email Anda.</span><span class="sxs-lookup"><span data-stu-id="dfa21-103">First check the Junk or Spam folder in your email.</span></span>
- <span data-ttu-id="dfa21-104">Jika **semua peringatan dari beberapa file atau Perpustakaan tertunda**, kunjungi [dasbor layanan kesehatan](https://nam06.safelinks.protection.outlook.com/?url=https://admin.microsoft.com/AdminPortal/Home%23/servicehealth&data=02%7c01%7cv-todmc%40microsoft.com%7c2cd2037aa7304711d2bc08d741fae254%7c72f988bf86f141af91ab2d7cd011db47%7c1%7c0%7c637050418099632638&sdata=35FUOTleK0Sc0z%2B7N7Vm0tOgXplyeOe3LcIzqRziGXc%3D&reserved=0) untuk memeriksa setiap saran/insiden yang mungkin terjadi dengan SharePoint atau Exchange.</span><span class="sxs-lookup"><span data-stu-id="dfa21-104">If **all alerts from multiple files or libraries are delayed**, visit the [Service Health dashboard](https://nam06.safelinks.protection.outlook.com/?url=https://admin.microsoft.com/AdminPortal/Home%23/servicehealth&data=02%7c01%7cv-todmc%40microsoft.com%7c2cd2037aa7304711d2bc08d741fae254%7c72f988bf86f141af91ab2d7cd011db47%7c1%7c0%7c637050418099632638&sdata=35FUOTleK0Sc0z%2B7N7Vm0tOgXplyeOe3LcIzqRziGXc%3D&reserved=0) to check for any advisories/incidents that may be occurring with SharePoint or Exchange.</span></span> <span data-ttu-id="dfa21-105">Masalah mungkin dengan kemampuan peringatan SharePoint atau penundaan dalam email melalui Exchange.</span><span class="sxs-lookup"><span data-stu-id="dfa21-105">The issue might be with the SharePoint alert capability or delays in emails through Exchange.</span></span> <span data-ttu-id="dfa21-106">Perhatikan juga Apakah email lain yang dikirim-jika tidak, masalah ini mungkin dengan penundaan Exchange.</span><span class="sxs-lookup"><span data-stu-id="dfa21-106">Also note whether other email is being delivered—if not, the issue is likely with Exchange delays.</span></span>
- <span data-ttu-id="dfa21-107">Jika **peringatan individu dari file atau perpustakaan tertentu tidak terkirim**, coba hapus dan buat ulang.</span><span class="sxs-lookup"><span data-stu-id="dfa21-107">If **an individual alert from a specific file or library is not delivered**, attempt to delete and recreate it.</span></span> <span data-ttu-id="dfa21-108">Lihat [mengelola, melihat, atau menghapus peringatan SharePoint](https://nam06.safelinks.protection.outlook.com/?url=https://support.office.com/article/manage-view-or-delete-sharepoint-alerts-99dfb19c-9a90-4a8c-aba1-aa8c8afb0de2?ui%3Den-US%26rs%3D%26ad%3DUS%23ID0EAADAAA%3DOnline&data=02%7c01%7cv-todmc%40microsoft.com%7c2cd2037aa7304711d2bc08d741fae254%7c72f988bf86f141af91ab2d7cd011db47%7c1%7c0%7c637050418099632638&sdata=AkE%2BjiG6%2BA59llp2DGcg4uHHUjaUDUnAlK5ax/epn3E%3D&reserved=0) untuk membuat ulang peringatan.</span><span class="sxs-lookup"><span data-stu-id="dfa21-108">See [Manage, view, or delete SharePoint alerts](https://nam06.safelinks.protection.outlook.com/?url=https://support.office.com/article/manage-view-or-delete-sharepoint-alerts-99dfb19c-9a90-4a8c-aba1-aa8c8afb0de2?ui%3Den-US%26rs%3D%26ad%3DUS%23ID0EAADAAA%3DOnline&data=02%7c01%7cv-todmc%40microsoft.com%7c2cd2037aa7304711d2bc08d741fae254%7c72f988bf86f141af91ab2d7cd011db47%7c1%7c0%7c637050418099632638&sdata=AkE%2BjiG6%2BA59llp2DGcg4uHHUjaUDUnAlK5ax/epn3E%3D&reserved=0) to recreate the alert.</span></span>

> [!NOTE]
> - <span data-ttu-id="dfa21-109">Peringatan tidak dapat dikirim ke grup distribusi.</span><span class="sxs-lookup"><span data-stu-id="dfa21-109">Alerts cannot be sent to a Distribution Group.</span></span> <span data-ttu-id="dfa21-110">Hanya grup keamanan dan O365 yang didukung.</span><span class="sxs-lookup"><span data-stu-id="dfa21-110">Only Security and O365 groups are supported.</span></span>
> - <span data-ttu-id="dfa21-111">Anda tidak dapat menyesuaikan template email peringatan.</span><span class="sxs-lookup"><span data-stu-id="dfa21-111">You cannot customize alert email templates.</span></span> <span data-ttu-id="dfa21-112">Anda harus menggunakan alur kerja Microsoft Flow atau SharePoint Designer untuk mencapainya.</span><span class="sxs-lookup"><span data-stu-id="dfa21-112">You must use Microsoft Flow or SharePoint Designer Workflow to achieve those.</span></span>
