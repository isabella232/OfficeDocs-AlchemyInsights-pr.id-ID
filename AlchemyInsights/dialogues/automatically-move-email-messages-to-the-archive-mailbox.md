---
title: Memindahkan pesan email secara otomatis ke kotak surat Arsip
ms.author: v-jmathew
author: v-jmathew
manager: dansimp
audience: Admin
ms.topic: article
ms.service: o365-administration
ROBOTS: NOINDEX, NOFOLLOW
localization_priority: Normal
ms.collection: Adm_O365
ms.custom:
- "3100008"
- "7217"
ms.openlocfilehash: 14ded561ee2b3c244fadbdab42fd0e833a1c66d5
ms.sourcegitcommit: 7fa9bf6f9fc7438791aa9241a440e5be817d4401
ms.translationtype: MT
ms.contentlocale: id-ID
ms.lasthandoff: 03/08/2021
ms.locfileid: "50527097"
---
# <a name="automatically-move-email-messages-to-the-archive-mailbox"></a><span data-ttu-id="9b8b5-102">Memindahkan pesan email secara otomatis ke kotak surat Arsip</span><span class="sxs-lookup"><span data-stu-id="9b8b5-102">Automatically move email messages to the archive mailbox</span></span>

<span data-ttu-id="9b8b5-103">Berikut ini cara menyiapkan kebijakan untuk secara otomatis memindahkan email lama pengguna ke kotak surat Arsip:</span><span class="sxs-lookup"><span data-stu-id="9b8b5-103">Here's how to set up a policy to automatically move a user's old email to the archive mailbox:</span></span>

1. <span data-ttu-id="9b8b5-104">Masuk ke [](https://go.microsoft.com/fwlink/p/?linkid=2077143)  >  **Arsip tata kelola data** kepatuhan & keamanan  >   untuk memverifikasi kotak surat Arsip telah diaktifkan untuk pengguna.</span><span class="sxs-lookup"><span data-stu-id="9b8b5-104">Go to [**Security & Compliance**](https://go.microsoft.com/fwlink/p/?linkid=2077143) > **Data governance** > **Archive** to verify an archive mailbox has been enabled for the user.</span></span> <span data-ttu-id="9b8b5-105">Jika belum, klik **Aktifkan** lalu **ya** dalam kotak peringatan.</span><span class="sxs-lookup"><span data-stu-id="9b8b5-105">If it hasn't, click **Enable** then **Yes** in the warning box.</span></span>
2. <span data-ttu-id="9b8b5-106">Masuk ke [**Pusat admin Exchange > manajemen kepatuhan > tag penyimpanan**](https://go.microsoft.com/fwlink/?linkid=2059104).</span><span class="sxs-lookup"><span data-stu-id="9b8b5-106">Go to [**Exchange admin center > compliance management > retention tags**](https://go.microsoft.com/fwlink/?linkid=2059104).</span></span>
3. <span data-ttu-id="9b8b5-107">Pilih ikon + lalu pilih **Terapkan secara otomatis ke seluruh kotak surat**.</span><span class="sxs-lookup"><span data-stu-id="9b8b5-107">Choose the + icon then choose **automatically apply to entire mailbox**.</span></span>
4. <span data-ttu-id="9b8b5-108">Tetapkan nama ke tag penyimpanan, dan pilih **Pindahkan ke arsip**.</span><span class="sxs-lookup"><span data-stu-id="9b8b5-108">Assign a name to the retention tag, and choose **Move to Archive**.</span></span> <span data-ttu-id="9b8b5-109">Untuk periode penyimpanan, masukkan waktu yang Anda inginkan, seperti 90 hari.</span><span class="sxs-lookup"><span data-stu-id="9b8b5-109">For the retention period, enter the time you want, such as 90 days.</span></span> <span data-ttu-id="9b8b5-110">Klik **Simpan**.</span><span class="sxs-lookup"><span data-stu-id="9b8b5-110">Click **Save**.</span></span>
5. <span data-ttu-id="9b8b5-111">Sekarang Buat kebijakan penyimpanan: Pilih **kebijakan penyimpanan**, pilih ikon untuk menambahkan kebijakan baru.</span><span class="sxs-lookup"><span data-stu-id="9b8b5-111">Now create a retention policy: choose **retention policies**, choose the icon to add a new policy.</span></span>
6. <span data-ttu-id="9b8b5-112">Tetapkan nama ke kebijakan penyimpanan, lalu klik dan gulir untuk menemukan dan menambahkan tag penyimpanan yang baru Anda buat.</span><span class="sxs-lookup"><span data-stu-id="9b8b5-112">Assign a name to the retention policy, then click and scroll to find and add the retention tag you just created.</span></span> <span data-ttu-id="9b8b5-113">Klik **Simpan**.</span><span class="sxs-lookup"><span data-stu-id="9b8b5-113">Click **Save**.</span></span>
7. <span data-ttu-id="9b8b5-114">Terakhir, Terapkan kebijakan penyimpanan ke kotak surat pengguna: masih di pusat admin Exchange, masuk ke   >  **kotak surat** Penerima.</span><span class="sxs-lookup"><span data-stu-id="9b8b5-114">Finally, apply the retention policy to the user's mailbox: still in the Exchange admin center, go to **recipients** > **mailboxes**.</span></span> <span data-ttu-id="9b8b5-115">Pilih Semua pengguna yang ingin Anda Terapkan kebijakannya, lalu pilih **Edit** (ikon pensil).</span><span class="sxs-lookup"><span data-stu-id="9b8b5-115">Choose all the users who you want to apply the policy to, then choose **Edit** (the pencil icon).</span></span>
8. <span data-ttu-id="9b8b5-116">Dalam kotak dialog, klik **fitur kotak surat**.</span><span class="sxs-lookup"><span data-stu-id="9b8b5-116">In the dialog box, click **mailbox features**.</span></span> <span data-ttu-id="9b8b5-117">Di bawah **kebijakan penyimpanan**, Terapkan kebijakan yang baru anda buat > **Simpan**.</span><span class="sxs-lookup"><span data-stu-id="9b8b5-117">Under **Retention policy**, apply the policy you just created > **Save**.</span></span>
9. <span data-ttu-id="9b8b5-118">Untuk instruksi tentang penerapan kebijakan kepada semua pengguna, lihat [menerapkan kebijakan penyimpanan ke kotak surat](https://docs.microsoft.com/exchange/security-and-compliance/messaging-records-management/apply-retention-policy).</span><span class="sxs-lookup"><span data-stu-id="9b8b5-118">For instructions for applying the policy to all users, see [Apply a retention policy to mailboxes](https://docs.microsoft.com/exchange/security-and-compliance/messaging-records-management/apply-retention-policy).</span></span>
