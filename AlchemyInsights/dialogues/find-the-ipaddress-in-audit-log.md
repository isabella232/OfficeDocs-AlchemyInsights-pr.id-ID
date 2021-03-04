---
title: Menemukan alamat IP dalam log audit
ms.author: v-aiyengar
author: AshaIyengar21
manager: dansimp
ms.date: 02/26/2021
ms.audience: Admin
ms.topic: article
ms.service: o365-administration
ROBOTS: NOINDEX, NOFOLLOW
localization_priority: Normal
ms.collection: Adm_O365
ms.custom:
- "3100005"
- "7327"
ms.openlocfilehash: 7a01aa3cc0d875e6534435f3e8f90a24f2832dc3
ms.sourcegitcommit: f4ba304b92ed01e35273ecda67e9dc3ad9d475c1
ms.translationtype: MT
ms.contentlocale: id-ID
ms.lasthandoff: 03/04/2021
ms.locfileid: "50429508"
---
# <a name="find-the-ip-address-in-audit-log"></a><span data-ttu-id="2b42d-102">Menemukan alamat IP dalam log audit</span><span class="sxs-lookup"><span data-stu-id="2b42d-102">Find the IP address in audit log</span></span>

1. <span data-ttu-id="2b42d-103">Alamat IP yang terkait dengan aktivitas yang dilakukan oleh pengguna atau administrator diperlihatkan dalam log audit.</span><span class="sxs-lookup"><span data-stu-id="2b42d-103">The IP address that corresponds to an activity performed by a user or administrator is shown in the audit logs.</span></span> <span data-ttu-id="2b42d-104">Informasi klien juga dicatat.</span><span class="sxs-lookup"><span data-stu-id="2b42d-104">The client information is also logged.</span></span> <span data-ttu-id="2b42d-105">Berikut cara mengidentifikasi alamat IP:</span><span class="sxs-lookup"><span data-stu-id="2b42d-105">Here's how to identify the IP address:</span></span>

1. <span data-ttu-id="2b42d-106">Masuk ke [pusat kepatuhan & keamanan Office 365](https://go.microsoft.com/fwlink/p/?linkid=2077143).</span><span class="sxs-lookup"><span data-stu-id="2b42d-106">Go to the [Office 365 Security & Compliance Center](https://go.microsoft.com/fwlink/p/?linkid=2077143).</span></span>
1. <span data-ttu-id="2b42d-107">Pilih **Cari pencarian**  >  **[log audit](https://go.microsoft.com/fwlink/?linkid=2103759)**.</span><span class="sxs-lookup"><span data-stu-id="2b42d-107">Select **Search** > **[Audit log search](https://go.microsoft.com/fwlink/?linkid=2103759)**.</span></span>
    > [!NOTE]
    > <span data-ttu-id="2b42d-108">Jika Anda melihat pemberitahuan bahwa Anda perlu mengaktifkan pengauditan, Lanjutkan dan Aktifkan sekarang.</span><span class="sxs-lookup"><span data-stu-id="2b42d-108">If you see a notice that you need to turn on auditing, go ahead and turn it on now.</span></span> <span data-ttu-id="2b42d-109">Jika fitur ini tidak diaktifkan, hasil pencarian tidak akan dapat menarik data dari tanggal sebelumnya.</span><span class="sxs-lookup"><span data-stu-id="2b42d-109">If this feature isn't enabled, search results won't be able to pull data from previous dates.</span></span>
1. <span data-ttu-id="2b42d-110">Jika Anda tertarik dengan aktivitas tertentu, pilih dari daftar **aktivitas** ; Jika tidak, secara default, semua aktivitas akan dikembalikan untuk pengguna yang dipilih.</span><span class="sxs-lookup"><span data-stu-id="2b42d-110">If you're interested in a specific activity, select it from the **Activities** list; otherwise, by default, all activities will be returned for the selected user.</span></span> <span data-ttu-id="2b42d-111">Perhatikan bahwa aktivitas tertentu mungkin tidak tersedia untuk pilihan dari menu **aktivitas** ; Namun, item audit tersebut akan dikembalikan jika **memperlihatkan hasil untuk semua aktivitas** yang dipilih (pengaturan default).</span><span class="sxs-lookup"><span data-stu-id="2b42d-111">Note that certain activities might not be available for selection from the **Activities** menu; however, those audit items will be returned if **Show results for all activities** is selected (default setting).</span></span>
1. <span data-ttu-id="2b42d-112">Tentukan rentang tanggal, dan di bidang **pengguna** , pilih nama pengguna yang ingin Anda selidiki.</span><span class="sxs-lookup"><span data-stu-id="2b42d-112">Specify the date range, and in the **Users** field, select the username for the user you want to investigate.</span></span>
1. <span data-ttu-id="2b42d-113">Pilih **pencarian**.</span><span class="sxs-lookup"><span data-stu-id="2b42d-113">Select **Search**.</span></span> <span data-ttu-id="2b42d-114">Aktivitas muncul di bawah **hasil**.</span><span class="sxs-lookup"><span data-stu-id="2b42d-114">The activities appear under **Results**.</span></span> <span data-ttu-id="2b42d-115">Anda dapat melihat alamat IP untuk setiap aktivitas.</span><span class="sxs-lookup"><span data-stu-id="2b42d-115">You can see the IP address for each activity.</span></span>
1. <span data-ttu-id="2b42d-116">Untuk menampilkan detail, pilih aktivitas, lalu pilih **informasi lainnya**.</span><span class="sxs-lookup"><span data-stu-id="2b42d-116">To view details, select an activity, and then select **More Information**.</span></span>

<span data-ttu-id="2b42d-117">Untuk mempelajari selengkapnya, lihat mencari [log audit Office 365 untuk memecahkan masalah skenario umum](https://go.microsoft.com/fwlink/?linkid=2103944).</span><span class="sxs-lookup"><span data-stu-id="2b42d-117">To learn more, see Search the [Office 365 audit log to troubleshoot common scenarios](https://go.microsoft.com/fwlink/?linkid=2103944).</span></span>