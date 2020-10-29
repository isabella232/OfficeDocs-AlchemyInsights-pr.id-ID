---
title: Mengaktifkan Office 365 ATP untuk SharePoint, OneDrive, dan Microsoft teams
ms.author: deniseb
author: denisebmsft
manager: laurawi
ms.date: 04/21/2020
ms.audience: Admin
ms.topic: article
ms.service: o365-administration
ROBOTS: NOINDEX, NOFOLLOW
localization_priority: Normal
ms.collection: Admin_O365
ms.custom: 3100021
ms.openlocfilehash: bef43656097c6f27677172899df1ada7900a9b64
ms.sourcegitcommit: 4caf5e6c2fee2903ccaf92cfc9006eb580faa7ba
ms.translationtype: MT
ms.contentlocale: id-ID
ms.lasthandoff: 10/29/2020
ms.locfileid: "48801051"
---
# <a name="enable-microsoft-defender-for-office-365-for-sharepoint-online-onedrive-and-microsoft-teams"></a><span data-ttu-id="bca88-102">Mengaktifkan Microsoft Defender untuk Office 365 untuk SharePoint online, OneDrive, dan Microsoft teams</span><span class="sxs-lookup"><span data-stu-id="bca88-102">Enable Microsoft Defender for Office 365 for SharePoint Online, OneDrive, and Microsoft Teams</span></span>

1. <span data-ttu-id="bca88-103">Masuk ke https://protection.office.com dan masuk.</span><span class="sxs-lookup"><span data-stu-id="bca88-103">Go to https://protection.office.com and sign in.</span></span>
2. <span data-ttu-id="bca88-104">Pilih **Threat management**  >  **Policy**  >  **lampiran aman** kebijakan manajemen ancaman.</span><span class="sxs-lookup"><span data-stu-id="bca88-104">Choose **Threat management** > **Policy** > **Safe Attachments** .</span></span>
3. <span data-ttu-id="bca88-105">Pilih **Aktifkan ATP untuk SharePoint, OneDrive, dan Microsoft teams** , lalu klik **Simpan** .</span><span class="sxs-lookup"><span data-stu-id="bca88-105">Select **Turn on ATP for SharePoint, OneDrive, and Microsoft Teams** , and then click **Save** .</span></span>
4. <span data-ttu-id="bca88-106">Telah Sebagai administrator global atau administrator SharePoint online, Jalankan cmdlet [set-SPOTenant](https://docs.microsoft.com/powershell/module/sharepoint-online/Set-SPOTenant?view=sharepoint-ps) dengan set parameter **Disallowinfecfiledownload** ke *True* .</span><span class="sxs-lookup"><span data-stu-id="bca88-106">(Recommended) As a global administrator or a SharePoint Online administrator, run the [Set-SPOTenant](https://docs.microsoft.com/powershell/module/sharepoint-online/Set-SPOTenant?view=sharepoint-ps) cmdlet with the **DisallowInfectedFileDownload** parameter set to *true* .</span></span>
5. <span data-ttu-id="bca88-107">Telah [Siapkan pemberitahuan](https://docs.microsoft.com/microsoft-365/security/office-365-security/turn-on-atp-for-spo-odb-and-teams#set-up-alerts-for-detected-files) untuk file yang terdeteksi.</span><span class="sxs-lookup"><span data-stu-id="bca88-107">(Recommended) [Set up alerts](https://docs.microsoft.com/microsoft-365/security/office-365-security/turn-on-atp-for-spo-odb-and-teams#set-up-alerts-for-detected-files) for detected files.</span></span>

> [!NOTE]
> <span data-ttu-id="bca88-108">ATP akan memindai setiap file di SharePoint online, OneDrive, atau Microsoft teams.</span><span class="sxs-lookup"><span data-stu-id="bca88-108">ATP will nto scan every single file in SharePoint Online, OneDrive, or Microsoft Teams.</span></span> <span data-ttu-id="bca88-109">File dipindai secara asinkron, melalui proses yang menggunakan acara berbagi dan aktivitas tamu, bersama dengan heuristics dan ancaman sinyal cerdas untuk mengidentifikasi file berbahaya.</span><span class="sxs-lookup"><span data-stu-id="bca88-109">Files are scanned asynchronously, through a process that uses sharing and guest activity events, along with smart heuristics and threat signals to identify malicious files.</span></span> <span data-ttu-id="bca88-110">Lihat [ATP untuk SharePoint, OneDrive, dan Microsoft teams](https://docs.microsoft.com/microsoft-365/security/office-365-security/atp-for-spo-odb-and-teams).</span><span class="sxs-lookup"><span data-stu-id="bca88-110">See [ATP for SharePoint, OneDrive, and Microsoft Teams](https://docs.microsoft.com/microsoft-365/security/office-365-security/atp-for-spo-odb-and-teams).</span></span>