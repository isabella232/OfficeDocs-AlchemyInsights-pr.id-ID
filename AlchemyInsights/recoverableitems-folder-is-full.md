---
title: 1336 RecoverableItems folder penuh
ms.author: chrisda
author: chrisda
manager: dansimp
ms.date: 11/5/2018
ms.audience: ITPro
ms.topic: article
ROBOTS: NOINDEX, NOFOLLOW
localization_priority: Normal
ms.custom:
- "1336"
- "3700003"
ms.assetid: a3a923e8-fece-4a26-b8b6-00970d75275e
ms.openlocfilehash: 05e7b47a2200c3b0500e7d786166966ea301179a
ms.sourcegitcommit: 5fb7a4b28859690020efdea630d03e70cc0e6334
ms.translationtype: MT
ms.contentlocale: id-ID
ms.lasthandoff: 06/28/2019
ms.locfileid: "35370390"
---
# <a name="the-recoverable-items-folder-is-full"></a><span data-ttu-id="85ecb-102">Folder item dapat dipulihkan ini penuh</span><span class="sxs-lookup"><span data-stu-id="85ecb-102">The Recoverable Items folder is full</span></span>

<span data-ttu-id="85ecb-103">Untuk kotak pesan Exchange Online pada Office 365, batas penyimpanan default untuk folder item dapat dipulihkan adalah 30 GB.</span><span class="sxs-lookup"><span data-stu-id="85ecb-103">For Exchange Online mailboxes in Office 365, the default storage limit for the Recoverable Items folder is 30 GB.</span></span> <span data-ttu-id="85ecb-104">Batas penyimpanan untuk folder item dapat dipulihkan secara otomatis meningkat menjadi 100 GB jika kotak pesan ditempatkan di penahanan litigasi, terus eDiscovery, atau ditetapkan ke kebijakan penyimpanan Office 365.</span><span class="sxs-lookup"><span data-stu-id="85ecb-104">The storage limit for the Recoverable Items folder is automatically increased to 100 GB if the mailbox is placed on Litigation Hold, eDiscovery hold, or is assigned to an Office 365 retention policy.</span></span>

<span data-ttu-id="85ecb-105">Ketika folder item dapat dipulihkan mencapai batas penyimpanan, fungsi kotak pesan dipengaruhi dengan cara berikut:</span><span class="sxs-lookup"><span data-stu-id="85ecb-105">When the Recoverable Items folder reaches the storage limit, mailbox functionality is affected in the following ways:</span></span>

- <span data-ttu-id="85ecb-106">Pengguna tidak dapat menghapus item dari kotak pesan.</span><span class="sxs-lookup"><span data-stu-id="85ecb-106">The user can't delete items from the mailbox.</span></span>

- <span data-ttu-id="85ecb-107">Bantuan Folder yang dikelola tidak dapat menghapus item yang didasarkan pada pengaturan folder terkelola atau tag penyimpanan.</span><span class="sxs-lookup"><span data-stu-id="85ecb-107">The Managed Folder Assistant can't delete items based on retention tag or managed folder settings.</span></span>

- <span data-ttu-id="85ecb-108">Untuk pesan yang memiliki pemulihan satu Item diaktifkan atau ditempatkan di penahanan, proses perlindungan salinan pada menulis halaman tidak mempertahankan versi item yang disunting oleh pengguna.</span><span class="sxs-lookup"><span data-stu-id="85ecb-108">For mailboxes that have Single Item Recovery enabled or are placed on hold, the copy-on-write page protection process can't maintain versions of items edited by the user.</span></span>

- <span data-ttu-id="85ecb-109">Untuk pesan yang memiliki kotak pesan yang diaktifkan pendataan audit, entri log audit kotak pesan tidak dapat disimpan dalam audit subfolder dalam folder item dapat dipulihkan.</span><span class="sxs-lookup"><span data-stu-id="85ecb-109">For mailboxes that have mailbox audit logging enabled, no mailbox audit log entries can be saved in the Audits subfolder in the Recoverable Items folder.</span></span>

<span data-ttu-id="85ecb-110">Untuk kotak pesan yang tidak ditahan, admin dapat menggunakan `Search-Mailbox -SearchDumpsterOnly -DeleteContent` perintah di Exchange Online PowerShell untuk menghapus item dalam folder item dapat dipulihkan.</span><span class="sxs-lookup"><span data-stu-id="85ecb-110">For mailboxes that aren't on hold, admins can use the `Search-Mailbox -SearchDumpsterOnly -DeleteContent` command in Exchange Online PowerShell to delete items in the Recoverable Items folder.</span></span> <span data-ttu-id="85ecb-111">Untuk informasi selengkapnya, lihat topik berikut ini:</span><span class="sxs-lookup"><span data-stu-id="85ecb-111">For more information, see the following topics:</span></span>

- [<span data-ttu-id="85ecb-112">Mencari dan menghapus pesan</span><span class="sxs-lookup"><span data-stu-id="85ecb-112">Search for and delete messages</span></span>](https://docs.microsoft.com/office365/securitycompliance/search-for-and-delete-messagesadmin-help)

- [<span data-ttu-id="85ecb-113">Search-Mailbox</span><span class="sxs-lookup"><span data-stu-id="85ecb-113">Search-Mailbox</span></span>](https://docs.microsoft.com/powershell/module/exchange/mailboxes/Search-Mailbox)

<span data-ttu-id="85ecb-114">Untuk kotak pesan yang ditahan, admin perlu menghapus penahanan sebelum mereka dapat item yang dihapus dari folder item dapat dipulihkan.</span><span class="sxs-lookup"><span data-stu-id="85ecb-114">For mailboxes that are on hold, admins have to remove the hold before they can deleted items from the Recoverable Items folder.</span></span> <span data-ttu-id="85ecb-115">Untuk informasi lebih lanjut, lihat [menghapus item dalam folder kotak pesan berbasis Internet pada menampung item dapat dipulihkan](https://docs.microsoft.com/office365/securitycompliance/delete-items-in-the-recoverable-items-folder-of-mailboxes-on-hold).</span><span class="sxs-lookup"><span data-stu-id="85ecb-115">For more information, see [Delete items in the Recoverable Items folder of cloud-based mailboxes on hold](https://docs.microsoft.com/office365/securitycompliance/delete-items-in-the-recoverable-items-folder-of-mailboxes-on-hold).</span></span>

<span data-ttu-id="85ecb-116">Untuk membantu mencegah folder item dapat dipulihkan menjadi penuh, admin dapat meningkatkan batas penyimpanan item dapat dipulihkan folder untuk kotak pesan di pegang dan mengatur kotak pesan kebijakan penyimpanan yang memindahkan item dari folder item dapat dipulihkan ke arsip pengguna kotak pesan.</span><span class="sxs-lookup"><span data-stu-id="85ecb-116">To help prevent the Recoverable Items folder from becoming full, admins can increase the storage limit of the Recoverable Items folder for mailboxes on hold and set up a mailbox retention policy that moves items from the Recoverable Items folder to the user's archive mailbox.</span></span> <span data-ttu-id="85ecb-117">Melihat [item yang dapat dipulihkan kuota untuk kotak pesan di terus meningkatkan](https://docs.microsoft.com/office365/securitycompliance/increase-the-recoverable-quota-for-mailboxes-on-hold).</span><span class="sxs-lookup"><span data-stu-id="85ecb-117">See [Increase the Recoverable Items quota for mailboxes on hold](https://docs.microsoft.com/office365/securitycompliance/increase-the-recoverable-quota-for-mailboxes-on-hold).</span></span>
