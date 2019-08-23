---
title: Mengidentifikasi penerusan email eksternal pada kotak pesan di log audit
ms.author: chrisda
author: chrisda
manager: dansimp
ms.date: ''
ms.audience: ITPro
ms.topic: article
ROBOTS: NOINDEX, NOFOLLOW
localization_priority: Normal
ms.custom:
- "1369"
- "3100005"
ms.assetid: ''
ms.openlocfilehash: 7defd0902e8c8bebae9c7bfee72c3199cbc1909f
ms.sourcegitcommit: 1d98db8acb9959aba3b5e308a567ade6b62da56c
ms.translationtype: MT
ms.contentlocale: id-ID
ms.lasthandoff: 08/22/2019
ms.locfileid: "36539104"
---
# <a name="identify-when-external-email-forwarding-is-configured-on-mailboxes"></a><span data-ttu-id="c0aed-102">Mengidentifikasi ketika penerusan email eksternal dikonfigurasi pada kotak pesan</span><span class="sxs-lookup"><span data-stu-id="c0aed-102">Identify when external email forwarding is configured on mailboxes</span></span>

<span data-ttu-id="c0aed-103">Ketika pengguna Office 365 mengkonfigurasi penerusan email eksternal di kotak pesan, kegiatan audit sebagai bagian dari cmdlet **Set-Mailbox** .</span><span class="sxs-lookup"><span data-stu-id="c0aed-103">When an Office 365  user configures external email forwarding on a mailbox, the activity is audited as part of the **Set-Mailbox** cmdlet.</span></span> <span data-ttu-id="c0aed-104">Anda dapat melihat aktivitas yang menggunakan log audit pencarian di & keamanan Compliance Center.</span><span class="sxs-lookup"><span data-stu-id="c0aed-104">You can see the activity using audit log search in the Security & Compliance Center.</span></span>

1. <span data-ttu-id="c0aed-105">Masuk ke [Kantor 365 keamanan & Compliance Center](https://protection.office.com/).</span><span class="sxs-lookup"><span data-stu-id="c0aed-105">Log in to the [Office 365 Security & Compliance Center](https://protection.office.com/).</span></span>

2. <span data-ttu-id="c0aed-106">Pergi ke **pencarian** > halaman**pencarian log Audit** .</span><span class="sxs-lookup"><span data-stu-id="c0aed-106">Go to the **Search** > **Audit log search** page.</span></span>

3. <span data-ttu-id="c0aed-107">Pilih rentang tanggal di bidang **tanggal mulai** dan **tanggal akhir** .</span><span class="sxs-lookup"><span data-stu-id="c0aed-107">Select the date range in the **Start date** and **End date** fields.</span></span> <span data-ttu-id="c0aed-108">Anda tidak perlu menetapkan nama pengguna.</span><span class="sxs-lookup"><span data-stu-id="c0aed-108">You don't need to specify a username.</span></span> <span data-ttu-id="c0aed-109">Pastikan bidang **kegiatan** diatur untuk **menunjukkan hasil untuk semua kegiatan**.</span><span class="sxs-lookup"><span data-stu-id="c0aed-109">Verify the **Activities** field is set to **Show results for all activities**.</span></span>

4. <span data-ttu-id="c0aed-110">Klik **Cari**.</span><span class="sxs-lookup"><span data-stu-id="c0aed-110">Click **Search**.</span></span>

<span data-ttu-id="c0aed-111">Hasil, klik **Filter hasil** dan ketik **Set-kotak surat** di kotak filter aktivitas.</span><span class="sxs-lookup"><span data-stu-id="c0aed-111">In the results, click **Filter Results** and type **Set-Mailbox** in the activity filter box.</span></span> <span data-ttu-id="c0aed-112">Pilih record audit dalam hasil.</span><span class="sxs-lookup"><span data-stu-id="c0aed-112">Select an audit record in the results.</span></span> <span data-ttu-id="c0aed-113">Di flyout **rincian** , klik **informasi lebih lanjut**.</span><span class="sxs-lookup"><span data-stu-id="c0aed-113">In the **Details** flyout, click **More information**.</span></span> <span data-ttu-id="c0aed-114">Anda harus melihat pada rincian dari setiap record audit untuk menentukan jika aktivitas terkait dengan email forwarding.</span><span class="sxs-lookup"><span data-stu-id="c0aed-114">You have to look at the details of each audit record to determine if the activity is related to email forwarding.</span></span>

- <span data-ttu-id="c0aed-115">**ObjectId**: nilai alias kotak pesan yang diubah.</span><span class="sxs-lookup"><span data-stu-id="c0aed-115">**ObjectId**: The alias value of the mailbox that was modified.</span></span>

- <span data-ttu-id="c0aed-116">**Parameter**: _ForwardingSmtpAddress_ menunjukkan alamat email target.</span><span class="sxs-lookup"><span data-stu-id="c0aed-116">**Parameters**: _ForwardingSmtpAddress_ indicates the target email address.</span></span>

- <span data-ttu-id="c0aed-117">**UserId**: pengguna yang dikonfigurasi pengalihan email di kotak surat di bidang **ObjectId** .</span><span class="sxs-lookup"><span data-stu-id="c0aed-117">**UserId**: The user who configured email forwarding on the mailbox in the **ObjectId** field.</span></span>

<span data-ttu-id="c0aed-118">Untuk informasi lebih lanjut, lihat [menentukan yang mengatur email forwarding untuk kotak pesan](https://docs.microsoft.com/office365/securitycompliance/auditing-troubleshooting-scenarios#determining-who-set-up-email-forwarding-for-a-mailbox).</span><span class="sxs-lookup"><span data-stu-id="c0aed-118">For more information, see [Determining who set up email forwarding for a mailbox](https://docs.microsoft.com/office365/securitycompliance/auditing-troubleshooting-scenarios#determining-who-set-up-email-forwarding-for-a-mailbox).</span></span>
