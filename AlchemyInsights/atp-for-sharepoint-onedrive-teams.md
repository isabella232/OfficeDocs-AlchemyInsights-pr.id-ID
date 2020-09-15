---
title: ATP untuk SharePoint, OneDrive, dan Microsoft teams
ms.author: chrisda
author: chrisda
manager: dansimp
ms.date: 04/21/2020
ms.audience: ITPro
ms.topic: article
ms.service: o365-administration
ROBOTS: NOINDEX, NOFOLLOW
localization_priority: Normal
ms.custom: 1037
ms.assetid: ''
ms.openlocfilehash: 3d02ded959114675847831690b4d4a3ebcf0e137
ms.sourcegitcommit: c6692ce0fa1358ec3529e59ca0ecdfdea4cdc759
ms.translationtype: MT
ms.contentlocale: id-ID
ms.lasthandoff: 09/14/2020
ms.locfileid: "47715564"
---
# <a name="atp-for-sharepoint-onedrive-and-microsoft-teams"></a><span data-ttu-id="1ea5a-102">ATP untuk SharePoint, OneDrive, dan Microsoft teams</span><span class="sxs-lookup"><span data-stu-id="1ea5a-102">ATP for SharePoint, OneDrive, and Microsoft Teams</span></span>

<span data-ttu-id="1ea5a-103">Ikuti langkah-langkah ini untuk mengaktifkan proteksi ancaman tingkat lanjut:</span><span class="sxs-lookup"><span data-stu-id="1ea5a-103">Follow these steps to enable Advanced Threat Protection:</span></span>

1. <span data-ttu-id="1ea5a-104">Masuk ke [https://protection.office.com](https://protection.office.com) dan masuk dengan akun administrator global atau administrator keamanan.</span><span class="sxs-lookup"><span data-stu-id="1ea5a-104">Go to [https://protection.office.com](https://protection.office.com) and sign in with a global administrator or security administrator account.</span></span>

2. <span data-ttu-id="1ea5a-105">Di panel navigasi kiri di bawah **manajemen ancaman**, pilih **Policy** \> **lampiran aman**kebijakan.</span><span class="sxs-lookup"><span data-stu-id="1ea5a-105">In the left navigation pane under **Threat management**, choose **Policy** \> **Safe Attachments**.</span></span>

3. <span data-ttu-id="1ea5a-106">Pilih **Aktifkan ATP untuk SharePoint, OneDrive, dan Microsoft teams**.</span><span class="sxs-lookup"><span data-stu-id="1ea5a-106">Select **Turn on ATP for SharePoint, OneDrive, and Microsoft Teams**.</span></span>

4. <span data-ttu-id="1ea5a-107">[Membuat kebijakan pemberitahuan aktivitas](https://docs.microsoft.com/microsoft-365/compliance/create-activity-alerts) untuk menerima pemberitahuan ketika kami mendeteksi file berbahaya.</span><span class="sxs-lookup"><span data-stu-id="1ea5a-107">[Create an activity alert policy](https://docs.microsoft.com/microsoft-365/compliance/create-activity-alerts) to receive notifications when we detect malicious files.</span></span>

<span data-ttu-id="1ea5a-108">Untuk instruksi lengkap, lihat [topik](https://docs.microsoft.com/microsoft-365/security/office-365-security/turn-on-atp-for-spo-odb-and-teams)ini.</span><span class="sxs-lookup"><span data-stu-id="1ea5a-108">For complete instructions, see this [topic](https://docs.microsoft.com/microsoft-365/security/office-365-security/turn-on-atp-for-spo-odb-and-teams).</span></span>

<span data-ttu-id="1ea5a-109">**Catatan**: berdasarkan desain, ATP tidak memindai setiap file di SharePoint online, OneDrive for Business, atau Microsoft teams.</span><span class="sxs-lookup"><span data-stu-id="1ea5a-109">**Note**: By design, ATP doesn't scan every single file in SharePoint Online, OneDrive for Business, or Microsoft Teams.</span></span> <span data-ttu-id="1ea5a-110">File dipindai secara asinkron dengan proses yang menggunakan aktivitas berbagi, aktivitas tamu, dan sinyal ancaman untuk mengidentifikasi file berbahaya.</span><span class="sxs-lookup"><span data-stu-id="1ea5a-110">Files are scanned asynchronously by a process that uses sharing activity, guest activity, and threat signals to identify malicious files.</span></span> <span data-ttu-id="1ea5a-111">Untuk informasi selengkapnya, lihat [topik](https://docs.microsoft.com/microsoft-365/security/office-365-security/atp-for-spo-odb-and-teams)ini.</span><span class="sxs-lookup"><span data-stu-id="1ea5a-111">For more information, see this [topic](https://docs.microsoft.com/microsoft-365/security/office-365-security/atp-for-spo-odb-and-teams).</span></span>
