---
title: Mengidentifikasi alamat IP dan klien dalam log audit
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
- "1367"
- "3100005"
ms.assetid: ''
ms.openlocfilehash: 295418f3c433df2ba1004f4bec4377c68e6bb155
ms.sourcegitcommit: c6692ce0fa1358ec3529e59ca0ecdfdea4cdc759
ms.translationtype: MT
ms.contentlocale: id-ID
ms.lasthandoff: 09/14/2020
ms.locfileid: "47668313"
---
# <a name="identify-ip-address-and-client-in-audit-logs"></a><span data-ttu-id="ea9fa-102">Mengidentifikasi alamat IP dan klien dalam log audit</span><span class="sxs-lookup"><span data-stu-id="ea9fa-102">Identify IP address and client in audit logs</span></span>

<span data-ttu-id="ea9fa-103">Alamat IP yang terkait dengan aktivitas oleh pengguna atau administrator Microsoft 365 diperlihatkan dalam log audit.</span><span class="sxs-lookup"><span data-stu-id="ea9fa-103">The IP address that corresponds to an activity by a Microsoft 365 user or administrator is shown in the Audit Logs.</span></span> <span data-ttu-id="ea9fa-104">Informasi klien juga dicatat.</span><span class="sxs-lookup"><span data-stu-id="ea9fa-104">The client information is also logged.</span></span> <span data-ttu-id="ea9fa-105">Berikut adalah langkah-langkah untuk mengidentifikasi informasi tersebut</span><span class="sxs-lookup"><span data-stu-id="ea9fa-105">Here are the steps to identifying such information</span></span>

1. <span data-ttu-id="ea9fa-106">Masuk ke [pusat kepatuhan & keamanan Microsoft 365](https://protection.office.com/).</span><span class="sxs-lookup"><span data-stu-id="ea9fa-106">Log in to the [Microsoft 365 Security & Compliance Center](https://protection.office.com/).</span></span>

2. <span data-ttu-id="ea9fa-107">Masuk ke halaman **Search**  >  **pencarian log audit** pencarian.</span><span class="sxs-lookup"><span data-stu-id="ea9fa-107">Go to the **Search** > **Audit log search** page.</span></span>

   <span data-ttu-id="ea9fa-108">Jika Anda tertarik dengan aktivitas tertentu, pilih dari daftar **aktivitas** .</span><span class="sxs-lookup"><span data-stu-id="ea9fa-108">If you're interested in a specific activity, select it from **Activities** list.</span></span> <span data-ttu-id="ea9fa-109">Jika tidak, semua aktivitas akan dikembalikan untuk pengguna yang dipilih (pengaturan default).</span><span class="sxs-lookup"><span data-stu-id="ea9fa-109">If not, all activities will be returned for the selected user (default setting).</span></span>

   <span data-ttu-id="ea9fa-110">**Catatan**: aktivitas tertentu mungkin tidak tersedia di menu **aktivitas** ; Namun, item audit tersebut akan dikembalikan jika **memperlihatkan hasil untuk semua aktivitas** yang dipilih (pengaturan default).</span><span class="sxs-lookup"><span data-stu-id="ea9fa-110">**Note**: Certain activities may not be available in the **Activities** menu; however, those audit items will be returned if **Show Results for all activities** is selected (default setting).</span></span>

3. <span data-ttu-id="ea9fa-111">Tentukan nama pengguna di bidang **pengguna** , pilih rentang tanggal yang sesuai untuk aktivitas tersebut, lalu klik **Cari**.</span><span class="sxs-lookup"><span data-stu-id="ea9fa-111">Specify the username in the **Users** field, select the appropriate date range for the activity, and then click **Search**.</span></span>

<span data-ttu-id="ea9fa-112">Dalam hasil, Anda dapat melihat alamat IP untuk aktivitas tersebut di panel hasil.</span><span class="sxs-lookup"><span data-stu-id="ea9fa-112">In the results, you can see the IP address for that activity in the results pane.</span></span> <span data-ttu-id="ea9fa-113">Pilih catatan audit untuk melihat informasi mendetail dalam Flyout **detail** (misalnya, klien, pengguna yang melakukan tindakan, dsb.).</span><span class="sxs-lookup"><span data-stu-id="ea9fa-113">Select the audit record to see detailed information in the **Details** flyout (for example, Client, User that performed action, etc.).</span></span>

<span data-ttu-id="ea9fa-114">Untuk informasi selengkapnya, lihat [menemukan alamat IP komputer yang digunakan untuk mengakses akun yang dikompromikan](https://docs.microsoft.com/microsoft-365/compliance/auditing-troubleshooting-scenarios#find-the-ip-address-of-the-computer-used-to-access-a-compromised-account).</span><span class="sxs-lookup"><span data-stu-id="ea9fa-114">For more information, see [Finding the IP address of the computer used to access a compromised account](https://docs.microsoft.com/microsoft-365/compliance/auditing-troubleshooting-scenarios#find-the-ip-address-of-the-computer-used-to-access-a-compromised-account).</span></span>
