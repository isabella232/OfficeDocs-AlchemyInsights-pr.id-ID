---
title: Mengaktifkan Office 365 ATP untuk SharePoint, OneDrive, dan tim Microsoft
ms.author: deniseb
author: denisebmsft
manager: laurawi
ms.date: 04/01/2019
ms.audience: Admin
ms.topic: article
ROBOTS: NOINDEX, NOFOLLOW
localization_priority: Normal
ms.collection: Admin_O365
ms.custom: 3100021
ms.openlocfilehash: ae2f574663ae3233a056589c2d5a578171f3b2f4
ms.sourcegitcommit: 601aec31e6556286fe5e0fd62827a037cbb6fe17
ms.translationtype: MT
ms.contentlocale: id-ID
ms.lasthandoff: 04/02/2019
ms.locfileid: "31030998"
---
# <a name="enable-office-365-advanced-threat-protection-for-sharepoint-online-onedrive-and-microsoft-teams"></a><span data-ttu-id="59fd6-102">Mengaktifkan Office 365 lanjutan ancaman perlindungan untuk SharePoint Online, OneDrive, dan tim Microsoft</span><span class="sxs-lookup"><span data-stu-id="59fd6-102">Enable Office 365 Advanced Threat Protection for SharePoint Online, OneDrive, and Microsoft Teams</span></span>

1. <span data-ttu-id="59fd6-103">Pergi ke https://protection.office.com dan masuk.</span><span class="sxs-lookup"><span data-stu-id="59fd6-103">Go to https://protection.office.com and sign in.</span></span>
2. <span data-ttu-id="59fd6-104">Memilih **manajemen ancaman** > **kebijakan** > **Lampiran aman**.</span><span class="sxs-lookup"><span data-stu-id="59fd6-104">Choose **Threat management** > **Policy** > **Safe Attachments**.</span></span>
3. <span data-ttu-id="59fd6-105">Pilih **Aktifkan ATP untuk SharePoint, OneDrive, dan Microsoft tim**, dan kemudian klik **Simpan**.</span><span class="sxs-lookup"><span data-stu-id="59fd6-105">Select **Turn on ATP for SharePoint, OneDrive, and Microsoft Teams**, and then click **Save**.</span></span>
4. <span data-ttu-id="59fd6-106">(Disarankan) Sebagai administrator global atau seorang administrator SharePoint Online, Jalankan cmdlet [Set-SPOTenant](https://docs.microsoft.com/powershell/module/sharepoint-online/Set-SPOTenant?view=sharepoint-ps) dengan parameter **DisallowInfectedFileDownload** diatur ke *true*.</span><span class="sxs-lookup"><span data-stu-id="59fd6-106">(Recommended) As a global administrator or a SharePoint Online administrator, run the [Set-SPOTenant](https://docs.microsoft.com/powershell/module/sharepoint-online/Set-SPOTenant?view=sharepoint-ps) cmdlet with the **DisallowInfectedFileDownload** parameter set to *true*.</span></span>
5. <span data-ttu-id="59fd6-107">(Disarankan) [Mengatur tanda](https://docs.microsoft.com/office365/securitycompliance/turn-on-atp-for-spo-odb-and-teams#set-up-alerts-for-detected-files) untuk file terdeteksi.</span><span class="sxs-lookup"><span data-stu-id="59fd6-107">(Recommended) [Set up alerts](https://docs.microsoft.com/office365/securitycompliance/turn-on-atp-for-spo-odb-and-teams#set-up-alerts-for-detected-files) for detected files.</span></span>

> [!NOTE]
> <span data-ttu-id="59fd6-108">ATP akan tidak memindai setiap satu file di SharePoint Online, OneDrive, atau Microsoft Teams.</span><span class="sxs-lookup"><span data-stu-id="59fd6-108">ATP will nto scan every single file in SharePoint Online, OneDrive, or Microsoft Teams.</span></span> <span data-ttu-id="59fd6-109">File scan asynchronously, melalui sebuah proses yang menggunakan berbagi dan tamu acara kegiatan, bersama dengan cerdas heuristik dan ancaman sinyal untuk mengidentifikasi file jahat.</span><span class="sxs-lookup"><span data-stu-id="59fd6-109">Files are scanned asynchronously, through a process that uses sharing and guest activity events, along with smart heuristics and threat signals to identify malicious files.</span></span> <span data-ttu-id="59fd6-110">Lihat [https://docs.microsoft.com/office365/securitycompliance/atp-for-spo-odb-and-teams](https://docs.microsoft.com/office365/securitycompliance/atp-for-spo-odb-and-teams).</span><span class="sxs-lookup"><span data-stu-id="59fd6-110">See [https://docs.microsoft.com/office365/securitycompliance/atp-for-spo-odb-and-teams](https://docs.microsoft.com/office365/securitycompliance/atp-for-spo-odb-and-teams).</span></span>