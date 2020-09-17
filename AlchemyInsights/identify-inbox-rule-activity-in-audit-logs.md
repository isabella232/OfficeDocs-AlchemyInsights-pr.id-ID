---
title: Mengidentifikasi aktivitas aturan kotak masuk dalam log audit
ms.author: chrisda
author: chrisda
manager: dansimp
ms.date: 04/21/2020
ms.audience: ITPro
ms.topic: article
ms.service: o365-administration
ROBOTS: NOINDEX, NOFOLLOW
localization_priority: Normal
ms.custom:
- "1368"
- "3100005"
ms.assetid: ''
ms.openlocfilehash: 3de6fcde6dc649cb77077d469cc66d4003e0c890
ms.sourcegitcommit: c6692ce0fa1358ec3529e59ca0ecdfdea4cdc759
ms.translationtype: MT
ms.contentlocale: id-ID
ms.lasthandoff: 09/15/2020
ms.locfileid: "47779054"
---
# <a name="identify-inbox-rule-activity-in-audit-logs"></a><span data-ttu-id="0d5dd-102">Mengidentifikasi aktivitas aturan kotak masuk dalam log audit</span><span class="sxs-lookup"><span data-stu-id="0d5dd-102">Identify inbox rule activity in audit logs</span></span>

<span data-ttu-id="0d5dd-103">Anda dapat menggunakan pencarian log audit di pusat kepatuhan & keamanan Microsoft 365 untuk menampilkan kejadian aturan kotak masuk (membuat, mengubah, dan menghapus aturan kotak masuk).</span><span class="sxs-lookup"><span data-stu-id="0d5dd-103">You can use audit log search in the Microsoft 365 Security & Compliance Center to view inbox rule events (creating, modifying, and deleting inbox rules).</span></span>

1. <span data-ttu-id="0d5dd-104">Masuk ke [pusat kepatuhan & keamanan Microsoft 365](https://protection.office.com/).</span><span class="sxs-lookup"><span data-stu-id="0d5dd-104">Log in to the [Microsoft 365 Security & Compliance Center](https://protection.office.com/).</span></span>

2. <span data-ttu-id="0d5dd-105">Masuk ke halaman **Search**  >  **pencarian log audit** pencarian.</span><span class="sxs-lookup"><span data-stu-id="0d5dd-105">Go to the **Search** > **Audit log search** page.</span></span>

3. <span data-ttu-id="0d5dd-106">Pilih rentang tanggal di bidang tanggal **mulai** dan **tanggal berakhir** .</span><span class="sxs-lookup"><span data-stu-id="0d5dd-106">Select the date range in the **Start date** and **End date** fields.</span></span>

4. <span data-ttu-id="0d5dd-107">Di bawah **aktivitas kotak surat Exchange**, verifikasi bidang **aktivitas** diatur ke **aturan kotak masuk baru membuat/mengubah/mengaktifkan/menonaktifkan kotak masuk**.</span><span class="sxs-lookup"><span data-stu-id="0d5dd-107">Under **Exchange Mailbox Activities**, verify the **Activities** field is set to **New-InboxRule Create/modify/enable/disable inbox rule**.</span></span>

5. <span data-ttu-id="0d5dd-108">Klik **Cari**.</span><span class="sxs-lookup"><span data-stu-id="0d5dd-108">Click **Search**.</span></span>

<span data-ttu-id="0d5dd-109">Dalam hasil, pilih catatan audit.</span><span class="sxs-lookup"><span data-stu-id="0d5dd-109">In the results, select an audit record.</span></span> <span data-ttu-id="0d5dd-110">Dalam Flyout detail, klik **informasi selengkapnya**.</span><span class="sxs-lookup"><span data-stu-id="0d5dd-110">In the details flyout, click **More Information**.</span></span> <span data-ttu-id="0d5dd-111">Informasi tentang pengaturan aturan kotak masuk ditampilkan dalam bidang **parameter** .</span><span class="sxs-lookup"><span data-stu-id="0d5dd-111">Information about the inbox rule settings is displayed in the **Parameters** field.</span></span>

<span data-ttu-id="0d5dd-112">Untuk informasi selengkapnya, lihat [menentukan apakah pengguna membuat aturan kotak masuk](https://docs.microsoft.com//office365/securitycompliance/auditing-troubleshooting-scenarios#determining-if-a-user-created-an-inbox-rule)</span><span class="sxs-lookup"><span data-stu-id="0d5dd-112">For more information, see [Determining if a user created an inbox rule](https://docs.microsoft.com//office365/securitycompliance/auditing-troubleshooting-scenarios#determining-if-a-user-created-an-inbox-rule)</span></span>
