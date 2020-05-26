---
title: Jalankan Windows Memory Diagnostics di Windows 10
ms.author: pebaum
author: pebaum
manager: mnirkhe
ms.audience: Admin
ms.topic: article
ROBOTS: NOINDEX, NOFOLLOW
localization_priority: Priority
ms.collection: Adm_O365
ms.custom:
- "9002959"
- "5661"
ms.openlocfilehash: 3fedc52d02f1f70743429d0313eda0361306c3f3
ms.sourcegitcommit: 18b080c2a5d741af01ec589158effc35ea7cf449
ms.translationtype: MT
ms.contentlocale: id-ID
ms.lasthandoff: 05/19/2020
ms.locfileid: "44357790"
---
# <a name="run-windows-memory-diagnostics-in-windows-10"></a><span data-ttu-id="cb0aa-102">Jalankan Windows Memory Diagnostics di Windows 10</span><span class="sxs-lookup"><span data-stu-id="cb0aa-102">Run Windows Memory Diagnostics in Windows 10</span></span>

<span data-ttu-id="cb0aa-103">Jika Windows dan aplikasi pada PC Anda menabrak, pembekuan, atau bertindak dengan cara yang tidak stabil, Anda mungkin memiliki masalah dengan memori PC (RAM).</span><span class="sxs-lookup"><span data-stu-id="cb0aa-103">If Windows and apps on your PC are crashing, freezing, or acting in an unstable manner, you may have a problem with the PC’s memory (RAM).</span></span> <span data-ttu-id="cb0aa-104">Anda dapat menjalankan Windows Memory Diagnostic untuk memeriksa masalah dengan RAM PC.</span><span class="sxs-lookup"><span data-stu-id="cb0aa-104">You can run the Windows Memory Diagnostic to check for problems with the PC’s RAM.</span></span>

<span data-ttu-id="cb0aa-105">Di kotak pencarian pada taskbar, ketik **diagnostik memori**, dan kemudian pilih **Windows Memory Diagnostic**.</span><span class="sxs-lookup"><span data-stu-id="cb0aa-105">In the search box on your taskbar, type **memory diagnostic**, and then select **Windows Memory Diagnostic**.</span></span> 

<span data-ttu-id="cb0aa-106">Untuk menjalankan diagnostik, PC harus me-restart.</span><span class="sxs-lookup"><span data-stu-id="cb0aa-106">To run the diagnostic, the PC needs to restart.</span></span> <span data-ttu-id="cb0aa-107">Anda memiliki pilihan untuk me-restart segera (silahkan menyimpan pekerjaan Anda dan menutup dokumen terbuka dan e-mail pertama), atau menjadwalkan diagnostik untuk menjalankan secara otomatis pada saat PC restart berikutnya:</span><span class="sxs-lookup"><span data-stu-id="cb0aa-107">You have the option to restart immediately (please save your work and close open documents and e-mails first), or schedule the diagnostic to run automatically the next time the PC restarts:</span></span>

![Diagnostik memori Windows](media/windows-memory-diagnostic.png)

<span data-ttu-id="cb0aa-109">Ketika PC dimulai ulang, **alat diagnostik memori Windows** akan berjalan secara otomatis.</span><span class="sxs-lookup"><span data-stu-id="cb0aa-109">When the PC restarts, the **Windows Memory Diagnostics Tool** will run automatically.</span></span> <span data-ttu-id="cb0aa-110">Status dan kemajuan akan ditampilkan sebagai menjalankan diagnostik, dan Anda memiliki pilihan untuk membatalkan diagnostik dengan menekan tombol **ESC** pada keyboard Anda.</span><span class="sxs-lookup"><span data-stu-id="cb0aa-110">Status and progress will be displayed as the diagnostics run, and you have the option of cancelling the diagnostics by hitting the **ESC** key on your keyboard.</span></span>

<span data-ttu-id="cb0aa-111">Ketika diagnostik selesai, Windows akan mulai normal.</span><span class="sxs-lookup"><span data-stu-id="cb0aa-111">When the diagnostics are complete, Windows will start normally.</span></span>
<span data-ttu-id="cb0aa-112">Segera setelah restart, saat desktop muncul, pemberitahuan akan muncul (di sebelah ikon **Action Center** pada taskbar), untuk menunjukkan apakah ada kesalahan memori yang ditemukan.</span><span class="sxs-lookup"><span data-stu-id="cb0aa-112">Immediately after restart, when the Desktop appears, a notification will appear (next to the **Action Center** icon on the taskbar), to indicate whether any memory errors were found.</span></span> <span data-ttu-id="cb0aa-113">Misalnya:</span><span class="sxs-lookup"><span data-stu-id="cb0aa-113">For example:</span></span>

<span data-ttu-id="cb0aa-114">Inilah ikon Action Center:</span><span class="sxs-lookup"><span data-stu-id="cb0aa-114">Here's the Action Center icon:</span></span> ![Ikon pusat aksi](media/action-center-icon.png) 

<span data-ttu-id="cb0aa-116">Dan contoh pemberitahuan:</span><span class="sxs-lookup"><span data-stu-id="cb0aa-116">And a sample notification:</span></span> ![Tidak ada kesalahan memori](media/no-memory-errors.png)

<span data-ttu-id="cb0aa-118">Jika Anda melewatkan pemberitahuan, Anda dapat memilih ikon **pusat aksi** di taskbar untuk menampilkan **pusat aksi** dan melihat daftar pemberitahuan digulir.</span><span class="sxs-lookup"><span data-stu-id="cb0aa-118">If you missed the notification, you can select the **Action Center** icon  on the taskbar to display the **Action Center** and see a scrollable list of notifications.</span></span>

<span data-ttu-id="cb0aa-119">Untuk meninjau informasi rinci, ketik **peristiwa** ke kotak pencarian di bilah tugas, dan kemudian pilih **peraga peristiwa**.</span><span class="sxs-lookup"><span data-stu-id="cb0aa-119">To review detailed information, type **event** into the search box on your taskbar, and then select **Event Viewer**.</span></span> <span data-ttu-id="cb0aa-120">Di panel sebelah kiri **penampil acara**, navigasikan ke **log Windows > sistem**.</span><span class="sxs-lookup"><span data-stu-id="cb0aa-120">In the **Event Viewer**’s left-hand pane, navigate to **Windows Logs > System**.</span></span> <span data-ttu-id="cb0aa-121">Di panel sebelah kanan, Pindai daftar sambil melihat kolom **sumber** , sampai Anda lihat peristiwa dengan nilai sumber **memorydiagnostics-hasil**.</span><span class="sxs-lookup"><span data-stu-id="cb0aa-121">In the right-hand pane, scan down the list while looking at the **Source** column, until you see events with Source value **MemoryDiagnostics-Results**.</span></span> <span data-ttu-id="cb0aa-122">Sorot setiap acara tersebut dan lihat informasi hasil di kotak di bawah tab **umum** di bawah daftar.</span><span class="sxs-lookup"><span data-stu-id="cb0aa-122">Highlight each such event and see the result information in the box under the **General** tab below the list.</span></span>
