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
- "9002385"
- "4645"
ms.openlocfilehash: 4f69de167dc51961fa7cf71b4d73ca7ee3ed4d55
ms.sourcegitcommit: 57fb994ddd3854d06faa67680c971b003b06bf83
ms.translationtype: MT
ms.contentlocale: id-ID
ms.lasthandoff: 04/13/2020
ms.locfileid: "43241255"
---
# <a name="fix-messages-that-are-stuck-in-the-outbox"></a><span data-ttu-id="fd1c6-102">Memperbaiki pesan yang terjebak di kotak keluar</span><span class="sxs-lookup"><span data-stu-id="fd1c6-102">Fix messages that are stuck in the Outbox</span></span>

<span data-ttu-id="fd1c6-103">Kami sarankan Anda memulai dengan menjalankan skenario ["saya mengalami masalah mengirim, menerima, atau menemukan pesan email"](https://aka.ms/SaRA-OutlookSendReceive) dari [Microsoft dukungan dan pemulihan asisten](https://diagnostics.office.com/#/) alat.</span><span class="sxs-lookup"><span data-stu-id="fd1c6-103">We recommend that you start by running the scenario ["I'm having problems sending, receiving, or finding email messages"](https://aka.ms/SaRA-OutlookSendReceive) from the [Microsoft Support and Recovery Assistant](https://diagnostics.office.com/#/) tool.</span></span>

<span data-ttu-id="fd1c6-104">Saat pesan macet di kotak keluar, kemungkinan penyebabnya adalah lampiran besar atau opsi "Kirim segera saat tersambung" tidak diaktifkan.</span><span class="sxs-lookup"><span data-stu-id="fd1c6-104">When a message gets stuck in your Outbox, the most likely cause is a large attachment or the option "Send immediately when connected" is not enabled.</span></span>

<span data-ttu-id="fd1c6-105">**Menghapus lampiran besar**</span><span class="sxs-lookup"><span data-stu-id="fd1c6-105">**Remove the large attachment**</span></span>

1. <span data-ttu-id="fd1c6-106">Di Outlook, pilih **kirim/terima** > **bekerja secara offline**.</span><span class="sxs-lookup"><span data-stu-id="fd1c6-106">In Outlook, select **Send / Receive** > **Work Offline**.</span></span> 
2. <span data-ttu-id="fd1c6-107">Di panel navigasi, pilih **kotak keluar**.</span><span class="sxs-lookup"><span data-stu-id="fd1c6-107">In the navigation pane, select **Outbox**.</span></span> <span data-ttu-id="fd1c6-108">Dari sini, Anda dapat:</span><span class="sxs-lookup"><span data-stu-id="fd1c6-108">From here, you can:</span></span> 
    - <span data-ttu-id="fd1c6-109">Hapus pesan (pilih dan pilih **Hapus**).</span><span class="sxs-lookup"><span data-stu-id="fd1c6-109">Delete the message (select it and then select **Delete**).</span></span>
    - <span data-ttu-id="fd1c6-110">Seret pesan ke folder draf, klik dua kali untuk membukanya, dan Hapus lampiran memilihnya lalu pilih **Hapus**).</span><span class="sxs-lookup"><span data-stu-id="fd1c6-110">Drag the message to your Drafts folder, double-click to open it, and remove the attachment select it and then select **Delete**).</span></span>
