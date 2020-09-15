---
title: Mengidentifikasi penerusan email eksternal pada kotak surat dalam log audit
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
- "1369"
- "3100005"
ms.assetid: ''
ms.openlocfilehash: d06ef83adcae1342173a6fe75f79525c7e1797ce
ms.sourcegitcommit: c6692ce0fa1358ec3529e59ca0ecdfdea4cdc759
ms.translationtype: MT
ms.contentlocale: id-ID
ms.lasthandoff: 09/14/2020
ms.locfileid: "47696300"
---
# <a name="identify-when-external-email-forwarding-is-configured-on-mailboxes"></a><span data-ttu-id="4040d-102">Mengidentifikasi Kapan penerusan email eksternal dikonfigurasikan pada kotak surat</span><span class="sxs-lookup"><span data-stu-id="4040d-102">Identify when external email forwarding is configured on mailboxes</span></span>

<span data-ttu-id="4040d-103">Saat pengguna Microsoft 365 mengonfigurasi penerusan email eksternal pada kotak surat, aktivitas diaudit sebagai bagian dari cmdlet **Set-Mailbox** .</span><span class="sxs-lookup"><span data-stu-id="4040d-103">When a Microsoft 365 user configures external email forwarding on a mailbox, the activity is audited as part of the **Set-Mailbox** cmdlet.</span></span> <span data-ttu-id="4040d-104">Anda dapat melihat aktivitas menggunakan pencarian log audit di pusat kepatuhan & keamanan.</span><span class="sxs-lookup"><span data-stu-id="4040d-104">You can see the activity using audit log search in the Security & Compliance Center.</span></span>

1. <span data-ttu-id="4040d-105">Masuk ke [pusat kepatuhan & keamanan Microsoft 365](https://protection.office.com/).</span><span class="sxs-lookup"><span data-stu-id="4040d-105">Log in to the [Microsoft 365 Security & Compliance Center](https://protection.office.com/).</span></span>

2. <span data-ttu-id="4040d-106">Masuk ke halaman **Search**  >  **pencarian log audit** pencarian.</span><span class="sxs-lookup"><span data-stu-id="4040d-106">Go to the **Search** > **Audit log search** page.</span></span>

3. <span data-ttu-id="4040d-107">Pilih rentang tanggal di bidang tanggal **mulai** dan **tanggal berakhir** .</span><span class="sxs-lookup"><span data-stu-id="4040d-107">Select the date range in the **Start date** and **End date** fields.</span></span> <span data-ttu-id="4040d-108">Anda tidak perlu menentukan nama pengguna.</span><span class="sxs-lookup"><span data-stu-id="4040d-108">You don't need to specify a username.</span></span> <span data-ttu-id="4040d-109">Verifikasi bidang **aktivitas** diatur untuk **memperlihatkan hasil untuk semua aktivitas**.</span><span class="sxs-lookup"><span data-stu-id="4040d-109">Verify the **Activities** field is set to **Show results for all activities**.</span></span>

4. <span data-ttu-id="4040d-110">Klik **Cari**.</span><span class="sxs-lookup"><span data-stu-id="4040d-110">Click **Search**.</span></span>

<span data-ttu-id="4040d-111">Dalam hasil, klik **filter hasil** dan ketik **set-kotak surat** di kotak filter aktivitas.</span><span class="sxs-lookup"><span data-stu-id="4040d-111">In the results, click **Filter Results** and type **Set-Mailbox** in the activity filter box.</span></span> <span data-ttu-id="4040d-112">Pilih catatan audit dalam hasil.</span><span class="sxs-lookup"><span data-stu-id="4040d-112">Select an audit record in the results.</span></span> <span data-ttu-id="4040d-113">Dalam Flyout **detail** , klik **informasi selengkapnya**.</span><span class="sxs-lookup"><span data-stu-id="4040d-113">In the **Details** flyout, click **More information**.</span></span> <span data-ttu-id="4040d-114">Anda harus melihat detail setiap catatan audit untuk menentukan apakah aktivitas terkait dengan penerusan email.</span><span class="sxs-lookup"><span data-stu-id="4040d-114">You have to look at the details of each audit record to determine if the activity is related to email forwarding.</span></span>

- <span data-ttu-id="4040d-115">**ObjectID**: nilai alias dari kotak surat yang telah dimodifikasi.</span><span class="sxs-lookup"><span data-stu-id="4040d-115">**ObjectId**: The alias value of the mailbox that was modified.</span></span>

- <span data-ttu-id="4040d-116">**Parameter**: _forwardingsmtpaddress_ menunjukkan alamat email target.</span><span class="sxs-lookup"><span data-stu-id="4040d-116">**Parameters**: _ForwardingSmtpAddress_ indicates the target email address.</span></span>

- <span data-ttu-id="4040d-117">**Userid**: pengguna yang mengonfigurasikan penerusan email pada kotak surat di bidang **ObjectID** .</span><span class="sxs-lookup"><span data-stu-id="4040d-117">**UserId**: The user who configured email forwarding on the mailbox in the **ObjectId** field.</span></span>

<span data-ttu-id="4040d-118">Untuk informasi selengkapnya, lihat [menentukan siapa yang menyetel penerusan email untuk kotak surat](https://docs.microsoft.com/microsoft-365/compliance/auditing-troubleshooting-scenarios#determine-who-set-up-email-forwarding-for-a-mailbox).</span><span class="sxs-lookup"><span data-stu-id="4040d-118">For more information, see [Determining who set up email forwarding for a mailbox](https://docs.microsoft.com/microsoft-365/compliance/auditing-troubleshooting-scenarios#determine-who-set-up-email-forwarding-for-a-mailbox).</span></span>
