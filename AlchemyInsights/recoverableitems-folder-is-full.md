---
title: 1336 RecoverableItems folder penuh
ms.author: chrisda
author: chrisda
manager: dansimp
ms.date: 04/21/2020
ms.audience: ITPro
ms.topic: article
ROBOTS: NOINDEX, NOFOLLOW
localization_priority: Normal
ms.custom:
- "1336"
- "3700003"
ms.assetid: a3a923e8-fece-4a26-b8b6-00970d75275e
ms.openlocfilehash: fb10b792981040bdcf4661b8aff30733c2438212
ms.sourcegitcommit: 55eff703a17e500681d8fa6a87eb067019ade3cc
ms.translationtype: MT
ms.contentlocale: id-ID
ms.lasthandoff: 04/22/2020
ms.locfileid: "43720255"
---
# <a name="the-recoverable-items-folder-is-full"></a><span data-ttu-id="44157-102">Folder item dapat dipulihkan penuh</span><span class="sxs-lookup"><span data-stu-id="44157-102">The Recoverable Items folder is full</span></span>

<span data-ttu-id="44157-103">Untuk kotak surat Exchange Online, batas penyimpanan default untuk folder item dapat dipulihkan adalah 30 GB.</span><span class="sxs-lookup"><span data-stu-id="44157-103">For Exchange Online mailboxes, the default storage limit for the Recoverable Items folder is 30 GB.</span></span> <span data-ttu-id="44157-104">Batas penyimpanan untuk folder item dapat dipulihkan akan secara otomatis ditingkatkan ke 100 GB jika kotak pesan ditempatkan di penahanan litigasi, pembekuan eDiscovery, atau ditetapkan ke kebijakan penyimpanan.</span><span class="sxs-lookup"><span data-stu-id="44157-104">The storage limit for the Recoverable Items folder is automatically increased to 100 GB if the mailbox is placed on Litigation Hold, eDiscovery hold, or is assigned to a retention policy.</span></span>

<span data-ttu-id="44157-105">Bila folder item dapat dipulihkan mencapai batas penyimpanan, fungsi kotak pesan akan terpengaruh dengan cara berikut:</span><span class="sxs-lookup"><span data-stu-id="44157-105">When the Recoverable Items folder reaches the storage limit, mailbox functionality is affected in the following ways:</span></span>

- <span data-ttu-id="44157-106">Pengguna tidak dapat menghapus item dari kotak surat.</span><span class="sxs-lookup"><span data-stu-id="44157-106">The user can't delete items from the mailbox.</span></span>

- <span data-ttu-id="44157-107">Bantuan folder yang dikelola tidak dapat menghapus item berdasarkan Tag penyimpanan atau pengaturan Folder Terkelola.</span><span class="sxs-lookup"><span data-stu-id="44157-107">The Managed Folder Assistant can't delete items based on retention tag or managed folder settings.</span></span>

- <span data-ttu-id="44157-108">Untuk kotak pesan yang memiliki pemulihan satu item diaktifkan atau ditempatkan di tahan, proses perlindungan halaman salinan-on-Write tidak dapat mempertahankan versi item yang diedit oleh pengguna.</span><span class="sxs-lookup"><span data-stu-id="44157-108">For mailboxes that have Single Item Recovery enabled or are placed on hold, the copy-on-write page protection process can't maintain versions of items edited by the user.</span></span>

- <span data-ttu-id="44157-109">Untuk kotak pesan yang memiliki pencatatan audit kotak pesan aktif, tidak ada entri log audit kotak pesan yang dapat disimpan di subfolder audit dalam folder Item bisa dipulihkan.</span><span class="sxs-lookup"><span data-stu-id="44157-109">For mailboxes that have mailbox audit logging enabled, no mailbox audit log entries can be saved in the Audits subfolder in the Recoverable Items folder.</span></span>

<span data-ttu-id="44157-110">Untuk kotak pesan yang tidak di tahan, admin dapat menggunakan `Search-Mailbox -SearchDumpsterOnly -DeleteContent` perintah di Exchange Online PowerShell untuk menghapus item dalam folder item dapat dipulihkan.</span><span class="sxs-lookup"><span data-stu-id="44157-110">For mailboxes that aren't on hold, admins can use the `Search-Mailbox -SearchDumpsterOnly -DeleteContent` command in Exchange Online PowerShell to delete items in the Recoverable Items folder.</span></span> <span data-ttu-id="44157-111">Untuk informasi selengkapnya, lihat topik berikut ini:</span><span class="sxs-lookup"><span data-stu-id="44157-111">For more information, see the following topics:</span></span>

- [<span data-ttu-id="44157-112">Mencari dan menghapus pesan</span><span class="sxs-lookup"><span data-stu-id="44157-112">Search for and delete messages</span></span>](https://docs.microsoft.com/office365/securitycompliance/search-for-and-delete-messagesadmin-help)

- [<span data-ttu-id="44157-113">Kotak pesan penelusuran</span><span class="sxs-lookup"><span data-stu-id="44157-113">Search-Mailbox</span></span>](https://docs.microsoft.com/powershell/module/exchange/mailboxes/Search-Mailbox)

<span data-ttu-id="44157-114">Untuk kotak pesan yang sedang di tahan, admin harus menghapus terus sebelum mereka dapat menghapus item dari folder Item bisa dipulihkan.</span><span class="sxs-lookup"><span data-stu-id="44157-114">For mailboxes that are on hold, admins have to remove the hold before they can deleted items from the Recoverable Items folder.</span></span> <span data-ttu-id="44157-115">Untuk selengkapnya, lihat [menghapus item di folder item dapat dipulihkan dari kotak pesan berbasis Internet yang akan ditahan](https://docs.microsoft.com/office365/securitycompliance/delete-items-in-the-recoverable-items-folder-of-mailboxes-on-hold).</span><span class="sxs-lookup"><span data-stu-id="44157-115">For more information, see [Delete items in the Recoverable Items folder of cloud-based mailboxes on hold](https://docs.microsoft.com/office365/securitycompliance/delete-items-in-the-recoverable-items-folder-of-mailboxes-on-hold).</span></span>

<span data-ttu-id="44157-116">Untuk membantu mencegah folder item dapat dipulihkan menjadi penuh, admin dapat meningkatkan batas penyimpanan folder item dapat dipulihkan untuk kotak pesan yang ditangguhkan dan mengatur kebijakan retensi kotak pesan yang memindahkan item dari folder item dapat dipulihkan ke kotak pesan arsip pengguna.</span><span class="sxs-lookup"><span data-stu-id="44157-116">To help prevent the Recoverable Items folder from becoming full, admins can increase the storage limit of the Recoverable Items folder for mailboxes on hold and set up a mailbox retention policy that moves items from the Recoverable Items folder to the user's archive mailbox.</span></span> <span data-ttu-id="44157-117">Lihat [meningkatkan kuota item dapat dipulihkan untuk kotak pesan yang akan ditahan](https://docs.microsoft.com/office365/securitycompliance/increase-the-recoverable-quota-for-mailboxes-on-hold).</span><span class="sxs-lookup"><span data-stu-id="44157-117">See [Increase the Recoverable Items quota for mailboxes on hold](https://docs.microsoft.com/office365/securitycompliance/increase-the-recoverable-quota-for-mailboxes-on-hold).</span></span>