3. <span data-ttu-id="fd1c6-111">Jika Anda menerima galat yang mengatakan Outlook mencoba untuk mengirimkan pesan, tutup Outlook.</span><span class="sxs-lookup"><span data-stu-id="fd1c6-111">If you receive an error that says Outlook is trying to transmit the message, close Outlook.</span></span> <span data-ttu-id="fd1c6-112">Mungkin perlu beberapa saat untuk keluar.</span><span class="sxs-lookup"><span data-stu-id="fd1c6-112">It may take a few moments to exit.</span></span> <span data-ttu-id="fd1c6-113">Jika Outlook tidak menutup, tekan CTRL + ALT + delete dan pilih **mulai pengelola tugas**.</span><span class="sxs-lookup"><span data-stu-id="fd1c6-113">If Outlook doesn't close, press Ctrl+Alt+Delete and select **Start Task Manager**.</span></span> <span data-ttu-id="fd1c6-114">Di Manajer tugas, pilih tab **proses** , gulir ke bawah ke Outlook. exe, dan pilih **Akhiri proses**.</span><span class="sxs-lookup"><span data-stu-id="fd1c6-114">In Task Manager, select the **Processes** tab, scroll down to outlook.exe, and select **End Process**.</span></span>
4. <span data-ttu-id="fd1c6-115">Setelah menutup Outlook, mulai ulang dan ulangi langkah 2 dan 3.</span><span class="sxs-lookup"><span data-stu-id="fd1c6-115">After Outlook closes, restart it and repeat steps 2 and 3.</span></span> 
5. <span data-ttu-id="fd1c6-116">Setelah Anda menghapus lampiran, klik **kirim/terima** > **bekerja secara offline** untuk melanjutkan kerja online.</span><span class="sxs-lookup"><span data-stu-id="fd1c6-116">After you remove the attachment, click **Send / Receive** > **Work Offline** to resume working online.</span></span> 

<span data-ttu-id="fd1c6-117">Pesan juga macet di kotak keluar bila Anda mengklik **kirim**, namun Anda tidak tersambung.</span><span class="sxs-lookup"><span data-stu-id="fd1c6-117">Messages also get stuck in the Outbox when you click **Send**, but you are not connected.</span></span> <span data-ttu-id="fd1c6-118">Klik **kirim/terima** dan lihat tombol **bekerja offline** .</span><span class="sxs-lookup"><span data-stu-id="fd1c6-118">Click **Send / Receive** and look at the **Work Offline** button.</span></span> <span data-ttu-id="fd1c6-119">Jika berwarna biru, Anda akan terputus.</span><span class="sxs-lookup"><span data-stu-id="fd1c6-119">If it's blue, you're disconnected.</span></span> <span data-ttu-id="fd1c6-120">Klik untuk menghubungkan (tombol berubah putih) dan klik **kirim semua**.</span><span class="sxs-lookup"><span data-stu-id="fd1c6-120">Click it to connect (the button turns white) and click **Send All**.</span></span>
 
<span data-ttu-id="fd1c6-121">**Aktifkan kirim segera ketika terhubung**</span><span class="sxs-lookup"><span data-stu-id="fd1c6-121">**Enable Send immediately when connected**</span></span>
 
1. <span data-ttu-id="fd1c6-122">Pada file tab, klik **opsi**.</span><span class="sxs-lookup"><span data-stu-id="fd1c6-122">On the File tab, click **Options**.</span></span>

2. <span data-ttu-id="fd1c6-123">Di kotak dialog Opsi Outlook, klik **lanjut**.</span><span class="sxs-lookup"><span data-stu-id="fd1c6-123">In the Outlook Options dialog box, click **Advanced**.</span></span>

3. <span data-ttu-id="fd1c6-124">Di bagian kirim dan terima, klik untuk mengaktifkan **kirim segera ketika tersambung**.</span><span class="sxs-lookup"><span data-stu-id="fd1c6-124">In the Send and receive section, click to enable **Send immediately when connected**.</span></span> <span data-ttu-id="fd1c6-125">Klik **OK**.</span><span class="sxs-lookup"><span data-stu-id="fd1c6-125">Click **OK**.</span></span>
 
<span data-ttu-id="fd1c6-126">Untuk detail selengkapnya, lihat:</span><span class="sxs-lookup"><span data-stu-id="fd1c6-126">For full details, see:</span></span>
- [<span data-ttu-id="fd1c6-127">Video: mengirim atau menghapus email yang macet</span><span class="sxs-lookup"><span data-stu-id="fd1c6-127">Video: Send or delete a stuck email</span></span>](https://support.office.com/article/Video-Send-or-delete-an-email-stuck-in-your-outbox-26d5d34a-4e5f-444a-a9e8-44db04a94dec) 
- [<span data-ttu-id="fd1c6-128">Email tetap berada di folder kotak keluar sampai Anda secara manual memulai operasi kirim/terima di Outlook</span><span class="sxs-lookup"><span data-stu-id="fd1c6-128">Email stays in the Outbox folder until you manually initiate a send/receive operation in Outlook</span></span>](https://support.microsoft.com/help/2797572/email-stays-in-the-outbox-folder-until-you-manually-initiate-a-send-re)
