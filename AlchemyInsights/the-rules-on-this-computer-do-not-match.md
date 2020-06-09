---
title: 'Galat: aturan pada komputer ini tidak cocok'
ms.author: pebaum
author: pebaum
manager: mnirkhe
ms.audience: ITPro
ms.topic: article
ROBOTS: NOINDEX, NOFOLLOW
localization_priority: Normal
ms.custom:
- "3518"
- "1800021"
ms.openlocfilehash: c0982da82826d1644f437b19e0d343a59d7ac473
ms.sourcegitcommit: e09af4285c6b81ca0a5320fdb811713ac25748c3
ms.translationtype: MT
ms.contentlocale: id-ID
ms.lasthandoff: 06/09/2020
ms.locfileid: "44664249"
---
# <a name="error-the-rules-on-this-computer-do-not-match"></a><span data-ttu-id="91617-102">Galat: aturan pada komputer ini tidak cocok</span><span class="sxs-lookup"><span data-stu-id="91617-102">Error: The rules on this computer do not match</span></span>

<span data-ttu-id="91617-103">Untuk melihat status diperbarui masalah ini diketahui, lihat [aturan pada komputer ini tidak cocok aturan pada Microsoft Exchange](https://support.office.com/article/d032e037-b224-429e-b325-633afde9b5f0)</span><span class="sxs-lookup"><span data-stu-id="91617-103">To see updated status of this known issue, see [The rules on this computer do not match the rules on Microsoft Exchange](https://support.office.com/article/d032e037-b224-429e-b325-633afde9b5f0)</span></span>

<span data-ttu-id="91617-104">Tim Outlook telah menerapkan perbaikan dalam membangun 12928,10000.</span><span class="sxs-lookup"><span data-stu-id="91617-104">The Outlook Team has implemented a fix in Build 12928.10000.</span></span> <span data-ttu-id="91617-105">Perbaikan ini sudah di Insider Fast dan akan pergi ke bulanan Channel pada akhir Juni 2020.</span><span class="sxs-lookup"><span data-stu-id="91617-105">The fix is already at Insider Fast and will go to Monthly Channel in late June 2020.</span></span> <span data-ttu-id="91617-106">Setelah Anda memiliki membangun tetap Anda mungkin mendapatkan prompt "aturan mana yang ingin Anda Simpan" satu terakhir kali.</span><span class="sxs-lookup"><span data-stu-id="91617-106">Once you have the fixed build you may get the prompt "Which rules do you want to keep" one last time.</span></span> <span data-ttu-id="91617-107">Pilih server ketika diminta dan kemudian kembali di Outlook dan mengaktifkan kembali aturan yang telah dinonaktifkan.</span><span class="sxs-lookup"><span data-stu-id="91617-107">Choose Server when prompted and then go back in Outlook and re-enable any rules that were disabled.</span></span>

<span data-ttu-id="91617-108">Sampai perbaikan tersedia silakan gunakan trik berikut:</span><span class="sxs-lookup"><span data-stu-id="91617-108">Until the fix is available please use the following workaround:</span></span>

<span data-ttu-id="91617-109">**Penyelesaian**: dalam laporan terbaru, masalah telah terjadi bagi mereka yang hanya membuat aturan klien di Outlook desktop.</span><span class="sxs-lookup"><span data-stu-id="91617-109">**Workaround**: In recent reports, the issue has occurred for those that have only created client rules in Outlook desktop.</span></span> <span data-ttu-id="91617-110">Jika Anda terus mengalami masalah, pertimbangkan menghapus aturan dan kemudian membuat dan mengedit aturan hanya di OWA (Outlook Web App) hingga masalah teratasi.</span><span class="sxs-lookup"><span data-stu-id="91617-110">If you continue to run into the problem, consider deleting the rules and then create and edit rules only in OWA (Outlook Web App) until the issue is resolved.</span></span>

<span data-ttu-id="91617-111">Jika Anda tidak dapat menghapus aturan secara manual Anda dapat menjalankan perintah Outlook saat Anda memulai Outlook dengan menjalankan Outlook. exe/cleanrules.</span><span class="sxs-lookup"><span data-stu-id="91617-111">If you cannot delete the rules manually you can run an Outlook command when you start Outlook by running Outlook.exe /cleanrules.</span></span> <span data-ttu-id="91617-112">Ini akan menghapus aturan klien dan server.</span><span class="sxs-lookup"><span data-stu-id="91617-112">This will delete both the client and server rules.</span></span> <span data-ttu-id="91617-113">Ini akan menghapus semua aturan untuk semua account di profil Outlook.</span><span class="sxs-lookup"><span data-stu-id="91617-113">It will delete all of the rules for all of the accounts in the Outlook Profile.</span></span> <span data-ttu-id="91617-114">Perintah ini selanjutnya didokumentasikan dalam artikel switch baris perintah.</span><span class="sxs-lookup"><span data-stu-id="91617-114">This command is further documented in the Command-line switches article.</span></span>

