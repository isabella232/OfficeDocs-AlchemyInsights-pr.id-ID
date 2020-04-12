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
ms.openlocfilehash: 35fe9ae76ca77faa43796b288af09be8525cb6df
ms.sourcegitcommit: 929f8accdca2b8e5be170e0fc8edd527581453d4
ms.translationtype: MT
ms.contentlocale: id-ID
ms.lasthandoff: 04/12/2020
ms.locfileid: "43232633"
---
# <a name="fix-messages-that-are-stuck-in-the-outbox"></a><span data-ttu-id="8f4db-102">Memperbaiki pesan yang terjebak di kotak keluar</span><span class="sxs-lookup"><span data-stu-id="8f4db-102">Fix messages that are stuck in the Outbox</span></span>

<span data-ttu-id="8f4db-103">Kami sarankan Anda memulai dengan menjalankan skenario ["saya mengalami masalah mengirim, menerima, atau menemukan pesan email"](https://aka.ms/SaRA-OutlookSendReceive) dari [Microsoft Support dan pemulihan asisten](https://diagnostics.office.com/#/) alat pada mesin yang terpengaruh.</span><span class="sxs-lookup"><span data-stu-id="8f4db-103">We recommend that you start by running the scenario ["I'm having problems sending, receiving, or finding email messages"](https://aka.ms/SaRA-OutlookSendReceive) from the [Microsoft Support and Recovery Assistant](https://diagnostics.office.com/#/) tool on the affected machine.</span></span>

<span data-ttu-id="8f4db-104">Saat pesan macet di kotak keluar, kemungkinan penyebabnya adalah lampiran besar atau opsi "Kirim segera saat tersambung" tidak diaktifkan.</span><span class="sxs-lookup"><span data-stu-id="8f4db-104">When a message gets stuck in your Outbox, the most likely cause is a large attachment or the option "Send immediately when connected" is not enabled.</span></span>

<span data-ttu-id="8f4db-105">**Menghapus lampiran besar**</span><span class="sxs-lookup"><span data-stu-id="8f4db-105">**Remove the large attachment**</span></span>

1. <span data-ttu-id="8f4db-106">Klik **kirim/terima** > **bekerja secara offline**.</span><span class="sxs-lookup"><span data-stu-id="8f4db-106">Click **Send / Receive** > **Work Offline**.</span></span> 
2. <span data-ttu-id="8f4db-107">Di panel navigasi, klik **kotak keluar**.</span><span class="sxs-lookup"><span data-stu-id="8f4db-107">In the navigation pane, click **Outbox**.</span></span> <span data-ttu-id="8f4db-108">Dari sini, Anda dapat:</span><span class="sxs-lookup"><span data-stu-id="8f4db-108">From here, you can:</span></span> 
    - <span data-ttu-id="8f4db-109">Hapus pesan.</span><span class="sxs-lookup"><span data-stu-id="8f4db-109">Delete the message.</span></span> <span data-ttu-id="8f4db-110">Cukup pilih dan klik **Delete**.</span><span class="sxs-lookup"><span data-stu-id="8f4db-110">Just select it and click **Delete**.</span></span>
    - <span data-ttu-id="8f4db-111">Seret pesan ke **folder draf**, klik dua kali untuk membuka pesan, dan Hapus lampiran (klik dan klik **Hapus**).</span><span class="sxs-lookup"><span data-stu-id="8f4db-111">Drag the message to your **drafts folder**, double-click to open the message, and delete the attachment (click it and click **Delete**).</span></span>
3. <span data-ttu-id="8f4db-112">Jika kesalahan memberitahu Anda Outlook mencoba untuk mengirimkan pesan, tutup Outlook.</span><span class="sxs-lookup"><span data-stu-id="8f4db-112">If an error tells you Outlook is trying to transmit the message, close Outlook.</span></span> <span data-ttu-id="8f4db-113">Mungkin perlu beberapa saat untuk keluar.</span><span class="sxs-lookup"><span data-stu-id="8f4db-113">It may take a few moments to exit.</span></span> <span data-ttu-id="8f4db-114">Jika Outlook tidak menutup, tekan **CTRL + ALT + delete** dan klik **mulai manajer tugas**.</span><span class="sxs-lookup"><span data-stu-id="8f4db-114">If Outlook doesn't close, press **Ctrl+Alt+Delete** and click **Start Task Manager**.</span></span> <span data-ttu-id="8f4db-115">Di Manajer tugas, pilih tab **proses** , gulir ke bawah ke Outlook. exe, dan klik **Akhiri proses**.</span><span class="sxs-lookup"><span data-stu-id="8f4db-115">In Task Manager, select the **Processes** tab, scroll down to outlook.exe, and click **End Process**.</span></span>
4. <span data-ttu-id="8f4db-116">Setelah menutup Outlook, mulai ulang Outlook dan ulangi langkah 2-3.</span><span class="sxs-lookup"><span data-stu-id="8f4db-116">After Outlook closes, restart Outlook and repeat steps 2-3.</span></span> 
5. <span data-ttu-id="8f4db-117">Setelah Anda menghapus lampiran, klik **kirim/terima** > **bekerja secara offline** untuk membatalkan pilihan tombol dan untuk melanjutkan kerja secara online.</span><span class="sxs-lookup"><span data-stu-id="8f4db-117">After you remove the attachment, click **Send / Receive** > **Work Offline** to deselect the button and to resume working online.</span></span> 

<span data-ttu-id="8f4db-118">Pesan juga macet di kotak keluar bila Anda mengklik **kirim**, namun Anda tidak tersambung.</span><span class="sxs-lookup"><span data-stu-id="8f4db-118">Messages also get stuck in the Outbox when you click **Send**, but you are not connected.</span></span> <span data-ttu-id="8f4db-119">Klik **kirim/terima** dan lihat tombol **bekerja offline** .</span><span class="sxs-lookup"><span data-stu-id="8f4db-119">Click **Send / Receive** and look at the **Work Offline** button.</span></span> <span data-ttu-id="8f4db-120">Jika berwarna biru, Anda akan terputus.</span><span class="sxs-lookup"><span data-stu-id="8f4db-120">If it's blue, you're disconnected.</span></span> <span data-ttu-id="8f4db-121">Klik untuk menghubungkan (tombol berubah putih) dan klik **kirim semua**.</span><span class="sxs-lookup"><span data-stu-id="8f4db-121">Click it to connect (the button turns white) and click **Send All**.</span></span>
 
<span data-ttu-id="8f4db-122">**Aktifkan kirim segera ketika terhubung**</span><span class="sxs-lookup"><span data-stu-id="8f4db-122">**Enable Send immediately when connected**</span></span>
 
1. <span data-ttu-id="8f4db-123">Pada file tab, klik **opsi**.</span><span class="sxs-lookup"><span data-stu-id="8f4db-123">On the File tab, click **Options**.</span></span>

2. <span data-ttu-id="8f4db-124">Di kotak dialog Opsi Outlook, klik **lanjut**.</span><span class="sxs-lookup"><span data-stu-id="8f4db-124">In the Outlook Options dialog box, click **Advanced**.</span></span>

3. <span data-ttu-id="8f4db-125">Di bagian kirim dan terima, klik untuk mengaktifkan **kirim segera ketika tersambung**.</span><span class="sxs-lookup"><span data-stu-id="8f4db-125">In the Send and receive section, click to enable **Send immediately when connected**.</span></span> <span data-ttu-id="8f4db-126">Klik **OK**.</span><span class="sxs-lookup"><span data-stu-id="8f4db-126">Click **OK**.</span></span>
 
<span data-ttu-id="8f4db-127">Untuk detail selengkapnya, lihat:</span><span class="sxs-lookup"><span data-stu-id="8f4db-127">For full details, see:</span></span>
- [<span data-ttu-id="8f4db-128">Video: mengirim atau menghapus email yang macet</span><span class="sxs-lookup"><span data-stu-id="8f4db-128">Video: Send or delete a stuck email</span></span>](https://support.office.com/article/Video-Send-or-delete-an-email-stuck-in-your-outbox-26d5d34a-4e5f-444a-a9e8-44db04a94dec) 
- [<span data-ttu-id="8f4db-129">Email tetap berada di folder kotak keluar sampai Anda secara manual memulai operasi kirim/terima di Outlook</span><span class="sxs-lookup"><span data-stu-id="8f4db-129">Email stays in the Outbox folder until you manually initiate a send/receive operation in Outlook</span></span>](https://support.microsoft.com/help/2797572/email-stays-in-the-outbox-folder-until-you-manually-initiate-a-send-re)
