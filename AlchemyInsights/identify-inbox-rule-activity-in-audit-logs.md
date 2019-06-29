---
title: Mengidentifikasi kegiatan aturan kotak masuk di log audit
ms.author: chrisda
author: chrisda
manager: dansimp
ms.date: ''
ms.audience: ITPro
ms.topic: article
ROBOTS: NOINDEX, NOFOLLOW
localization_priority: Normal
ms.custom:
- "1368"
- "3100005"
ms.assetid: ''
ms.openlocfilehash: 51c25897223371a6dcc94c948955107ce74b0e8e
ms.sourcegitcommit: 5fb7a4b28859690020efdea630d03e70cc0e6334
ms.translationtype: MT
ms.contentlocale: id-ID
ms.lasthandoff: 06/28/2019
ms.locfileid: "35383028"
---
# <a name="identify-inbox-rule-activity-in-audit-logs"></a><span data-ttu-id="b09bd-102">Mengidentifikasi kegiatan aturan kotak masuk di log audit</span><span class="sxs-lookup"><span data-stu-id="b09bd-102">Identify inbox rule activity in audit logs</span></span>

<span data-ttu-id="b09bd-103">Anda dapat menggunakan pencarian log audit di & keamanan Compliance Center untuk melihat kotak masuk aturan peristiwa (membuat, memodifikasi, dan menghapus aturan kotak masuk).</span><span class="sxs-lookup"><span data-stu-id="b09bd-103">You can use audit log search in the Security & Compliance Center to view inbox rule events (creating, modifying, and deleting inbox rules).</span></span>

1. <span data-ttu-id="b09bd-104">Masuk ke [Kantor 365 keamanan & Compliance Center](https://protection.office.com/)</span><span class="sxs-lookup"><span data-stu-id="b09bd-104">Log in to the [Office 365 Security & Compliance Center](https://protection.office.com/)</span></span>

2. <span data-ttu-id="b09bd-105">Klik **Cari dan penyelidikan** dan pilih **Cari Log Audit**.</span><span class="sxs-lookup"><span data-stu-id="b09bd-105">Click **Search and Investigation** and select **Audit Log Search**.</span></span>

3. <span data-ttu-id="b09bd-106">Pilih rentang tanggal di bidang **tanggal mulai** dan **tanggal akhir** .</span><span class="sxs-lookup"><span data-stu-id="b09bd-106">Select the date range in the **Start date** and **End date** fields.</span></span>

4. <span data-ttu-id="b09bd-107">Dalam **Kegiatan pertukaran kotak pesan**, pastikan bidang **kegiatan** diatur ke **New-InboxRule buat/memodifikasi/mengaktifkan/menonaktifkan aturan kotak masuk**.</span><span class="sxs-lookup"><span data-stu-id="b09bd-107">Under **Exchange Mailbox Activities**, verify the **Activities** field is set to **New-InboxRule Create/modify/enable/disable inbox rule**.</span></span>

5. <span data-ttu-id="b09bd-108">Klik **Cari**.</span><span class="sxs-lookup"><span data-stu-id="b09bd-108">Click **Search**.</span></span>

<span data-ttu-id="b09bd-109">Hasil, pilih catatan audit.</span><span class="sxs-lookup"><span data-stu-id="b09bd-109">In the results, select an audit record.</span></span> <span data-ttu-id="b09bd-110">Di flyout rincian, klik **Informasi selengkapnya**.</span><span class="sxs-lookup"><span data-stu-id="b09bd-110">In the details flyout, click **More Information**.</span></span> <span data-ttu-id="b09bd-111">Informasi tentang pengaturan aturan kotak masuk akan ditampilkan dalam bidang **parameter** .</span><span class="sxs-lookup"><span data-stu-id="b09bd-111">Information about the inbox rule settings is displayed in the **Parameters** field.</span></span>

<span data-ttu-id="b09bd-112">Untuk informasi lebih lanjut, lihat [menentukan jika pengguna membuat aturan kotak masuk](https://docs.microsoft.com//office365/securitycompliance/auditing-troubleshooting-scenarios#determining-if-a-user-created-an-inbox-rule)</span><span class="sxs-lookup"><span data-stu-id="b09bd-112">For more information, see [Determining if a user created an inbox rule](https://docs.microsoft.com//office365/securitycompliance/auditing-troubleshooting-scenarios#determining-if-a-user-created-an-inbox-rule)</span></span>
