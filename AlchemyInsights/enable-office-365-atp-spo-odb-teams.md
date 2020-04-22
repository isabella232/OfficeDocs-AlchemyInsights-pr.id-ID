---
title: Mengaktifkan Office 365 ATP untuk SharePoint, OneDrive, dan Microsoft teams
ms.author: deniseb
author: denisebmsft
manager: laurawi
ms.date: 04/21/2020
ms.audience: Admin
ms.topic: article
ROBOTS: NOINDEX, NOFOLLOW
localization_priority: Normal
ms.collection: Admin_O365
ms.custom: 3100021
ms.openlocfilehash: fdfdc97a198898051a3388672d01994d96dd5e97
ms.sourcegitcommit: 55eff703a17e500681d8fa6a87eb067019ade3cc
ms.translationtype: MT
ms.contentlocale: id-ID
ms.lasthandoff: 04/22/2020
ms.locfileid: "43703429"
---
# <a name="enable-office-365-advanced-threat-protection-for-sharepoint-online-onedrive-and-microsoft-teams"></a><span data-ttu-id="a3d21-102">Mengaktifkan Office 365 lanjut ancaman perlindungan untuk SharePoint online, OneDrive dan Microsoft teams</span><span class="sxs-lookup"><span data-stu-id="a3d21-102">Enable Office 365 Advanced Threat Protection for SharePoint Online, OneDrive, and Microsoft Teams</span></span>

1. <span data-ttu-id="a3d21-103">Buka https://protection.office.com dan masuk.</span><span class="sxs-lookup"><span data-stu-id="a3d21-103">Go to https://protection.office.com and sign in.</span></span>
2. <span data-ttu-id="a3d21-104">Pilih > **Policy**kebijakan >  **manajemen ancaman\*\*\*\*lampiran aman**.</span><span class="sxs-lookup"><span data-stu-id="a3d21-104">Choose **Threat management** > **Policy** > **Safe Attachments**.</span></span>
3. <span data-ttu-id="a3d21-105">Pilih **Aktifkan ATP untuk SharePoint, OneDrive, dan Microsoft teams**, dan kemudian klik **Simpan**.</span><span class="sxs-lookup"><span data-stu-id="a3d21-105">Select **Turn on ATP for SharePoint, OneDrive, and Microsoft Teams**, and then click **Save**.</span></span>
4. <span data-ttu-id="a3d21-106">Merekomendasikan Sebagai administrator global atau administrator SharePoint online, Jalankan cmdlet [set-SPOTenant](https://docs.microsoft.com/powershell/module/sharepoint-online/Set-SPOTenant?view=sharepoint-ps) dengan parameter **Disallowinfectedfiledownload** ditetapkan ke *True*.</span><span class="sxs-lookup"><span data-stu-id="a3d21-106">(Recommended) As a global administrator or a SharePoint Online administrator, run the [Set-SPOTenant](https://docs.microsoft.com/powershell/module/sharepoint-online/Set-SPOTenant?view=sharepoint-ps) cmdlet with the **DisallowInfectedFileDownload** parameter set to *true*.</span></span>
5. <span data-ttu-id="a3d21-107">Merekomendasikan [Mengatur peringatan](https://docs.microsoft.com/office365/securitycompliance/turn-on-atp-for-spo-odb-and-teams#set-up-alerts-for-detected-files) untuk file terdeteksi.</span><span class="sxs-lookup"><span data-stu-id="a3d21-107">(Recommended) [Set up alerts](https://docs.microsoft.com/office365/securitycompliance/turn-on-atp-for-spo-odb-and-teams#set-up-alerts-for-detected-files) for detected files.</span></span>

> [!NOTE]
> <span data-ttu-id="a3d21-108">ATP akan nuntuk memindai setiap file tunggal di SharePoint online, OneDrive, atau Microsoft teams.</span><span class="sxs-lookup"><span data-stu-id="a3d21-108">ATP will nto scan every single file in SharePoint Online, OneDrive, or Microsoft Teams.</span></span> <span data-ttu-id="a3d21-109">File dipindai secara asinkron, melalui proses yang menggunakan kegiatan berbagi dan aktivitas tamu, bersama dengan heuristik cerdas dan sinyal ancaman untuk mengidentifikasi file berbahaya.</span><span class="sxs-lookup"><span data-stu-id="a3d21-109">Files are scanned asynchronously, through a process that uses sharing and guest activity events, along with smart heuristics and threat signals to identify malicious files.</span></span> <span data-ttu-id="a3d21-110">Lihat [https://docs.microsoft.com/office365/securitycompliance/atp-for-spo-odb-and-teams](https://docs.microsoft.com/office365/securitycompliance/atp-for-spo-odb-and-teams)semuanya.</span><span class="sxs-lookup"><span data-stu-id="a3d21-110">See [https://docs.microsoft.com/office365/securitycompliance/atp-for-spo-odb-and-teams](https://docs.microsoft.com/office365/securitycompliance/atp-for-spo-odb-and-teams).</span></span>