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
ms.sourcegitcommit: 251e2e82571fb3bb1fbe3dbf7bfca30e004b3373
ms.translationtype: MT
ms.contentlocale: id-ID
ms.lasthandoff: 03/05/2021
ms.locfileid: "50482607"
---
# <a name="find-the-ip-address-in-audit-log"></a><span data-ttu-id="ff9a3-102">Menemukan alamat IP dalam log audit</span><span class="sxs-lookup"><span data-stu-id="ff9a3-102">Find the IP address in audit log</span></span>

1. <span data-ttu-id="ff9a3-103">Alamat IP yang terkait dengan aktivitas yang dilakukan oleh pengguna atau administrator diperlihatkan dalam log audit.</span><span class="sxs-lookup"><span data-stu-id="ff9a3-103">The IP address that corresponds to an activity performed by a user or administrator is shown in the audit logs.</span></span> <span data-ttu-id="ff9a3-104">Informasi klien juga dicatat.</span><span class="sxs-lookup"><span data-stu-id="ff9a3-104">The client information is also logged.</span></span> <span data-ttu-id="ff9a3-105">Berikut cara mengidentifikasi alamat IP:</span><span class="sxs-lookup"><span data-stu-id="ff9a3-105">Here's how to identify the IP address:</span></span>

1. <span data-ttu-id="ff9a3-106">Masuk ke [pusat kepatuhan & keamanan Office 365](https://go.microsoft.com/fwlink/p/?linkid=2077143).</span><span class="sxs-lookup"><span data-stu-id="ff9a3-106">Go to the [Office 365 Security & Compliance Center](https://go.microsoft.com/fwlink/p/?linkid=2077143).</span></span>
1. <span data-ttu-id="ff9a3-107">Pilih **Cari pencarian**  >  **[log audit](https://go.microsoft.com/fwlink/?linkid=2103759)**.</span><span class="sxs-lookup"><span data-stu-id="ff9a3-107">Select **Search** > **[Audit log search](https://go.microsoft.com/fwlink/?linkid=2103759)**.</span></span>
    > [!NOTE]
    > <span data-ttu-id="ff9a3-108">Jika Anda melihat pemberitahuan bahwa Anda perlu mengaktifkan pengauditan, Lanjutkan dan Aktifkan sekarang.</span><span class="sxs-lookup"><span data-stu-id="ff9a3-108">If you see a notice that you need to turn on auditing, go ahead and turn it on now.</span></span> <span data-ttu-id="ff9a3-109">Jika fitur ini tidak diaktifkan, hasil pencarian tidak akan dapat menarik data dari tanggal sebelumnya.</span><span class="sxs-lookup"><span data-stu-id="ff9a3-109">If this feature isn't enabled, search results won't be able to pull data from previous dates.</span></span>
1. <span data-ttu-id="ff9a3-110">Jika Anda tertarik dengan aktivitas tertentu, pilih dari daftar **aktivitas** ; Jika tidak, secara default, semua aktivitas akan dikembalikan untuk pengguna yang dipilih.</span><span class="sxs-lookup"><span data-stu-id="ff9a3-110">If you're interested in a specific activity, select it from the **Activities** list; otherwise, by default, all activities will be returned for the selected user.</span></span> <span data-ttu-id="ff9a3-111">Perhatikan bahwa aktivitas tertentu mungkin tidak tersedia untuk pilihan dari menu **aktivitas** ; Namun, item audit tersebut akan dikembalikan jika **memperlihatkan hasil untuk semua aktivitas** yang dipilih (pengaturan default).</span><span class="sxs-lookup"><span data-stu-id="ff9a3-111">Note that certain activities might not be available for selection from the **Activities** menu; however, those audit items will be returned if **Show results for all activities** is selected (default setting).</span></span>
1. <span data-ttu-id="ff9a3-112">Tentukan rentang tanggal, dan di bidang **pengguna** , pilih nama pengguna yang ingin Anda selidiki.</span><span class="sxs-lookup"><span data-stu-id="ff9a3-112">Specify the date range, and in the **Users** field, select the username for the user you want to investigate.</span></span>
1. <span data-ttu-id="ff9a3-113">Pilih **pencarian**.</span><span class="sxs-lookup"><span data-stu-id="ff9a3-113">Select **Search**.</span></span> <span data-ttu-id="ff9a3-114">Aktivitas muncul di bawah **hasil**.</span><span class="sxs-lookup"><span data-stu-id="ff9a3-114">The activities appear under **Results**.</span></span> <span data-ttu-id="ff9a3-115">Anda dapat melihat alamat IP untuk setiap aktivitas.</span><span class="sxs-lookup"><span data-stu-id="ff9a3-115">You can see the IP address for each activity.</span></span>
1. <span data-ttu-id="ff9a3-116">Untuk menampilkan detail, pilih aktivitas, lalu pilih **informasi lainnya**.</span><span class="sxs-lookup"><span data-stu-id="ff9a3-116">To view details, select an activity, and then select **More Information**.</span></span>

<span data-ttu-id="ff9a3-117">Untuk mempelajari selengkapnya, lihat mencari [log audit Office 365 untuk memecahkan masalah skenario umum](https://go.microsoft.com/fwlink/?linkid=2103944).</span><span class="sxs-lookup"><span data-stu-id="ff9a3-117">To learn more, see Search the [Office 365 audit log to troubleshoot common scenarios](https://go.microsoft.com/fwlink/?linkid=2103944).</span></span>