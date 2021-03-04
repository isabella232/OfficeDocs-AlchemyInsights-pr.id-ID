---
title: Menemukan acara yang dilakukan pada aturan kotak masuk
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
ms.openlocfilehash: deb83d278a2b398b4ea6fc31b043c33309b736e3
ms.sourcegitcommit: f4ba304b92ed01e35273ecda67e9dc3ad9d475c1
ms.translationtype: MT
ms.contentlocale: id-ID
ms.lasthandoff: 03/04/2021
ms.locfileid: "50429628"
---
# <a name="find-events-performed-on-inbox-rules"></a><span data-ttu-id="2939a-102">Menemukan acara yang dilakukan pada aturan kotak masuk</span><span class="sxs-lookup"><span data-stu-id="2939a-102">Find events performed on inbox rules</span></span>

<span data-ttu-id="2939a-103">Saat aturan kotak masuk dibuat, diubah, atau dihapus, kejadian dicatat dalam log audit.</span><span class="sxs-lookup"><span data-stu-id="2939a-103">When inbox rules are created, changed, or deleted, the events are recorded in the audit log.</span></span> <span data-ttu-id="2939a-104">Berikut ini cara untuk meninjau mereka:</span><span class="sxs-lookup"><span data-stu-id="2939a-104">Here's how to review them:</span></span>

1. <span data-ttu-id="2939a-105">Masuk ke [pusat kepatuhan & keamanan Office 365](https://go.microsoft.com/fwlink/p/?linkid=2077143).</span><span class="sxs-lookup"><span data-stu-id="2939a-105">Go to the [Office 365 Security & Compliance Center](https://go.microsoft.com/fwlink/p/?linkid=2077143).</span></span>
1. <span data-ttu-id="2939a-106">Pilih pencarian > pencarian log audit.</span><span class="sxs-lookup"><span data-stu-id="2939a-106">Select Search > Audit log search.</span></span>

    > [!NOTE]
    > <span data-ttu-id="2939a-107">Jika Anda melihat pemberitahuan bahwa Anda perlu mengaktifkan pengauditan, Lanjutkan dan Aktifkan sekarang.</span><span class="sxs-lookup"><span data-stu-id="2939a-107">If you see a notice that you need to turn on auditing, go ahead and turn it on now.</span></span> <span data-ttu-id="2939a-108">Jika fitur ini tidak diaktifkan, hasil pencarian tidak akan dapat menarik data dari tanggal sebelumnya.</span><span class="sxs-lookup"><span data-stu-id="2939a-108">If this feature isn't turned on, search results won't be able to pull data from previous dates.</span></span>
1. <span data-ttu-id="2939a-109">Pilih bidang aktivitas dan temukan aktivitas kotak surat Exchange, lalu pilih New-InboxRule Buat aturan kotak masuk dari Outlook Web App.</span><span class="sxs-lookup"><span data-stu-id="2939a-109">Select the Activities field and find Exchange mailbox activities, and then select New-InboxRule Create inbox rule from Outlook Web App.</span></span> <span data-ttu-id="2939a-110">Bila sudah selesai, klik di luar panel untuk meminimalkan panel aktivitas.</span><span class="sxs-lookup"><span data-stu-id="2939a-110">When you're done, click outside of the pane to minimize the Activities pane.</span></span>
1. <span data-ttu-id="2939a-111">Tentukan rentang tanggal, lalu di bidang pengguna, pilih nama pengguna yang ingin Anda selidiki.</span><span class="sxs-lookup"><span data-stu-id="2939a-111">Specify the date range, and then in the Users field, select the username for the user you want to investigate.</span></span> <span data-ttu-id="2939a-112">Anda dapat memilih lebih dari satu pengguna dalam satu waktu.</span><span class="sxs-lookup"><span data-stu-id="2939a-112">You can select more than one user at a time.</span></span>
1. <span data-ttu-id="2939a-113">Pilih pencarian.</span><span class="sxs-lookup"><span data-stu-id="2939a-113">Select Search.</span></span> <span data-ttu-id="2939a-114">Aktivitas muncul di bawah hasil.</span><span class="sxs-lookup"><span data-stu-id="2939a-114">The activities appear under Results.</span></span>
1. <span data-ttu-id="2939a-115">Untuk menampilkan detail, pilih aktivitas, lalu pilih informasi lainnya.</span><span class="sxs-lookup"><span data-stu-id="2939a-115">To view details, select an activity, and then select More Information.</span></span> <span data-ttu-id="2939a-116">Di bawah bagian parameter, Anda bisa melihat nama aturan, ketentuan yang ditetapkan, dan tindakan yang akan diambil oleh aturan tersebut.</span><span class="sxs-lookup"><span data-stu-id="2939a-116">Under the Parameters section you can see the name of the rule, conditions set, and the actions that the rule will take.</span></span>

<span data-ttu-id="2939a-117">Untuk mempelajari selengkapnya, lihat mencari log audit Office 365 untuk memecahkan masalah skenario umum.</span><span class="sxs-lookup"><span data-stu-id="2939a-117">To learn more, see Search the Office 365 audit log to troubleshoot common scenarios.</span></span>