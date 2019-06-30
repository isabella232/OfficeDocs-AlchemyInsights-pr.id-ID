---
title: Mengidentifikasi Hapus pesan peristiwa di log audit
ms.author: chrisda
author: chrisda
manager: dansimp
ms.date: ''
ms.audience: ITPro
ms.topic: article
ROBOTS: NOINDEX, NOFOLLOW
localization_priority: Normal
ms.custom:
- "1370"
- "3100005"
ms.assetid: ''
ms.openlocfilehash: 89877331d328d798177fab3150d5219c5b484a70
ms.sourcegitcommit: 5fb7a4b28859690020efdea630d03e70cc0e6334
ms.translationtype: MT
ms.contentlocale: id-ID
ms.lasthandoff: 06/28/2019
ms.locfileid: "35383136"
---
# <a name="audit-logs-for-deleted-email-messages"></a><span data-ttu-id="7dab8-102">Log audit untuk pesan dihapus email</span><span class="sxs-lookup"><span data-stu-id="7dab8-102">Audit logs for deleted email messages</span></span>

<span data-ttu-id="7dab8-103">Mulai Januari 2019, Microsoft adalah menyalakan audit kotak pesan log secara default.</span><span class="sxs-lookup"><span data-stu-id="7dab8-103">Starting in January 2019, Microsoft is turning on mailbox audit logging by default.</span></span> <span data-ttu-id="7dab8-104">Jika tidak, untuk meninjau Hapus pesan acara untuk pengguna tertentu, Anda harus secara manual mengaktifkan tindakan delete untuk audit.</span><span class="sxs-lookup"><span data-stu-id="7dab8-104">Otherwise, to review delete message events for a specific user, you need to manually enable the delete actions for auditing.</span></span> <span data-ttu-id="7dab8-105">Jika kotak pesan audit penebangan kayu sudah diaktifkan untuk organisasi Anda atau untuk pengguna tertentu, ikuti langkah berikut.</span><span class="sxs-lookup"><span data-stu-id="7dab8-105">If mailbox audit logging is already enabled for your organization or for the specific user, follow the steps below.</span></span>

1. <span data-ttu-id="7dab8-106">Masuk ke [Kantor 365 keamanan & Compliance Center](https://protection.office.com/)</span><span class="sxs-lookup"><span data-stu-id="7dab8-106">Log in to the [Office 365 Security & Compliance Center](https://protection.office.com/)</span></span>

2. <span data-ttu-id="7dab8-107">Klik **Cari dan penyelidikan** dan pilih **Cari Log Audit**.</span><span class="sxs-lookup"><span data-stu-id="7dab8-107">Click **Search and Investigation** and select **Audit Log Search**.</span></span>

3. <span data-ttu-id="7dab8-108">Pilih rentang tanggal di bidang **tanggal mulai** dan **tanggal akhir** .</span><span class="sxs-lookup"><span data-stu-id="7dab8-108">Select the date range in the **Start date** and **End date** fields.</span></span> <span data-ttu-id="7dab8-109">Tentukan nama pengguna untuk pengguna yang ingin menyelidiki (pengguna yang dihapus).</span><span class="sxs-lookup"><span data-stu-id="7dab8-109">Specify username for the user that you want to investigate (the user who deleted the items).</span></span> <span data-ttu-id="7dab8-110">Di bidang **kegiatan** , pilih **pesan dihapus dari folder Item dihapus** dan **pesan dipindahkan ke folder Item dihapus**.</span><span class="sxs-lookup"><span data-stu-id="7dab8-110">In the **Activities** field, select **Deleted messages from Deleted Items folder** and **Moved messages to Deleted Items folder**.</span></span>

4. <span data-ttu-id="7dab8-111">Klik **Cari**.</span><span class="sxs-lookup"><span data-stu-id="7dab8-111">Click **Search**.</span></span>

<span data-ttu-id="7dab8-112">Hasil, pilih catatan audit.</span><span class="sxs-lookup"><span data-stu-id="7dab8-112">In the results, select an audit record.</span></span> <span data-ttu-id="7dab8-113">Di flyout rincian, klik **Informasi selengkapnya**.</span><span class="sxs-lookup"><span data-stu-id="7dab8-113">In the details flyout, click **More Information**.</span></span> <span data-ttu-id="7dab8-114">Informasi tambahan tentang item yang dihapus (misalnya, baris subjek dan lokasi item ketika dihapus) dipajangkan di bidang **AffectedItems** .</span><span class="sxs-lookup"><span data-stu-id="7dab8-114">Additional information about the deleted item (for example, the subject line and the location of the item when it was deleted) is displayed in the **AffectedItems** field.</span></span> <span data-ttu-id="7dab8-115">Properti **ClientInfoString** akan menunjukkan jika penghapusan terjadi di Outlook, Outlook pada web (sebelumnya dikenal sebagai Outlook Web App), atau perangkat lain.</span><span class="sxs-lookup"><span data-stu-id="7dab8-115">The **ClientInfoString** property will show if the deletion occurred in Outlook, Outlook on the web (formerly known as Outlook Web App), or any other device.</span></span>

<span data-ttu-id="7dab8-116">Untuk informasi lebih lanjut, lihat [menentukan yang mengatur email forwarding untuk kotak pesan](https://docs.microsoft.com/office365/securitycompliance/auditing-troubleshooting-scenarios#determining-if-a-user-deleted-email-items).</span><span class="sxs-lookup"><span data-stu-id="7dab8-116">For more information, see [Determining who set up email forwarding for a mailbox](https://docs.microsoft.com/office365/securitycompliance/auditing-troubleshooting-scenarios#determining-if-a-user-deleted-email-items).</span></span>

<span data-ttu-id="7dab8-117">**Catatan**: Anda tidak dapat mengambil item yang dihapus menggunakan fitur log audit.</span><span class="sxs-lookup"><span data-stu-id="7dab8-117">**Note**: You can't retrieve deleted items using the audit log feature.</span></span> <span data-ttu-id="7dab8-118">Untuk mengambil pesan dihapus di Outlook di web, lihat [memulihkan item di Outlook Web App yang dihapus](https://support.office.com/article/C3D8FC15-EEEF-4F1C-81DF-E27964B7EDD4).</span><span class="sxs-lookup"><span data-stu-id="7dab8-118">To retrieve deleted messages in Outlook on the web, see [Recover deleted items in Outlook Web App](https://support.office.com/article/C3D8FC15-EEEF-4F1C-81DF-E27964B7EDD4).</span></span>
