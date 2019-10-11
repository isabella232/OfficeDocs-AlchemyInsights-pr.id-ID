---
title: Terjebak dalam outbox karena lampiran besar
ms.author: pebaum
author: pebaum
manager: mnirkhe
ms.audience: Admin
ms.topic: article
ROBOTS: NOINDEX, NOFOLLOW
localization_priority: Normal
ms.collection: Adm_O365
ms.custom:
- "2713"
- "9000768"
ms.openlocfilehash: d5fb20fcc146be67c5a04de0640ed4efd625311a
ms.sourcegitcommit: 8004ee243b5c68ff9532224a2e6c69dda0abbd0b
ms.translationtype: MT
ms.contentlocale: id-ID
ms.lasthandoff: 10/10/2019
ms.locfileid: "37441309"
---
# <a name="fix-messages-that-are-stuck-in-the-outbox"></a><span data-ttu-id="035c1-102">Memperbaiki pesan yang terjebak di kotak keluar</span><span class="sxs-lookup"><span data-stu-id="035c1-102">Fix messages that are stuck in the Outbox</span></span>

<span data-ttu-id="035c1-103">Kami sarankan Anda memulai dengan menjalankan skenario ["saya mengalami masalah mengirim, menerima, atau menemukan pesan email"](https://aka.ms/SaRA-OutlookSendReceive) dari [Microsoft dukungan dan pemulihan asisten](https://diagnostics.office.com/#/) alat.</span><span class="sxs-lookup"><span data-stu-id="035c1-103">We recommend that you start by running the scenario ["I’m having problems sending, receiving, or finding email messages"](https://aka.ms/SaRA-OutlookSendReceive) from the [Microsoft Support and Recovery Assistant](https://diagnostics.office.com/#/) tool.</span></span>

<span data-ttu-id="035c1-104">Saat pesan macet di kotak keluar, kemungkinan penyebabnya adalah:</span><span class="sxs-lookup"><span data-stu-id="035c1-104">When a message gets stuck in your Outbox, the most likely causes are:</span></span>
- <span data-ttu-id="035c1-105">Lampiran besar.</span><span class="sxs-lookup"><span data-stu-id="035c1-105">Large attachments.</span></span>
- <span data-ttu-id="035c1-106">**Kirim segera ketika opsi tersambung** tidak diaktifkan.</span><span class="sxs-lookup"><span data-stu-id="035c1-106">The **Send immediately when connected** option is not enabled.</span></span>

<span data-ttu-id="035c1-107">Untuk menghapus lampiran berukuran besar:</span><span class="sxs-lookup"><span data-stu-id="035c1-107">To remove large attachments:</span></span> 

1. <span data-ttu-id="035c1-108">Di Outlook, pilih **kirim/terima** > **bekerja secara offline**.</span><span class="sxs-lookup"><span data-stu-id="035c1-108">In Outlook, select **Send / Receive** > **Work Offline**.</span></span> 
2. <span data-ttu-id="035c1-109">Di panel navigasi, pilih **kotak keluar**.</span><span class="sxs-lookup"><span data-stu-id="035c1-109">In the navigation pane, select **Outbox**.</span></span> <span data-ttu-id="035c1-110">Dari sini, Anda dapat:</span><span class="sxs-lookup"><span data-stu-id="035c1-110">From here, you can:</span></span> 
    - <span data-ttu-id="035c1-111">Hapus pesan (pilih dan pilih **Hapus**).</span><span class="sxs-lookup"><span data-stu-id="035c1-111">Delete the message (select it and then select **Delete**).</span></span>
    - <span data-ttu-id="035c1-112">Seret pesan ke folder draf, klik dua kali untuk membukanya, dan Hapus lampiran memilihnya lalu pilih **Hapus**).</span><span class="sxs-lookup"><span data-stu-id="035c1-112">Drag the message to your Drafts folder, double-click to open it, and remove the attachment select it and then select **Delete**).</span></span>
