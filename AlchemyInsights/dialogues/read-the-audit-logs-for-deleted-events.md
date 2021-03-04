---
title: Membaca log audit untuk acara yang dihapus
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
ms.openlocfilehash: 9739fb1eb8e4f5adf81cd699c851a51176f0429e
ms.sourcegitcommit: f4ba304b92ed01e35273ecda67e9dc3ad9d475c1
ms.translationtype: MT
ms.contentlocale: id-ID
ms.lasthandoff: 03/04/2021
ms.locfileid: "50429521"
---
# <a name="read-the-audit-logs-for-deleted-events"></a><span data-ttu-id="b39a9-102">Membaca log audit untuk acara yang dihapus</span><span class="sxs-lookup"><span data-stu-id="b39a9-102">Read the audit logs for deleted events</span></span>

<span data-ttu-id="b39a9-103">Berikut ini cara melakukan ini:</span><span class="sxs-lookup"><span data-stu-id="b39a9-103">Here's how to do this:</span></span>

1. <span data-ttu-id="b39a9-104">Masuk ke [pusat kepatuhan & keamanan Office 365](https://go.microsoft.com/fwlink/p/?linkid=2077143).</span><span class="sxs-lookup"><span data-stu-id="b39a9-104">Go to the [Office 365 Security & Compliance Center](https://go.microsoft.com/fwlink/p/?linkid=2077143).</span></span>
1. <span data-ttu-id="b39a9-105">Pilih **Cari pencarian**  >  [**log audit**](https://go.microsoft.com/fwlink/?linkid=2103759).</span><span class="sxs-lookup"><span data-stu-id="b39a9-105">Select **Search** > [**Audit log search**](https://go.microsoft.com/fwlink/?linkid=2103759).</span></span>
    > [!NOTE]
    > <span data-ttu-id="b39a9-106">Jika Anda melihat pemberitahuan bahwa Anda perlu mengaktifkan fitur tersebut, Lanjutkan dan Aktifkan sekarang.</span><span class="sxs-lookup"><span data-stu-id="b39a9-106">If you see a notice that you need to turn on the feature, go ahead and turn it on now.</span></span> <span data-ttu-id="b39a9-107">Jika fitur tidak diaktifkan, hasil pencarian tidak akan dapat menarik data dari tanggal sebelumnya.</span><span class="sxs-lookup"><span data-stu-id="b39a9-107">If the feature isn't turned on, search results won't be able to pull data from previous dates.</span></span>
1. <span data-ttu-id="b39a9-108">Pilih **aktivitas**, lalu temukan **aktivitas kotak surat Exchange**.</span><span class="sxs-lookup"><span data-stu-id="b39a9-108">Select **Activities**, and then find **Exchange mailbox activities**.</span></span> <span data-ttu-id="b39a9-109">Pilih opsi Hapus **pesan dari folder Item terhapus** dan **Pindahkan pesan ke folder Item terhapus** .</span><span class="sxs-lookup"><span data-stu-id="b39a9-109">Select the **Deleted messages from Deleted Items** folder and **Moved messages to Deleted Items** folder options.</span></span> <span data-ttu-id="b39a9-110">Bila sudah selesai, klik di luar panel untuk meminimalkan panel **aktivitas** .</span><span class="sxs-lookup"><span data-stu-id="b39a9-110">When you're done, click outside of the pane to minimize the **Activities** pane.</span></span>
1. <span data-ttu-id="b39a9-111">Tentukan rentang tanggal, lalu di kotak **pengguna** , pilih nama pengguna yang ingin Anda selidiki.</span><span class="sxs-lookup"><span data-stu-id="b39a9-111">Specify the date range, and then in the **Users** box, select the username for the user you want to investigate.</span></span> <span data-ttu-id="b39a9-112">Anda dapat memilih lebih dari satu pengguna dalam satu waktu.</span><span class="sxs-lookup"><span data-stu-id="b39a9-112">You can select more than one user at a time.</span></span>
1. <span data-ttu-id="b39a9-113">Pilih **pencarian**.</span><span class="sxs-lookup"><span data-stu-id="b39a9-113">Select **Search**.</span></span> <span data-ttu-id="b39a9-114">Aktivitas muncul di bawah **hasil**.</span><span class="sxs-lookup"><span data-stu-id="b39a9-114">The activities appear under **Results**.</span></span>
1. <span data-ttu-id="b39a9-115">Untuk menampilkan detail, pilih aktivitas, lalu pilih **informasi lainnya**.</span><span class="sxs-lookup"><span data-stu-id="b39a9-115">To view the details, select an activity, and then select **More Information**.</span></span> <span data-ttu-id="b39a9-116">Informasi tambahan tentang item terhapus, seperti baris subjek dan lokasi item saat dihapus, ditampilkan di bidang **Affecteditems** .</span><span class="sxs-lookup"><span data-stu-id="b39a9-116">Additional information about the deleted item, such as the subject line and the location of the item when it was deleted, is displayed in the **AffectedItems** field.</span></span>
    > [!NOTE]
    > <span data-ttu-id="b39a9-117">Anda tidak bisa memulihkan item terhapus menggunakan fitur log audit.</span><span class="sxs-lookup"><span data-stu-id="b39a9-117">You can't restore deleted items using the audit log feature.</span></span> <span data-ttu-id="b39a9-118">Untuk memulihkan item yang dihapus, lihat [memulihkan item atau email terhapus di Outlook Web App](https://go.microsoft.com/fwlink/?linkid=2103759).</span><span class="sxs-lookup"><span data-stu-id="b39a9-118">To restore deleted items, see [Recover deleted items or email in Outlook Web App](https://go.microsoft.com/fwlink/?linkid=2103759).</span></span>

<span data-ttu-id="b39a9-119">Untuk mempelajari selengkapnya, lihat [mencari log audit Office 365 untuk memecahkan masalah skenario umum](https://go.microsoft.com/fwlink/?linkid=2103944).</span><span class="sxs-lookup"><span data-stu-id="b39a9-119">To learn more, see [Search the Office 365 audit log to troubleshoot common scenarios](https://go.microsoft.com/fwlink/?linkid=2103944).</span></span>
