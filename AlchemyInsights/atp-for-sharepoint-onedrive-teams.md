---
title: ATP untuk SharePoint, OneDrive, dan Microsoft teams
ms.author: chrisda
author: chrisda
manager: dansimp
ms.date: 04/21/2020
ms.audience: ITPro
ms.topic: article
ROBOTS: NOINDEX, NOFOLLOW
localization_priority: Normal
ms.custom: 1037
ms.assetid: ''
ms.openlocfilehash: 28046c61e1aedbb2c07cca3fc01b118d0dc3c143
ms.sourcegitcommit: 55eff703a17e500681d8fa6a87eb067019ade3cc
ms.translationtype: MT
ms.contentlocale: id-ID
ms.lasthandoff: 04/22/2020
ms.locfileid: "43712461"
---
# <a name="atp-for-sharepoint-onedrive-and-microsoft-teams"></a><span data-ttu-id="ca612-102">ATP untuk SharePoint, OneDrive, dan Microsoft teams</span><span class="sxs-lookup"><span data-stu-id="ca612-102">ATP for SharePoint, OneDrive, and Microsoft Teams</span></span>

<span data-ttu-id="ca612-103">Ikuti langkah berikut untuk mengaktifkan perlindungan ancaman lanjutan:</span><span class="sxs-lookup"><span data-stu-id="ca612-103">Follow these steps to enable Advanced Threat Protection:</span></span>

1. <span data-ttu-id="ca612-104">Buka [https://protection.office.com](https://protection.office.com) dan masuk dengan administrator global atau akun administrator keamanan.</span><span class="sxs-lookup"><span data-stu-id="ca612-104">Go to [https://protection.office.com](https://protection.office.com) and sign in with a global administrator or security administrator account.</span></span>

2. <span data-ttu-id="ca612-105">Di panel navigasi kiri di bawah **manajemen ancaman**, pilih **kebijakan** \> **lampiran aman**.</span><span class="sxs-lookup"><span data-stu-id="ca612-105">In the left navigation pane under **Threat management**, choose **Policy** \> **Safe Attachments**.</span></span>

3. <span data-ttu-id="ca612-106">Pilih **Aktifkan ATP untuk SharePoint, OneDrive, dan Microsoft teams**.</span><span class="sxs-lookup"><span data-stu-id="ca612-106">Select **Turn on ATP for SharePoint, OneDrive, and Microsoft Teams**.</span></span>

4. <span data-ttu-id="ca612-107">[Membuat kebijakan peringatan aktivitas](https://docs.microsoft.com/office365/securitycompliance/create-activity-alerts) untuk menerima pemberitahuan saat kami mendeteksi file berbahaya.</span><span class="sxs-lookup"><span data-stu-id="ca612-107">[Create an activity alert policy](https://docs.microsoft.com/office365/securitycompliance/create-activity-alerts) to receive notifications when we detect malicious files.</span></span>

<span data-ttu-id="ca612-108">Untuk petunjuk lengkap, lihat [topik](https://docs.microsoft.com/office365/securitycompliance/turn-on-atp-for-spo-odb-and-teams)ini.</span><span class="sxs-lookup"><span data-stu-id="ca612-108">For complete instructions, see this [topic](https://docs.microsoft.com/office365/securitycompliance/turn-on-atp-for-spo-odb-and-teams).</span></span>

<span data-ttu-id="ca612-109">**Catatan**: Desain, ATP tidak memindai setiap file di SharePoint online, OneDrive untuk bisnis, atau Microsoft teams.</span><span class="sxs-lookup"><span data-stu-id="ca612-109">**Note**: By design, ATP doesn't scan every single file in SharePoint Online, OneDrive for Business, or Microsoft Teams.</span></span> <span data-ttu-id="ca612-110">File dipindai secara asinkron oleh proses yang menggunakan aktivitas berbagi, aktivitas tamu, dan sinyal ancaman untuk mengidentifikasi file berbahaya.</span><span class="sxs-lookup"><span data-stu-id="ca612-110">Files are scanned asynchronously by a process that uses sharing activity, guest activity, and threat signals to identify malicious files.</span></span> <span data-ttu-id="ca612-111">Untuk informasi lebih lanjut, lihat [topik](https://docs.microsoft.com/office365/securitycompliance/atp-for-spo-odb-and-teams)ini.</span><span class="sxs-lookup"><span data-stu-id="ca612-111">For more information, see this [topic](https://docs.microsoft.com/office365/securitycompliance/atp-for-spo-odb-and-teams).</span></span>
