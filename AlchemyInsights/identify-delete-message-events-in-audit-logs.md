---
title: Mengidentifikasi menghapus peristiwa pesan di log audit
ms.author: chrisda
author: chrisda
manager: dansimp
ms.date: 04/21/2020
ms.audience: ITPro
ms.topic: article
ROBOTS: NOINDEX, NOFOLLOW
localization_priority: Normal
ms.custom:
- "1370"
- "3100005"
ms.assetid: ''
ms.openlocfilehash: 797a4b1146862faf91d2b9e8d74feade90f71650
ms.sourcegitcommit: 55eff703a17e500681d8fa6a87eb067019ade3cc
ms.translationtype: MT
ms.contentlocale: id-ID
ms.lasthandoff: 04/22/2020
ms.locfileid: "43716499"
---
# <a name="audit-logs-for-deleted-email-messages"></a><span data-ttu-id="92c83-102">Log audit untuk pesan email yang dihapus</span><span class="sxs-lookup"><span data-stu-id="92c83-102">Audit logs for deleted email messages</span></span>

<span data-ttu-id="92c83-103">Mulai Januari 2019, Microsoft telah mengaktifkan pengelogan audit kotak surat secara default.</span><span class="sxs-lookup"><span data-stu-id="92c83-103">Starting in January 2019, Microsoft is turning on mailbox audit logging by default.</span></span> <span data-ttu-id="92c83-104">Jika tidak, untuk meninjau menghapus peristiwa pesan untuk pengguna tertentu, Anda harus secara manual mengaktifkan tindakan Hapus untuk audit.</span><span class="sxs-lookup"><span data-stu-id="92c83-104">Otherwise, to review delete message events for a specific user, you need to manually enable the delete actions for auditing.</span></span> <span data-ttu-id="92c83-105">Jika pencatatan audit kotak pesan sudah diaktifkan untuk organisasi Anda atau pengguna tertentu, ikuti langkah di bawah.</span><span class="sxs-lookup"><span data-stu-id="92c83-105">If mailbox audit logging is already enabled for your organization or for the specific user, follow the steps below.</span></span>

1. <span data-ttu-id="92c83-106">Masuk ke [Microsoft 365 keamanan & Compliance Center](https://protection.office.com/)</span><span class="sxs-lookup"><span data-stu-id="92c83-106">Log in to the [Microsoft 365 Security & Compliance Center](https://protection.office.com/)</span></span>

2. <span data-ttu-id="92c83-107">Klik **Cari dan investigasi** , lalu pilih **pencarian log audit**.</span><span class="sxs-lookup"><span data-stu-id="92c83-107">Click **Search and Investigation** and select **Audit Log Search**.</span></span>

3. <span data-ttu-id="92c83-108">Pilih rentang tanggal di kolom tanggal **mulai** dan **tanggal akhir** .</span><span class="sxs-lookup"><span data-stu-id="92c83-108">Select the date range in the **Start date** and **End date** fields.</span></span> <span data-ttu-id="92c83-109">Tentukan username untuk pengguna yang ingin Anda menyelidiki (pengguna yang dihapus item).</span><span class="sxs-lookup"><span data-stu-id="92c83-109">Specify username for the user that you want to investigate (the user who deleted the items).</span></span> <span data-ttu-id="92c83-110">Di bidang **aktivitas** , pilih **pesan yang dihapus dari folder Item dihapus** dan **Pindahkan pesan ke folder Item dihapus**.</span><span class="sxs-lookup"><span data-stu-id="92c83-110">In the **Activities** field, select **Deleted messages from Deleted Items folder** and **Moved messages to Deleted Items folder**.</span></span>

4. <span data-ttu-id="92c83-111">Klik **Cari**.</span><span class="sxs-lookup"><span data-stu-id="92c83-111">Click **Search**.</span></span>

<span data-ttu-id="92c83-112">Di hasil, pilih rekaman audit.</span><span class="sxs-lookup"><span data-stu-id="92c83-112">In the results, select an audit record.</span></span> <span data-ttu-id="92c83-113">Dalam Flyout rincian, klik **informasi lebih lanjut**.</span><span class="sxs-lookup"><span data-stu-id="92c83-113">In the details flyout, click **More Information**.</span></span> <span data-ttu-id="92c83-114">Informasi tambahan tentang item yang dihapus (misalnya, baris subjek dan lokasi item saat dihapus) ditampilkan di bidang **Affecteditems** .</span><span class="sxs-lookup"><span data-stu-id="92c83-114">Additional information about the deleted item (for example, the subject line and the location of the item when it was deleted) is displayed in the **AffectedItems** field.</span></span> <span data-ttu-id="92c83-115">Properti **Clientinfostring** akan menunjukkan jika penghapusan terjadi di Outlook, Outlook di web (sebelumnya dikenal sebagai Outlook Web App), atau perangkat lainnya.</span><span class="sxs-lookup"><span data-stu-id="92c83-115">The **ClientInfoString** property will show if the deletion occurred in Outlook, Outlook on the web (formerly known as Outlook Web App), or any other device.</span></span>

<span data-ttu-id="92c83-116">Untuk selengkapnya, lihat [menentukan siapa yang mengatur penerusan email untuk kotak pesan](https://docs.microsoft.com/office365/securitycompliance/auditing-troubleshooting-scenarios#determining-if-a-user-deleted-email-items).</span><span class="sxs-lookup"><span data-stu-id="92c83-116">For more information, see [Determining who set up email forwarding for a mailbox](https://docs.microsoft.com/office365/securitycompliance/auditing-troubleshooting-scenarios#determining-if-a-user-deleted-email-items).</span></span>

<span data-ttu-id="92c83-117">**Catatan**: Anda tidak dapat mengambil item yang dihapus menggunakan fitur log audit.</span><span class="sxs-lookup"><span data-stu-id="92c83-117">**Note**: You can't retrieve deleted items using the audit log feature.</span></span> <span data-ttu-id="92c83-118">Untuk mengambil pesan yang dihapus di Outlook di web, lihat [memulihkan item yang dihapus di Outlook Web App](https://support.office.com/article/C3D8FC15-EEEF-4F1C-81DF-E27964B7EDD4).</span><span class="sxs-lookup"><span data-stu-id="92c83-118">To retrieve deleted messages in Outlook on the web, see [Recover deleted items in Outlook Web App](https://support.office.com/article/C3D8FC15-EEEF-4F1C-81DF-E27964B7EDD4).</span></span>