3. <span data-ttu-id="035c1-113">Jika Anda menerima galat yang mengatakan Outlook mencoba untuk mengirimkan pesan, tutup Outlook.</span><span class="sxs-lookup"><span data-stu-id="035c1-113">If you receive an error that says Outlook is trying to transmit the message, close Outlook.</span></span> <span data-ttu-id="035c1-114">Mungkin perlu beberapa saat untuk keluar.</span><span class="sxs-lookup"><span data-stu-id="035c1-114">It may take a few moments to exit.</span></span> <span data-ttu-id="035c1-115">Jika Outlook tidak menutup, tekan CTRL + ALT + delete dan pilih **mulai pengelola tugas**.</span><span class="sxs-lookup"><span data-stu-id="035c1-115">If Outlook doesn’t close, press Ctrl+Alt+Delete and select **Start Task Manager**.</span></span> <span data-ttu-id="035c1-116">Di Manajer tugas, pilih tab **proses** , gulir ke bawah ke Outlook. exe, dan pilih **Akhiri proses**.</span><span class="sxs-lookup"><span data-stu-id="035c1-116">In Task Manager, select the **Processes** tab, scroll down to outlook.exe, and select **End Process**.</span></span>
4. <span data-ttu-id="035c1-117">Setelah menutup Outlook, mulai ulang dan ulangi langkah 2 dan 3.</span><span class="sxs-lookup"><span data-stu-id="035c1-117">After Outlook closes, restart it and repeat steps 2 and 3.</span></span> 
5. <span data-ttu-id="035c1-118">Setelah Anda menghapus lampiran, klik **kirim/terima** > **bekerja secara offline** untuk melanjutkan kerja online.</span><span class="sxs-lookup"><span data-stu-id="035c1-118">After you remove the attachment, click **Send / Receive** > **Work Offline** to resume working online.</span></span> 

<span data-ttu-id="035c1-119">Pesan juga macet di kotak keluar bila Anda mengklik **kirim**, namun Anda tidak tersambung.</span><span class="sxs-lookup"><span data-stu-id="035c1-119">Messages also get stuck in the Outbox when you click **Send**, but you are not connected.</span></span> <span data-ttu-id="035c1-120">Klik **kirim/terima** dan lihat tombol **bekerja offline** .</span><span class="sxs-lookup"><span data-stu-id="035c1-120">Click **Send / Receive** and look at the **Work Offline** button.</span></span> <span data-ttu-id="035c1-121">Jika berwarna biru, Anda akan terputus.</span><span class="sxs-lookup"><span data-stu-id="035c1-121">If it's blue, you're disconnected.</span></span> <span data-ttu-id="035c1-122">Pilih untuk menghubungkan (tombol berubah putih) dan klik **kirim semua**.</span><span class="sxs-lookup"><span data-stu-id="035c1-122">Select it to connect (the button turns white) and click **Send All**.</span></span>
 
<span data-ttu-id="035c1-123">Untuk mengaktifkan **kirim segera ketika terhubung**:</span><span class="sxs-lookup"><span data-stu-id="035c1-123">To enable **Send immediately when connected**:</span></span>
 
- <span data-ttu-id="035c1-124">Pilih **file** > **Options** >  **Advanced**.</span><span class="sxs-lookup"><span data-stu-id="035c1-124">Select **File** > **Options** >  **Advanced**.</span></span>
<span data-ttu-id="035c1-125">Di bagian **mengirim dan menerima** , pilih **kirim segera ketika tersambung**, dan kemudian pilih **OK**.</span><span class="sxs-lookup"><span data-stu-id="035c1-125">In the **Send and receive** section, select **Send immediately when connected**, and then choose **OK**.</span></span>
 
<span data-ttu-id="035c1-126">Untuk detail selengkapnya, lihat:</span><span class="sxs-lookup"><span data-stu-id="035c1-126">For full details see:</span></span>
- [<span data-ttu-id="035c1-127">Video: mengirim atau menghapus email yang macet</span><span class="sxs-lookup"><span data-stu-id="035c1-127">Video: Send or delete a stuck email</span></span>](https://support.office.com/article/Video-Send-or-delete-an-email-stuck-in-your-outbox-26d5d34a-4e5f-444a-a9e8-44db04a94dec) 
- [<span data-ttu-id="035c1-128">Email tetap berada di folder kotak keluar sampai Anda secara manual memulai operasi kirim/terima di Outlook</span><span class="sxs-lookup"><span data-stu-id="035c1-128">Email stays in the Outbox folder until you manually initiate a send/receive operation in Outlook</span></span>](https://support.microsoft.com/help/2797572/email-stays-in-the-outbox-folder-until-you-manually-initiate-a-send-re)
