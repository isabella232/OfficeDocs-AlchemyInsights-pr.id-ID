---
title: Menjalankan Diagnostik Memori Windows di Windows 10
ms.author: pebaum
author: pebaum
manager: scotv
ms.audience: Admin
ms.topic: article
ms.service: o365-administration
ROBOTS: NOINDEX, NOFOLLOW
localization_priority: Priority
ms.collection: Adm_O365
ms.custom:
- "9002959"
- "5661"
ms.openlocfilehash: ff8f80b3df4e3809e844195128f4d99cbc4667be
ms.sourcegitcommit: 8bc60ec34bc1e40685e3976576e04a2623f63a7c
ms.translationtype: MT
ms.contentlocale: id-ID
ms.lasthandoff: 04/15/2021
ms.locfileid: "51826670"
---
# <a name="run-windows-memory-diagnostics-in-windows-10"></a><span data-ttu-id="6aba1-102">Menjalankan Diagnostik Memori Windows di Windows 10</span><span class="sxs-lookup"><span data-stu-id="6aba1-102">Run Windows Memory Diagnostics in Windows 10</span></span>

<span data-ttu-id="6aba1-103">Jika Windows dan aplikasi di PC Anda mengalami crash, berhenti berfungsi, atau bekerja secara tidak stabil, Anda mungkin mengalami masalah dengan memori (RAM) PC.</span><span class="sxs-lookup"><span data-stu-id="6aba1-103">If Windows and apps on your PC are crashing, freezing, or acting in an unstable manner, you may have a problem with the PC’s memory (RAM).</span></span> <span data-ttu-id="6aba1-104">Anda dapat menjalankan Diagnostik Memori Windows untuk memeriksa masalah RAM PC.</span><span class="sxs-lookup"><span data-stu-id="6aba1-104">You can run the Windows Memory Diagnostic to check for problems with the PC’s RAM.</span></span>

<span data-ttu-id="6aba1-105">Dalam kotak pencarian di taskbar Anda, ketik **diagnostik memori**, lalu pilih Diagnostik **Memori Windows**.</span><span class="sxs-lookup"><span data-stu-id="6aba1-105">In the search box on your taskbar, type **memory diagnostic**, and then select **Windows Memory Diagnostic**.</span></span> 

<span data-ttu-id="6aba1-106">Untuk menjalankan diagnostik, PC harus dihidupkan ulang.</span><span class="sxs-lookup"><span data-stu-id="6aba1-106">To run the diagnostic, the PC needs to restart.</span></span> <span data-ttu-id="6aba1-107">Anda memiliki opsi untuk segera memulai ulang (silakan simpan pekerjaan dan tutup dokumen serta email yang terbuka terlebih dahulu), atau jadwalkan diagnostik untuk berjalan secara otomatis saat PC dimulai ulang di lain waktu:</span><span class="sxs-lookup"><span data-stu-id="6aba1-107">You have the option to restart immediately (please save your work and close open documents and e-mails first), or schedule the diagnostic to run automatically the next time the PC restarts:</span></span>

![Diagnostik Memori Windows](media/windows-memory-diagnostic.png)

<span data-ttu-id="6aba1-109">Saat PC dihidupkan ulang, Alat **Diagnostik Memori Windows akan** berjalan secara otomatis.</span><span class="sxs-lookup"><span data-stu-id="6aba1-109">When the PC restarts, the **Windows Memory Diagnostics Tool** will run automatically.</span></span> <span data-ttu-id="6aba1-110">Status dan kemajuan akan ditampilkan saat diagnostik berjalan, dan Anda memiliki opsi untuk membatalkan diagnostik dengan menekan **tombol ESC** di keyboard Anda.</span><span class="sxs-lookup"><span data-stu-id="6aba1-110">Status and progress will be displayed as the diagnostics run, and you have the option of cancelling the diagnostics by hitting the **ESC** key on your keyboard.</span></span>

<span data-ttu-id="6aba1-111">Ketika diagnostik selesai, Windows akan dimulai secara normal.</span><span class="sxs-lookup"><span data-stu-id="6aba1-111">When the diagnostics are complete, Windows will start normally.</span></span>
<span data-ttu-id="6aba1-112">Segera setelah mulai ulang, saat Desktop muncul, pemberitahuan  akan muncul (di samping ikon Pusat Tindakan di taskbar), untuk menunjukkan apakah ada kesalahan memori yang ditemukan.</span><span class="sxs-lookup"><span data-stu-id="6aba1-112">Immediately after restart, when the Desktop appears, a notification will appear (next to the **Action Center** icon on the taskbar), to indicate whether any memory errors were found.</span></span> <span data-ttu-id="6aba1-113">Misalnya:</span><span class="sxs-lookup"><span data-stu-id="6aba1-113">For example:</span></span>

<span data-ttu-id="6aba1-114">Berikut ikon Pusat Tindakan:</span><span class="sxs-lookup"><span data-stu-id="6aba1-114">Here's the Action Center icon:</span></span> ![Ikon pusat tindakan](media/action-center-icon.png) 

<span data-ttu-id="6aba1-116">Dan pemberitahuan sampel:</span><span class="sxs-lookup"><span data-stu-id="6aba1-116">And a sample notification:</span></span> ![Tidak ada kesalahan memori](media/no-memory-errors.png)

<span data-ttu-id="6aba1-118">Jika Anda melewatkan pemberitahuan, Anda bisa memilih ikon **Pusat** Tindakan pada taskbar untuk menampilkan Pusat **Tindakan** dan melihat daftar pemberitahuan yang bisa digulir.</span><span class="sxs-lookup"><span data-stu-id="6aba1-118">If you missed the notification, you can select the **Action Center** icon  on the taskbar to display the **Action Center** and see a scrollable list of notifications.</span></span>

<span data-ttu-id="6aba1-119">Untuk meninjau informasi mendetail, ketikkan **acara** ke dalam kotak pencarian di taskbar, lalu pilih **Penampil Kejadian**.</span><span class="sxs-lookup"><span data-stu-id="6aba1-119">To review detailed information, type **event** into the search box on your taskbar, and then select **Event Viewer**.</span></span> <span data-ttu-id="6aba1-120">Di panel **kiri Penampil** Kejadian, navigasikan ke Log Windows **> Sistem.**</span><span class="sxs-lookup"><span data-stu-id="6aba1-120">In the **Event Viewer**’s left-hand pane, navigate to **Windows Logs > System**.</span></span> <span data-ttu-id="6aba1-121">Di panel sebelah kanan, pindai daftar sambil  melihat kolom Sumber, hingga Anda melihat kejadian dengan nilai Sumber **MemoriDiagnostics-Hasil.**</span><span class="sxs-lookup"><span data-stu-id="6aba1-121">In the right-hand pane, scan down the list while looking at the **Source** column, until you see events with Source value **MemoryDiagnostics-Results**.</span></span> <span data-ttu-id="6aba1-122">Sorot setiap kejadian tersebut dan lihat informasi hasilnya dalam kotak di bawah tab **Umum** di bawah daftar tersebut.</span><span class="sxs-lookup"><span data-stu-id="6aba1-122">Highlight each such event and see the result information in the box under the **General** tab below the list.</span></span>
