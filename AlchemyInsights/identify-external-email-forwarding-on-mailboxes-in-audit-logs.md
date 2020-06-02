---
title: Mengidentifikasi penerusan email eksternal di kotak pesan dalam log audit
ms.author: chrisda
author: chrisda
manager: dansimp
ms.date: 04/21/2020
ms.audience: ITPro
ms.topic: article
ROBOTS: NOINDEX, NOFOLLOW
localization_priority: Normal
ms.custom:
- "1369"
- "3100005"
ms.assetid: ''
ms.openlocfilehash: 592eb92e4b0fe0f9da2fa20bb93ffa4fbbb76662
ms.sourcegitcommit: bc7d6f4f3c9f7060d073f5130e1ec856e248d020
ms.translationtype: MT
ms.contentlocale: id-ID
ms.lasthandoff: 06/02/2020
ms.locfileid: "44508955"
---
# <a name="identify-when-external-email-forwarding-is-configured-on-mailboxes"></a><span data-ttu-id="9c45f-102">Mengidentifikasi saat penerusan email eksternal dikonfigurasi pada kotak pesan</span><span class="sxs-lookup"><span data-stu-id="9c45f-102">Identify when external email forwarding is configured on mailboxes</span></span>

<span data-ttu-id="9c45f-103">Ketika pengguna 365 Microsoft mengkonfigurasi penerusan email eksternal di kotak surat, aktivitas diaudit sebagai bagian dari cmdlet **Set-Mailbox** .</span><span class="sxs-lookup"><span data-stu-id="9c45f-103">When a Microsoft 365 user configures external email forwarding on a mailbox, the activity is audited as part of the **Set-Mailbox** cmdlet.</span></span> <span data-ttu-id="9c45f-104">Anda dapat melihat aktivitas menggunakan pencarian log audit di pusat kepatuhan & keamanan.</span><span class="sxs-lookup"><span data-stu-id="9c45f-104">You can see the activity using audit log search in the Security & Compliance Center.</span></span>

1. <span data-ttu-id="9c45f-105">Masuk ke [Microsoft 365 keamanan & Compliance Center](https://protection.office.com/).</span><span class="sxs-lookup"><span data-stu-id="9c45f-105">Log in to the [Microsoft 365 Security & Compliance Center](https://protection.office.com/).</span></span>

2. <span data-ttu-id="9c45f-106">Buka halaman penelusuran **Search**  >  **log audit** penelusuran.</span><span class="sxs-lookup"><span data-stu-id="9c45f-106">Go to the **Search** > **Audit log search** page.</span></span>

3. <span data-ttu-id="9c45f-107">Pilih rentang tanggal di kolom tanggal **mulai** dan **tanggal akhir** .</span><span class="sxs-lookup"><span data-stu-id="9c45f-107">Select the date range in the **Start date** and **End date** fields.</span></span> <span data-ttu-id="9c45f-108">Anda tidak perlu menentukan nama pengguna.</span><span class="sxs-lookup"><span data-stu-id="9c45f-108">You don't need to specify a username.</span></span> <span data-ttu-id="9c45f-109">Verifikasi bidang **aktivitas** diatur untuk **Menampilkan hasil untuk semua aktivitas**.</span><span class="sxs-lookup"><span data-stu-id="9c45f-109">Verify the **Activities** field is set to **Show results for all activities**.</span></span>

4. <span data-ttu-id="9c45f-110">Klik **Cari**.</span><span class="sxs-lookup"><span data-stu-id="9c45f-110">Click **Search**.</span></span>

<span data-ttu-id="9c45f-111">Di hasil, klik **filter hasil** dan ketik **set-kotak surat** di kotak filter aktivitas.</span><span class="sxs-lookup"><span data-stu-id="9c45f-111">In the results, click **Filter Results** and type **Set-Mailbox** in the activity filter box.</span></span> <span data-ttu-id="9c45f-112">Pilih catatan audit di hasil.</span><span class="sxs-lookup"><span data-stu-id="9c45f-112">Select an audit record in the results.</span></span> <span data-ttu-id="9c45f-113">Di Flyout **rincian** , klik **informasi lebih lanjut**.</span><span class="sxs-lookup"><span data-stu-id="9c45f-113">In the **Details** flyout, click **More information**.</span></span> <span data-ttu-id="9c45f-114">Anda harus melihat rincian setiap catatan audit untuk menentukan apakah aktivitas terkait dengan penerusan email.</span><span class="sxs-lookup"><span data-stu-id="9c45f-114">You have to look at the details of each audit record to determine if the activity is related to email forwarding.</span></span>

- <span data-ttu-id="9c45f-115">**ObjectID**: nilai alias kotak surat yang telah diubah.</span><span class="sxs-lookup"><span data-stu-id="9c45f-115">**ObjectId**: The alias value of the mailbox that was modified.</span></span>

- <span data-ttu-id="9c45f-116">**Parameter**: _forwardingsmtpaddress_ menunjukkan alamat email target.</span><span class="sxs-lookup"><span data-stu-id="9c45f-116">**Parameters**: _ForwardingSmtpAddress_ indicates the target email address.</span></span>

- <span data-ttu-id="9c45f-117">**Userid**: pengguna yang dikonfigurasi penerusan email di kotak surat di kolom **ObjectID** .</span><span class="sxs-lookup"><span data-stu-id="9c45f-117">**UserId**: The user who configured email forwarding on the mailbox in the **ObjectId** field.</span></span>

<span data-ttu-id="9c45f-118">Untuk selengkapnya, lihat [menentukan siapa yang mengatur penerusan email untuk kotak pesan](https://docs.microsoft.com/microsoft-365/compliance/auditing-troubleshooting-scenarios#determine-who-set-up-email-forwarding-for-a-mailbox).</span><span class="sxs-lookup"><span data-stu-id="9c45f-118">For more information, see [Determining who set up email forwarding for a mailbox](https://docs.microsoft.com/microsoft-365/compliance/auditing-troubleshooting-scenarios#determine-who-set-up-email-forwarding-for-a-mailbox).</span></span>
