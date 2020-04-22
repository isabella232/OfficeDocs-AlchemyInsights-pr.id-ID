---
title: Mengidentifikasi alamat IP dan klien dalam log audit
ms.author: chrisda
author: chrisda
manager: dansimp
ms.date: 04/21/2020
ms.audience: ITPro
ms.topic: article
ROBOTS: NOINDEX, NOFOLLOW
localization_priority: Normal
ms.custom:
- "1367"
- "3100005"
ms.assetid: ''
ms.openlocfilehash: d1a0d412fc0c6d79e50b101ca759127522f45dcd
ms.sourcegitcommit: 55eff703a17e500681d8fa6a87eb067019ade3cc
ms.translationtype: MT
ms.contentlocale: id-ID
ms.lasthandoff: 04/22/2020
ms.locfileid: "43716391"
---
# <a name="identify-ip-address-and-client-in-audit-logs"></a><span data-ttu-id="2d8ce-102">Mengidentifikasi alamat IP dan klien dalam log audit</span><span class="sxs-lookup"><span data-stu-id="2d8ce-102">Identify IP address and client in audit logs</span></span>

<span data-ttu-id="2d8ce-103">Alamat IP yang berkaitan dengan aktivitas oleh pengguna 365 Microsoft atau administrator ditampilkan di log audit.</span><span class="sxs-lookup"><span data-stu-id="2d8ce-103">The IP address that corresponds to an activity by a Microsoft 365 user or administrator is shown in the Audit Logs.</span></span> <span data-ttu-id="2d8ce-104">Informasi klien juga dicatat.</span><span class="sxs-lookup"><span data-stu-id="2d8ce-104">The client information is also logged.</span></span> <span data-ttu-id="2d8ce-105">Berikut adalah langkah untuk mengidentifikasi informasi tersebut</span><span class="sxs-lookup"><span data-stu-id="2d8ce-105">Here are the steps to identifying such information</span></span>

1. <span data-ttu-id="2d8ce-106">Masuk ke [Microsoft 365 keamanan & Compliance Center](https://protection.office.com/).</span><span class="sxs-lookup"><span data-stu-id="2d8ce-106">Log in to the [Microsoft 365 Security & Compliance Center](https://protection.office.com/).</span></span>

2. <span data-ttu-id="2d8ce-107">Buka halaman pencarian **Search** > **log audit** penelusuran.</span><span class="sxs-lookup"><span data-stu-id="2d8ce-107">Go to the **Search** > **Audit log search** page.</span></span>

   <span data-ttu-id="2d8ce-108">Jika Anda tertarik dengan aktivitas tertentu, pilih dari daftar **aktivitas** .</span><span class="sxs-lookup"><span data-stu-id="2d8ce-108">If you're interested in a specific activity, select it from **Activities** list.</span></span> <span data-ttu-id="2d8ce-109">Jika tidak, semua aktivitas akan dikembalikan untuk pengguna yang dipilih (setelan default).</span><span class="sxs-lookup"><span data-stu-id="2d8ce-109">If not, all activities will be returned for the selected user (default setting).</span></span>

   <span data-ttu-id="2d8ce-110">**Catatan**: aktivitas tertentu mungkin tidak tersedia di menu **aktivitas** ; Namun, item audit tersebut akan dikembalikan jika **Tampilkan hasil untuk semua aktivitas** dipilih (pengaturan default).</span><span class="sxs-lookup"><span data-stu-id="2d8ce-110">**Note**: Certain activities may not be available in the **Activities** menu; however, those audit items will be returned if **Show Results for all activities** is selected (default setting).</span></span>

3. <span data-ttu-id="2d8ce-111">Tentukan nama pengguna di bidang **pengguna** , pilih rentang tanggal yang sesuai untuk aktivitas, dan kemudian klik **Cari**.</span><span class="sxs-lookup"><span data-stu-id="2d8ce-111">Specify the username in the **Users** field, select the appropriate date range for the activity, and then click **Search**.</span></span>

<span data-ttu-id="2d8ce-112">Pada hasil, Anda dapat melihat alamat IP untuk aktivitas tersebut di panel hasil.</span><span class="sxs-lookup"><span data-stu-id="2d8ce-112">In the results, you can see the IP address for that activity in the results pane.</span></span> <span data-ttu-id="2d8ce-113">Pilih rekaman audit untuk melihat informasi terperinci dalam Flyout **rincian** (misalnya, klien, pengguna yang melakukan tindakan, dsb.).</span><span class="sxs-lookup"><span data-stu-id="2d8ce-113">Select the audit record to see detailed information in the **Details** flyout (for example, Client, User that performed action, etc.).</span></span>

<span data-ttu-id="2d8ce-114">Untuk informasi lebih lanjut, lihat [menemukan alamat IP komputer yang digunakan untuk mengakses akun yang disusupi](https://docs.microsoft.com/office365/securitycompliance/auditing-troubleshooting-scenarios#finding-the-ip-address-of-the-computer-used-to-access-a-compromised-account).</span><span class="sxs-lookup"><span data-stu-id="2d8ce-114">For more information, see [Finding the IP address of the computer used to access a compromised account](https://docs.microsoft.com/office365/securitycompliance/auditing-troubleshooting-scenarios#finding-the-ip-address-of-the-computer-used-to-access-a-compromised-account).</span></span>
