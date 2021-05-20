---
title: Mengaktifkan Office 365 ATP untuk SharePoint, OneDrive, dan Microsoft Teams
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
ms.openlocfilehash: dd367176f8d6f38f1f94ae6627229234f15c81ff
ms.sourcegitcommit: f4866e94918c7b591ad0cd3b58169d340bcc7f00
ms.translationtype: MT
ms.contentlocale: id-ID
ms.lasthandoff: 05/19/2021
ms.locfileid: "52543931"
---
# <a name="enable-microsoft-defender-for-office-365-for-sharepoint-online-onedrive-and-microsoft-teams"></a><span data-ttu-id="419c6-102">Mengaktifkan Pertahanan Microsoft untuk Office 365 untuk SharePoint Online, OneDrive, dan Microsoft Teams</span><span class="sxs-lookup"><span data-stu-id="419c6-102">Enable Microsoft Defender for Office 365 for SharePoint Online, OneDrive, and Microsoft Teams</span></span>

1. <span data-ttu-id="419c6-103">Buka https://protection.office.com dan masuk.</span><span class="sxs-lookup"><span data-stu-id="419c6-103">Go to https://protection.office.com and sign in.</span></span>
2. <span data-ttu-id="419c6-104">Pilih **Kebijakan manajemen**  >  **ancaman** Brankas  >  **Lampiran**.</span><span class="sxs-lookup"><span data-stu-id="419c6-104">Choose **Threat management** > **Policy** > **Safe Attachments**.</span></span>
3. <span data-ttu-id="419c6-105">Pilih **Aktifkan Pertahanan untuk Office 365 untuk SharePoint, OneDrive, dan Microsoft Teams**, lalu klik **Simpan.**</span><span class="sxs-lookup"><span data-stu-id="419c6-105">Select **Turn on Defender for Office 365 for SharePoint, OneDrive, and Microsoft Teams**, and then click **Save**.</span></span>
4. <span data-ttu-id="419c6-106">(Direkomendasikan) Sebagai administrator global atau administrator SharePoint Online, jalankan cmdlet [Set-SPOTenant](/powershell/module/sharepoint-online/Set-SPOTenant?view=sharepoint-ps) dengan parameter **DisallowInfectedFileDownload** diatur ke *true.*</span><span class="sxs-lookup"><span data-stu-id="419c6-106">(Recommended) As a global administrator or a SharePoint Online administrator, run the [Set-SPOTenant](/powershell/module/sharepoint-online/Set-SPOTenant?view=sharepoint-ps) cmdlet with the **DisallowInfectedFileDownload** parameter set to *true*.</span></span>
5. <span data-ttu-id="419c6-107">(Direkomendasikan) [Setel pemberitahuan untuk](/microsoft-365/security/office-365-security/turn-on-atp-for-spo-odb-and-teams#set-up-alerts-for-detected-files) file yang terdeteksi.</span><span class="sxs-lookup"><span data-stu-id="419c6-107">(Recommended) [Set up alerts](/microsoft-365/security/office-365-security/turn-on-atp-for-spo-odb-and-teams#set-up-alerts-for-detected-files) for detected files.</span></span>

> [!NOTE]
> <span data-ttu-id="419c6-108">Pertahanan Microsoft untuk Office 365 tidak akan memindai setiap file dalam SharePoint Online, OneDrive, atau Microsoft Teams.</span><span class="sxs-lookup"><span data-stu-id="419c6-108">Microsoft Defender for Office 365 will not scan every single file in SharePoint Online, OneDrive, or Microsoft Teams.</span></span> <span data-ttu-id="419c6-109">File dipindai secara asinkron, melalui proses yang menggunakan aktivitas berbagi dan acara tamu, bersama dengan heuristics cerdas dan sinyal ancaman untuk mengidentifikasi file berbahaya.</span><span class="sxs-lookup"><span data-stu-id="419c6-109">Files are scanned asynchronously, through a process that uses sharing and guest activity events, along with smart heuristics and threat signals to identify malicious files.</span></span> <span data-ttu-id="419c6-110">Lihat [Pertahanan Microsoft untuk Office 365, SharePoint, OneDrive, dan Microsoft Teams](/microsoft-365/security/office-365-security/atp-for-spo-odb-and-teams).</span><span class="sxs-lookup"><span data-stu-id="419c6-110">See [Microsoft Defender for Office 365 for SharePoint, OneDrive, and Microsoft Teams](/microsoft-365/security/office-365-security/atp-for-spo-odb-and-teams).</span></span>