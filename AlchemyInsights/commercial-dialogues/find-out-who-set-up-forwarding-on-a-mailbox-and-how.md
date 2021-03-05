---
title: Mencari tahu siapa yang menyetel penerusan pada kotak surat, dan caranya
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
ms.openlocfilehash: 6a1a1376758024339939d10a7d17520faa8505ea
ms.sourcegitcommit: 251e2e82571fb3bb1fbe3dbf7bfca30e004b3373
ms.translationtype: MT
ms.contentlocale: id-ID
ms.lasthandoff: 03/05/2021
ms.locfileid: "50482300"
---
# <a name="find-out-who-set-up-forwarding-on-a-mailbox-and-how"></a><span data-ttu-id="991e3-102">Mencari tahu siapa yang menyetel penerusan pada kotak surat, dan caranya</span><span class="sxs-lookup"><span data-stu-id="991e3-102">Find out who set up forwarding on a mailbox, and how</span></span>

<span data-ttu-id="991e3-103">Jika penerusan eksternal diatur di kotak surat, aktivitas diaudit sebagai bagian dari cmdlet Set-Mailbox.</span><span class="sxs-lookup"><span data-stu-id="991e3-103">If external forwarding was set on a mailbox, the activity is audited as part of the Set-Mailbox cmdlet.</span></span> <span data-ttu-id="991e3-104">Berikut cara menemukan aktivitas dalam log audit:</span><span class="sxs-lookup"><span data-stu-id="991e3-104">Here's how to find the activity in the audit log:</span></span>

1. <span data-ttu-id="991e3-105">Masuk ke [pusat kepatuhan & keamanan Office 365](https://go.microsoft.com/fwlink/p/?linkid=2077143).</span><span class="sxs-lookup"><span data-stu-id="991e3-105">Go to the [Office 365 Security & Compliance Center](https://go.microsoft.com/fwlink/p/?linkid=2077143).</span></span>
1. <span data-ttu-id="991e3-106">Pilih **Cari pencarian** >  **log audit**.</span><span class="sxs-lookup"><span data-stu-id="991e3-106">Select **Search**> **Audit log search**.</span></span>
    > [!NOTE]
    > <span data-ttu-id="991e3-107">Jika Anda melihat pemberitahuan bahwa Anda perlu mengaktifkan pengauditan, Lanjutkan dan Aktifkan sekarang.</span><span class="sxs-lookup"><span data-stu-id="991e3-107">If you see a notice that you need to turn on auditing, go ahead and turn it on now.</span></span> <span data-ttu-id="991e3-108">Jika fitur ini tidak diaktifkan, hasil pencarian tidak akan dapat menarik data dari tanggal sebelumnya.</span><span class="sxs-lookup"><span data-stu-id="991e3-108">If this feature isn't turned on, search results won't be able to pull data from previous dates.</span></span>
1. <span data-ttu-id="991e3-109">Pastikan bidang **aktivitas** diatur untuk **memperlihatkan hasil untuk semua aktivitas** (default).</span><span class="sxs-lookup"><span data-stu-id="991e3-109">Make sure the **Activities** field is set to **Show results for all activities** (the default).</span></span> <span data-ttu-id="991e3-110">Menentukan rentang tanggal.</span><span class="sxs-lookup"><span data-stu-id="991e3-110">Specify the date range.</span></span> <span data-ttu-id="991e3-111">Anda tidak perlu menentukan nama pengguna.</span><span class="sxs-lookup"><span data-stu-id="991e3-111">You don't need to specify a username.</span></span>
1. <span data-ttu-id="991e3-112">Pilih **pencarian**.</span><span class="sxs-lookup"><span data-stu-id="991e3-112">Select **Search**.</span></span> <span data-ttu-id="991e3-113">Aktivitas muncul di bawah **hasil**.</span><span class="sxs-lookup"><span data-stu-id="991e3-113">The activities appear under **Results**.</span></span>
1. <span data-ttu-id="991e3-114">Pilih **filter hasil**, lalu masukkan **set-kotak surat** di bidang filter **aktivitas** .</span><span class="sxs-lookup"><span data-stu-id="991e3-114">Select **Filter Results**, and then enter **Set-mailbox** in the **Activity** filter field.</span></span> <span data-ttu-id="991e3-115">Ini mengembalikan semua aktivitas **kumpulan-kotak surat** .</span><span class="sxs-lookup"><span data-stu-id="991e3-115">This returns all **Set-Mailbox** activities.</span></span>
1. <span data-ttu-id="991e3-116">Untuk menampilkan detail, pilih aktivitas, lalu pilih **informasi lainnya**.</span><span class="sxs-lookup"><span data-stu-id="991e3-116">To view the details, select an activity, and then select **More Information**.</span></span> <span data-ttu-id="991e3-117">Di bawah **parameter** Anda dapat melihat alamat email penerusan yang diatur di kotak surat.</span><span class="sxs-lookup"><span data-stu-id="991e3-117">Under **Parameters** you can see the forwarding email address that was set on the mailbox.</span></span> <span data-ttu-id="991e3-118">**Userid** mewakili pengguna yang menyetel penerusan eksternal pada kotak surat.</span><span class="sxs-lookup"><span data-stu-id="991e3-118">The **UserID** represents the user who set up external forwarding on the mailbox.</span></span>
<span data-ttu-id="991e3-119">Untuk mempelajari selengkapnya, lihat [mencari log audit Office 365 untuk memecahkan masalah skenario umum](https://go.microsoft.com/fwlink/?linkid=2103944).</span><span class="sxs-lookup"><span data-stu-id="991e3-119">To learn more, see [Search the Office 365 audit log to troubleshoot common scenarios](https://go.microsoft.com/fwlink/?linkid=2103944).</span></span>