---
title: Ikon daya atau baterai tidak ada di Windows 10
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
- "9002953"
- "5655"
ms.openlocfilehash: 95b68cee58f88d04f02e29477b139f7f583dc0b1
ms.sourcegitcommit: 8bc60ec34bc1e40685e3976576e04a2623f63a7c
ms.translationtype: HT
ms.contentlocale: id-ID
ms.lasthandoff: 04/15/2021
ms.locfileid: "51790551"
---
# <a name="power-or-battery-icon-missing-in-windows-10"></a><span data-ttu-id="83bf2-102">Ikon daya atau baterai tidak ada di Windows 10</span><span class="sxs-lookup"><span data-stu-id="83bf2-102">Power or battery icon missing in Windows 10</span></span>

<span data-ttu-id="83bf2-103">Jika perangkat Windows 10 memiliki baterai (misalnya, laptop atau tablet, atau PC yang disambungkan melalui USB ke UPS), biasanya ikon daya/baterai ditampilkan di taskbar dekat jam, misalnya:</span><span class="sxs-lookup"><span data-stu-id="83bf2-103">If your Windows 10 device has a battery (e.g., laptop or tablet, or a PC connected via USB to a UPS), normally a power/battery icon is shown in the taskbar near the clock, for example:</span></span>

![Ikon baterai](media/battery-icon.png)

<span data-ttu-id="83bf2-105">Jika Anda tidak melihat ikon ini, ikon mungkin tersembunyi:</span><span class="sxs-lookup"><span data-stu-id="83bf2-105">If you don't see this icon, it may be hidden:</span></span>

1. <span data-ttu-id="83bf2-106">Masuk ke **[Pengaturan > Personalisasi > Taskbar](ms-settings:taskbar?activationSource=GetHelp)**.</span><span class="sxs-lookup"><span data-stu-id="83bf2-106">Go to **[Settings > Personalization > Taskbar](ms-settings:taskbar?activationSource=GetHelp)**.</span></span>

2. <span data-ttu-id="83bf2-107">Di area Pemberitahuan, klik **Pilih ikon yang muncul di taskbar**.</span><span class="sxs-lookup"><span data-stu-id="83bf2-107">In the Notification area, click **Select which icons appear on the taskbar**.</span></span>

3. <span data-ttu-id="83bf2-108">Lalu, temukan item **Daya** di daftar dan alihkan pengaturannya ke **Aktif**.</span><span class="sxs-lookup"><span data-stu-id="83bf2-108">Then find the **Power** item in the list and toggle its setting to **On**.</span></span>

    ![Menampilkan ikon daya di Taskbar](media/power-icon-on.png)

<span data-ttu-id="83bf2-110">**Pemecahan masalah**</span><span class="sxs-lookup"><span data-stu-id="83bf2-110">**Troubleshooting**</span></span>

<span data-ttu-id="83bf2-111">Jika Anda telah mengikuti instruksi di atas dan tombol alih **Daya** berwarna abu-abu atau tidak terlihat, di kotak pencarian di taskbar, ketik **device manager**, lalu pilih **Device Manager** di daftar hasil.</span><span class="sxs-lookup"><span data-stu-id="83bf2-111">If you followed the above instructions and the **Power** toggle is greyed out or not visible, in the search box on the taskbar, type **device manager**, and then select **Device Manager** in the list of results.</span></span> <span data-ttu-id="83bf2-112">Di bawah **Baterai**, klik kanan baterai perangkat Anda, klik **Nonaktifkan**, lalu klik **Ya**.</span><span class="sxs-lookup"><span data-stu-id="83bf2-112">Under **Batteries**, right-click the battery for your device, click **Disable**, and click **Yes**.</span></span> <span data-ttu-id="83bf2-113">Tunggu beberapa detik, lalu klik kanan baterai dan klik **Aktifkan**.</span><span class="sxs-lookup"><span data-stu-id="83bf2-113">Wait a few seconds, and then right-click the battery and click **Enable**.</span></span> <span data-ttu-id="83bf2-114">Lalu, hidupkan ulang perangkat Anda.</span><span class="sxs-lookup"><span data-stu-id="83bf2-114">Then restart your device.</span></span>

<span data-ttu-id="83bf2-115">Jika Anda telah mengikuti instruksi di atas, tetapi ikon baterai tidak muncul di taskbar, di kotak pencarian di taskbar, ketik **manajer tugas**, lalu klik **Manajer Tugas** di daftar hasil.</span><span class="sxs-lookup"><span data-stu-id="83bf2-115">If you followed the above instructions, but the battery icon does not appear on the taskbar, in the search box on the taskbar, type **task manager**, and then click **Task Manager** in the list of results.</span></span> <span data-ttu-id="83bf2-116">Di tab **Proses**, di bawah **Nama**, klik kanan **Explorer**, lalu klik **Hidupkan ulang**.</span><span class="sxs-lookup"><span data-stu-id="83bf2-116">On the **Processes** tab, under **Name**, right-click **Explorer**, and then click **Restart**.</span></span>
