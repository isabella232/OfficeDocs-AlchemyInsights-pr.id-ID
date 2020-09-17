---
title: Memindahkan pesan email ke kotak surat Arsip
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
- "1083"
- "3100008"
ms.assetid: 59cd8630-6196-4680-ad92-1ce0e479f924
ms.openlocfilehash: 61d0b1a58fff6655b745bb9d39e8384f0a543336
ms.sourcegitcommit: c6692ce0fa1358ec3529e59ca0ecdfdea4cdc759
ms.translationtype: MT
ms.contentlocale: id-ID
ms.lasthandoff: 09/15/2020
ms.locfileid: "47799783"
---
# <a name="move-email-to-the-archive-mailbox"></a><span data-ttu-id="5b925-102">Memindahkan email ke kotak surat Arsip</span><span class="sxs-lookup"><span data-stu-id="5b925-102">Move email to the archive mailbox</span></span>

<span data-ttu-id="5b925-103">Jika Anda ingin kami menjalankan pemeriksaan otomatis untuk pengaturan yang disebutkan di bawah ini, pilih tombol kembali <--di bagian atas Halaman ini, lalu masukkan alamat email pengguna yang mengalami masalah dalam memindahkan email ke kotak surat arsip mereka.</span><span class="sxs-lookup"><span data-stu-id="5b925-103">If you want us to run automated checks for the settings mentioned below, select the back button <-- at the top of this page, and then enter the email address of the user who has problems moving email to their archive mailbox.</span></span>

1. <span data-ttu-id="5b925-104">Konfirmasi bahwa **kotak surat Arsip** telah diaktifkan.</span><span class="sxs-lookup"><span data-stu-id="5b925-104">Confirm that an **Archive mailbox** has been enabled.</span></span> <span data-ttu-id="5b925-105">Jika tidak, gunakan langkah-langkah dalam [artikel ini](https://docs.microsoft.com/microsoft-365/compliance/enable-archive-mailboxes) untuk mengaktifkan kotak surat Arsip.</span><span class="sxs-lookup"><span data-stu-id="5b925-105">If not, use the steps in [this article](https://docs.microsoft.com/microsoft-365/compliance/enable-archive-mailboxes) to enable the archive mailbox.</span></span>

2. <span data-ttu-id="5b925-106">Untuk mengarsipkan pesan secara otomatis ke kotak surat arsip, tag penyimpanan dengan tindakan **Pindahkan ke arsip** harus diatur untuk diterapkan secara **otomatis ke seluruh Tag kotak surat (default)**.</span><span class="sxs-lookup"><span data-stu-id="5b925-106">To archive messages automatically to the archive mailbox, a retention tag with the **Move to archive** action must be set to **applied automatically to entire mailbox (default) tag**.</span></span> <span data-ttu-id="5b925-107">Gunakan langkah-langkah di sini untuk membuat Tag: [tag default Arsip](https://docs.microsoft.com/microsoft-365/compliance/set-up-an-archive-and-deletion-policy-for-mailboxes#create-a-custom-archive-default-policy-tag).</span><span class="sxs-lookup"><span data-stu-id="5b925-107">Use the steps here to create the tag: [Archive Default tag](https://docs.microsoft.com/microsoft-365/compliance/set-up-an-archive-and-deletion-policy-for-mailboxes#create-a-custom-archive-default-policy-tag).</span></span>

3. <span data-ttu-id="5b925-108">Berikutnya, Tambahkan tag **Arsip** ke kebijakan penyimpanan Anda.</span><span class="sxs-lookup"><span data-stu-id="5b925-108">Next, add the **Archive** tag to your retention policy.</span></span> <span data-ttu-id="5b925-109">Di pusat admin Exchange, pilih **kebijakan penyimpanan** > Tambahkan **tag Pindahkan ke arsip** ke kebijakan > **Simpan**.</span><span class="sxs-lookup"><span data-stu-id="5b925-109">In the Exchange admin center, choose **Retention Policies** > add the **Move to Archive tag** to the policy > **Save**.</span></span>

4. <span data-ttu-id="5b925-110">Sekarang [tetapkan kebijakan penyimpanan](https://docs.microsoft.com/exchange/security-and-compliance/messaging-records-management/apply-retention-policy) ke kotak surat pengguna tertentu.</span><span class="sxs-lookup"><span data-stu-id="5b925-110">Now [Assign the Retention Policy](https://docs.microsoft.com/exchange/security-and-compliance/messaging-records-management/apply-retention-policy) to the specific user's mailbox.</span></span> <span data-ttu-id="5b925-111">Kebijakan yang sama akan diterapkan ke kotak surat **Arsip** dan **utama** .</span><span class="sxs-lookup"><span data-stu-id="5b925-111">The same policy will be applied to both the **Primary** and the **Archive** mailbox.</span></span>

<span data-ttu-id="5b925-112">Mungkin diperlukan untuk memaksa bantuan folder yang dikelola (MFA) untuk menjalankan dan menerapkan pengaturan baru ke kotak surat pengguna.</span><span class="sxs-lookup"><span data-stu-id="5b925-112">It may be necessary to force the Managed Folder Assistant (MFA) to run and apply the new settings to the user's mailbox.</span></span> <span data-ttu-id="5b925-113">Jalankan perintah berikut ini saat [tersambung ke EXO PowerShell](https://docs.microsoft.com/powershell/exchange/exchange-online/connect-to-exchange-online-powershell/connect-to-exchange-online-powershell?view=exchange-ps) untuk memulai bantuan folder yang dikelola untuk kotak surat tertentu:</span><span class="sxs-lookup"><span data-stu-id="5b925-113">Run the following command while [connected to EXO PowerShell](https://docs.microsoft.com/powershell/exchange/exchange-online/connect-to-exchange-online-powershell/connect-to-exchange-online-powershell?view=exchange-ps) to start the Managed Folder Assistant for a specific mailbox:</span></span>
  
<span data-ttu-id="5b925-114">Mulai-ManagedFolderAssistant-identitas <name of the mailbox></span><span class="sxs-lookup"><span data-stu-id="5b925-114">Start-ManagedFolderAssistant -Identity <name of the mailbox></span></span>

<span data-ttu-id="5b925-115">Untuk informasi selengkapnya tentang menyiapkan kebijakan arsip, lihat [menyetel kebijakan arsip dan penghapusan untuk kotak surat](https://docs.microsoft.com/microsoft-365/compliance/set-up-an-archive-and-deletion-policy-for-mailboxes#step-1-enable-archive-mailboxes-for-users).</span><span class="sxs-lookup"><span data-stu-id="5b925-115">For more information on setting up an archive policy, see [Set up an archive and deletion policy for mailboxes](https://docs.microsoft.com/microsoft-365/compliance/set-up-an-archive-and-deletion-policy-for-mailboxes#step-1-enable-archive-mailboxes-for-users).</span></span>
  