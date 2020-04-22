---
title: Mengidentifikasi aktivitas aturan kotak masuk di log audit
ms.author: chrisda
author: chrisda
manager: dansimp
ms.date: 04/21/2020
ms.audience: ITPro
ms.topic: article
ROBOTS: NOINDEX, NOFOLLOW
localization_priority: Normal
ms.custom:
- "1368"
- "3100005"
ms.assetid: ''
ms.openlocfilehash: f946510539b3d28f2ceeec1546cbffce8bd352fd
ms.sourcegitcommit: 55eff703a17e500681d8fa6a87eb067019ade3cc
ms.translationtype: MT
ms.contentlocale: id-ID
ms.lasthandoff: 04/22/2020
ms.locfileid: "43716427"
---
# <a name="identify-inbox-rule-activity-in-audit-logs"></a><span data-ttu-id="680bc-102">Mengidentifikasi aktivitas aturan kotak masuk di log audit</span><span class="sxs-lookup"><span data-stu-id="680bc-102">Identify inbox rule activity in audit logs</span></span>

<span data-ttu-id="680bc-103">Anda dapat menggunakan pencarian log audit di Microsoft 365 keamanan & Compliance Center untuk melihat peristiwa aturan kotak masuk (membuat, mengubah, dan menghapus aturan kotak masuk).</span><span class="sxs-lookup"><span data-stu-id="680bc-103">You can use audit log search in the Microsoft 365 Security & Compliance Center to view inbox rule events (creating, modifying, and deleting inbox rules).</span></span>

1. <span data-ttu-id="680bc-104">Masuk ke [Microsoft 365 keamanan & Compliance Center](https://protection.office.com/).</span><span class="sxs-lookup"><span data-stu-id="680bc-104">Log in to the [Microsoft 365 Security & Compliance Center](https://protection.office.com/).</span></span>

2. <span data-ttu-id="680bc-105">Buka halaman pencarian **Search** > **log audit** penelusuran.</span><span class="sxs-lookup"><span data-stu-id="680bc-105">Go to the **Search** > **Audit log search** page.</span></span>

3. <span data-ttu-id="680bc-106">Pilih rentang tanggal di kolom tanggal **mulai** dan **tanggal akhir** .</span><span class="sxs-lookup"><span data-stu-id="680bc-106">Select the date range in the **Start date** and **End date** fields.</span></span>

4. <span data-ttu-id="680bc-107">Di bawah **kotak surat Exchange aktivitas**, verifikasi kolom **aktivitas** diatur ke **baru-inboxrule membuat/mengubah/mengaktifkan/menonaktifkan aturan kotak masuk**.</span><span class="sxs-lookup"><span data-stu-id="680bc-107">Under **Exchange Mailbox Activities**, verify the **Activities** field is set to **New-InboxRule Create/modify/enable/disable inbox rule**.</span></span>

5. <span data-ttu-id="680bc-108">Klik **Cari**.</span><span class="sxs-lookup"><span data-stu-id="680bc-108">Click **Search**.</span></span>

<span data-ttu-id="680bc-109">Di hasil, pilih rekaman audit.</span><span class="sxs-lookup"><span data-stu-id="680bc-109">In the results, select an audit record.</span></span> <span data-ttu-id="680bc-110">Dalam Flyout rincian, klik **informasi lebih lanjut**.</span><span class="sxs-lookup"><span data-stu-id="680bc-110">In the details flyout, click **More Information**.</span></span> <span data-ttu-id="680bc-111">Informasi tentang pengaturan aturan kotak masuk ditampilkan di bidang **parameter** .</span><span class="sxs-lookup"><span data-stu-id="680bc-111">Information about the inbox rule settings is displayed in the **Parameters** field.</span></span>

<span data-ttu-id="680bc-112">Untuk informasi lebih lanjut, lihat [menentukan apakah pengguna membuat aturan kotak masuk](https://docs.microsoft.com//office365/securitycompliance/auditing-troubleshooting-scenarios#determining-if-a-user-created-an-inbox-rule)</span><span class="sxs-lookup"><span data-stu-id="680bc-112">For more information, see [Determining if a user created an inbox rule](https://docs.microsoft.com//office365/securitycompliance/auditing-troubleshooting-scenarios#determining-if-a-user-created-an-inbox-rule)</span></span>
