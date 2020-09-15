---
title: Mengidentifikasi menghapus acara pesan dalam log audit
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
- "1370"
- "3100005"
ms.assetid: ''
ms.openlocfilehash: bc78076706aee15a3133c4b1a89064591f790b58
ms.sourcegitcommit: c6692ce0fa1358ec3529e59ca0ecdfdea4cdc759
ms.translationtype: MT
ms.contentlocale: id-ID
ms.lasthandoff: 09/14/2020
ms.locfileid: "47696516"
---
# <a name="audit-logs-for-deleted-email-messages"></a><span data-ttu-id="6c7e3-102">Log audit untuk pesan email yang dihapus</span><span class="sxs-lookup"><span data-stu-id="6c7e3-102">Audit logs for deleted email messages</span></span>

<span data-ttu-id="6c7e3-103">Mulai Januari 2019, Microsoft mengaktifkan pembuatan log audit kotak surat secara default.</span><span class="sxs-lookup"><span data-stu-id="6c7e3-103">Starting in January 2019, Microsoft is turning on mailbox audit logging by default.</span></span> <span data-ttu-id="6c7e3-104">Jika tidak, untuk meninjau menghapus acara pesan untuk pengguna tertentu, Anda perlu mengaktifkan tindakan penghapusan untuk pengauditan secara manual.</span><span class="sxs-lookup"><span data-stu-id="6c7e3-104">Otherwise, to review delete message events for a specific user, you need to manually enable the delete actions for auditing.</span></span> <span data-ttu-id="6c7e3-105">Jika pembuatan log audit kotak surat sudah diaktifkan untuk organisasi Anda atau pengguna tertentu, ikuti langkah-langkah di bawah ini.</span><span class="sxs-lookup"><span data-stu-id="6c7e3-105">If mailbox audit logging is already enabled for your organization or for the specific user, follow the steps below.</span></span>

1. <span data-ttu-id="6c7e3-106">Masuk ke [pusat kepatuhan & keamanan Microsoft 365](https://protection.office.com/)</span><span class="sxs-lookup"><span data-stu-id="6c7e3-106">Log in to the [Microsoft 365 Security & Compliance Center](https://protection.office.com/)</span></span>

2. <span data-ttu-id="6c7e3-107">Klik **pencarian dan investigasi** dan pilih **pencarian log audit**.</span><span class="sxs-lookup"><span data-stu-id="6c7e3-107">Click **Search and Investigation** and select **Audit Log Search**.</span></span>

3. <span data-ttu-id="6c7e3-108">Pilih rentang tanggal di bidang tanggal **mulai** dan **tanggal berakhir** .</span><span class="sxs-lookup"><span data-stu-id="6c7e3-108">Select the date range in the **Start date** and **End date** fields.</span></span> <span data-ttu-id="6c7e3-109">Tentukan nama pengguna untuk pengguna yang ingin Anda selidiki (pengguna yang menghapus item).</span><span class="sxs-lookup"><span data-stu-id="6c7e3-109">Specify username for the user that you want to investigate (the user who deleted the items).</span></span> <span data-ttu-id="6c7e3-110">Di bidang **aktivitas** , pilih **pesan yang dihapus dari folder Item terhapus** dan **Pindahkan pesan ke folder Item terhapus**.</span><span class="sxs-lookup"><span data-stu-id="6c7e3-110">In the **Activities** field, select **Deleted messages from Deleted Items folder** and **Moved messages to Deleted Items folder**.</span></span>

4. <span data-ttu-id="6c7e3-111">Klik **Cari**.</span><span class="sxs-lookup"><span data-stu-id="6c7e3-111">Click **Search**.</span></span>

<span data-ttu-id="6c7e3-112">Dalam hasil, pilih catatan audit.</span><span class="sxs-lookup"><span data-stu-id="6c7e3-112">In the results, select an audit record.</span></span> <span data-ttu-id="6c7e3-113">Dalam Flyout detail, klik **informasi selengkapnya**.</span><span class="sxs-lookup"><span data-stu-id="6c7e3-113">In the details flyout, click **More Information**.</span></span> <span data-ttu-id="6c7e3-114">Informasi tambahan tentang item terhapus (misalnya, baris subjek dan lokasi item saat dihapus) ditampilkan di bidang **Affecteditems** .</span><span class="sxs-lookup"><span data-stu-id="6c7e3-114">Additional information about the deleted item (for example, the subject line and the location of the item when it was deleted) is displayed in the **AffectedItems** field.</span></span> <span data-ttu-id="6c7e3-115">Properti **Clientinfostring** akan ditampilkan jika penghapusan terjadi di Outlook, Outlook di web (sebelumnya dikenal sebagai Outlook Web App), atau perangkat lain.</span><span class="sxs-lookup"><span data-stu-id="6c7e3-115">The **ClientInfoString** property will show if the deletion occurred in Outlook, Outlook on the web (formerly known as Outlook Web App), or any other device.</span></span>

<span data-ttu-id="6c7e3-116">Untuk informasi selengkapnya, lihat [menentukan siapa yang menyetel penerusan email untuk kotak surat](https://docs.microsoft.com/microsoft-365/compliance/auditing-troubleshooting-scenarios#determine-if-a-user-deleted-email-items).</span><span class="sxs-lookup"><span data-stu-id="6c7e3-116">For more information, see [Determining who set up email forwarding for a mailbox](https://docs.microsoft.com/microsoft-365/compliance/auditing-troubleshooting-scenarios#determine-if-a-user-deleted-email-items).</span></span>

<span data-ttu-id="6c7e3-117">**Catatan**: Anda tidak bisa mengambil item terhapus menggunakan fitur log audit.</span><span class="sxs-lookup"><span data-stu-id="6c7e3-117">**Note**: You can't retrieve deleted items using the audit log feature.</span></span> <span data-ttu-id="6c7e3-118">Untuk mengambil pesan yang dihapus di Outlook di web, lihat [memulihkan item terhapus di Outlook Web App](https://support.office.com/article/C3D8FC15-EEEF-4F1C-81DF-E27964B7EDD4).</span><span class="sxs-lookup"><span data-stu-id="6c7e3-118">To retrieve deleted messages in Outlook on the web, see [Recover deleted items in Outlook Web App](https://support.office.com/article/C3D8FC15-EEEF-4F1C-81DF-E27964B7EDD4).</span></span>
