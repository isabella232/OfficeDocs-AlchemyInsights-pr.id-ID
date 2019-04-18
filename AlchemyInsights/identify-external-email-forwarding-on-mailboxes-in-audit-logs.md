---
title: Mengidentifikasi penerusan email eksternal pada kotak pesan di log audit
ms.author: chrisda
author: chrisda
manager: serdars
ms.date: ''
ms.audience: ITPro
ms.topic: article
ROBOTS: NOINDEX, NOFOLLOW
localization_priority: Normal
ms.custom: 1369
ms.assetid: ''
ms.openlocfilehash: 7fb2c161c558a7eb961f86ca2b86e33750d902fd
ms.sourcegitcommit: ffe2f489b1ac3aae62aa784c959da6a41c3261eb
ms.translationtype: MT
ms.contentlocale: id-ID
ms.lasthandoff: 04/17/2019
ms.locfileid: "31909325"
---
# <a name="identify-when-external-email-forwarding-is-configured-on-mailboxes"></a><span data-ttu-id="73bf4-102">Mengidentifikasi ketika penerusan email eksternal dikonfigurasi pada kotak pesan</span><span class="sxs-lookup"><span data-stu-id="73bf4-102">Identify when external email forwarding is configured on mailboxes</span></span>

<span data-ttu-id="73bf4-103">Ketika pengguna mengkonfigurasi penerusan email eksternal di kotak pesan, kegiatan audit sebagai bagian dari cmdlet **Set-Mailbox** .</span><span class="sxs-lookup"><span data-stu-id="73bf4-103">When a user configures external email forwarding on a mailbox, the activity is audited as part of the **Set-Mailbox** cmdlet.</span></span> <span data-ttu-id="73bf4-104">Anda dapat melihat aktivitas yang menggunakan log audit pencarian di & keamanan Compliance Center.</span><span class="sxs-lookup"><span data-stu-id="73bf4-104">You can see the activity using audit log search in the Security & Compliance Center.</span></span>

1. <span data-ttu-id="73bf4-105">Masuk ke [Kantor 365 keamanan & Compliance Center](https://protection.office.com/)</span><span class="sxs-lookup"><span data-stu-id="73bf4-105">Log in to the [Office 365 Security & Compliance Center](https://protection.office.com/)</span></span>

2. <span data-ttu-id="73bf4-106">Klik **Cari dan penyelidikan** dan pilih **Cari Log Audit**.</span><span class="sxs-lookup"><span data-stu-id="73bf4-106">Click **Search and Investigation** and select **Audit Log Search**.</span></span>

3. <span data-ttu-id="73bf4-107">Pilih rentang tanggal di bidang **tanggal mulai** dan **tanggal akhir** .</span><span class="sxs-lookup"><span data-stu-id="73bf4-107">Select the date range in the **Start date** and **End date** fields.</span></span> <span data-ttu-id="73bf4-108">Anda tidak perlu menetapkan nama pengguna.</span><span class="sxs-lookup"><span data-stu-id="73bf4-108">You don't need to specify a username.</span></span> <span data-ttu-id="73bf4-109">Pastikan bidang **kegiatan** diatur untuk **menunjukkan hasil untuk semua kegiatan**.</span><span class="sxs-lookup"><span data-stu-id="73bf4-109">Verify the **Activities** field is set to **Show results for all activities**.</span></span>

4. <span data-ttu-id="73bf4-110">Klik **Cari**.</span><span class="sxs-lookup"><span data-stu-id="73bf4-110">Click **Search**.</span></span>

<span data-ttu-id="73bf4-111">Hasil, klik **Filter hasil** dan ketik **Set-kotak surat** di kotak filter aktivitas.</span><span class="sxs-lookup"><span data-stu-id="73bf4-111">In the results, click **Filter Results** and type **Set-Mailbox** in the activity filter box.</span></span> <span data-ttu-id="73bf4-112">Pilih record audit dalam hasil.</span><span class="sxs-lookup"><span data-stu-id="73bf4-112">Select an audit record in the results.</span></span> <span data-ttu-id="73bf4-113">Di flyout **rincian** , klik **informasi lebih lanjut**.</span><span class="sxs-lookup"><span data-stu-id="73bf4-113">In the **Details** flyout, click **More information**.</span></span> <span data-ttu-id="73bf4-114">Anda harus melihat pada rincian dari setiap record audit untuk menentukan jika aktivitas terkait dengan email forwarding.</span><span class="sxs-lookup"><span data-stu-id="73bf4-114">You have to look at the details of each audit record to determine if the activity is related to email forwarding.</span></span>

- <span data-ttu-id="73bf4-115">**ObjectId**: nilai alias kotak pesan yang diubah.</span><span class="sxs-lookup"><span data-stu-id="73bf4-115">**ObjectId**: The alias value of the mailbox that was modified.</span></span>

- <span data-ttu-id="73bf4-116">**Parameter**: _ForwardingSmtpAddress_ menunjukkan alamat email target.</span><span class="sxs-lookup"><span data-stu-id="73bf4-116">**Parameters**: _ForwardingSmtpAddress_ indicates the target email address.</span></span>

- <span data-ttu-id="73bf4-117">**UserId**: pengguna yang dikonfigurasi pengalihan email di kotak surat di bidang **ObjectId** .</span><span class="sxs-lookup"><span data-stu-id="73bf4-117">**UserId**: The user who configured email forwarding on the mailbox in the **ObjectId** field.</span></span>

<span data-ttu-id="73bf4-118">Untuk informasi lebih lanjut, lihat [menentukan yang mengatur email forwarding untuk kotak pesan](https://docs.microsoft.com/office365/securitycompliance/auditing-troubleshooting-scenarios#determining-who-set-up-email-forwarding-for-a-mailbox).</span><span class="sxs-lookup"><span data-stu-id="73bf4-118">For more information, see [Determining who set up email forwarding for a mailbox](https://docs.microsoft.com/office365/securitycompliance/auditing-troubleshooting-scenarios#determining-who-set-up-email-forwarding-for-a-mailbox).</span></span>
