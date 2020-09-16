---
title: folder 1336 RecoverableItems penuh
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
- "1336"
- "3700003"
ms.assetid: a3a923e8-fece-4a26-b8b6-00970d75275e
ms.openlocfilehash: 6ae608b776332402fe333315f5e4ff6072b0a651
ms.sourcegitcommit: c6692ce0fa1358ec3529e59ca0ecdfdea4cdc759
ms.translationtype: MT
ms.contentlocale: id-ID
ms.lasthandoff: 09/14/2020
ms.locfileid: "47741270"
---
# <a name="the-recoverable-items-folder-is-full"></a><span data-ttu-id="a3cd7-102">Folder Item yang dapat dipulihkan penuh</span><span class="sxs-lookup"><span data-stu-id="a3cd7-102">The Recoverable Items folder is full</span></span>

<span data-ttu-id="a3cd7-103">Untuk kotak surat Exchange Online, batas penyimpanan default untuk folder Item yang dapat dipulihkan adalah 30 GB.</span><span class="sxs-lookup"><span data-stu-id="a3cd7-103">For Exchange Online mailboxes, the default storage limit for the Recoverable Items folder is 30 GB.</span></span> <span data-ttu-id="a3cd7-104">Batas penyimpanan untuk folder Item yang dapat dipulihkan secara otomatis ditingkatkan ke 100 GB jika kotak surat ditempatkan pada penahanan litigasi, penangguhan eDiscovery, atau ditetapkan ke kebijakan penyimpanan.</span><span class="sxs-lookup"><span data-stu-id="a3cd7-104">The storage limit for the Recoverable Items folder is automatically increased to 100 GB if the mailbox is placed on Litigation Hold, eDiscovery hold, or is assigned to a retention policy.</span></span>

<span data-ttu-id="a3cd7-105">Saat folder Item yang dapat dipulihkan mencapai batas penyimpanan, fungsionalitas kotak surat terpengaruh dengan cara berikut ini:</span><span class="sxs-lookup"><span data-stu-id="a3cd7-105">When the Recoverable Items folder reaches the storage limit, mailbox functionality is affected in the following ways:</span></span>

- <span data-ttu-id="a3cd7-106">Pengguna tidak dapat menghapus item dari kotak surat.</span><span class="sxs-lookup"><span data-stu-id="a3cd7-106">The user can't delete items from the mailbox.</span></span>

- <span data-ttu-id="a3cd7-107">Bantuan folder yang dikelola tidak dapat menghapus item berdasarkan pengaturan tag penyimpanan atau folder terkelola.</span><span class="sxs-lookup"><span data-stu-id="a3cd7-107">The Managed Folder Assistant can't delete items based on retention tag or managed folder settings.</span></span>

- <span data-ttu-id="a3cd7-108">Untuk kotak surat yang memiliki pemulihan satu item yang diaktifkan atau ditunda, proses proteksi halaman Salin pada penulisan tidak bisa mempertahankan versi item yang diedit oleh pengguna.</span><span class="sxs-lookup"><span data-stu-id="a3cd7-108">For mailboxes that have Single Item Recovery enabled or are placed on hold, the copy-on-write page protection process can't maintain versions of items edited by the user.</span></span>

- <span data-ttu-id="a3cd7-109">Untuk kotak surat yang telah mengaktifkan pembuatan log audit kotak surat, tidak ada entri log audit kotak surat yang bisa disimpan dalam subfolder audit dalam folder Item yang dapat dipulihkan.</span><span class="sxs-lookup"><span data-stu-id="a3cd7-109">For mailboxes that have mailbox audit logging enabled, no mailbox audit log entries can be saved in the Audits subfolder in the Recoverable Items folder.</span></span>

<span data-ttu-id="a3cd7-110">Untuk kotak surat yang tidak ditunda, admin dapat menggunakan `Search-Mailbox -SearchDumpsterOnly -DeleteContent` perintah di Exchange Online PowerShell untuk menghapus item di folder Item yang dapat dipulihkan.</span><span class="sxs-lookup"><span data-stu-id="a3cd7-110">For mailboxes that aren't on hold, admins can use the `Search-Mailbox -SearchDumpsterOnly -DeleteContent` command in Exchange Online PowerShell to delete items in the Recoverable Items folder.</span></span> <span data-ttu-id="a3cd7-111">Untuk informasi selengkapnya, lihat topik berikut ini:</span><span class="sxs-lookup"><span data-stu-id="a3cd7-111">For more information, see the following topics:</span></span>

- [<span data-ttu-id="a3cd7-112">Mencari dan menghapus pesan</span><span class="sxs-lookup"><span data-stu-id="a3cd7-112">Search for and delete messages</span></span>](https://docs.microsoft.com/microsoft-365/compliance/search-for-and-delete-messagesadmin-help)

- [<span data-ttu-id="a3cd7-113">Kotak surat pencarian</span><span class="sxs-lookup"><span data-stu-id="a3cd7-113">Search-Mailbox</span></span>](https://docs.microsoft.com/powershell/module/exchange/mailboxes/Search-Mailbox)

<span data-ttu-id="a3cd7-114">Untuk kotak surat yang ditangguhkan, admin harus menghapus penangguhan sebelum mereka bisa menghapus item dari folder Item yang dapat dipulihkan.</span><span class="sxs-lookup"><span data-stu-id="a3cd7-114">For mailboxes that are on hold, admins have to remove the hold before they can deleted items from the Recoverable Items folder.</span></span> <span data-ttu-id="a3cd7-115">Untuk informasi selengkapnya, lihat [menghapus item dalam folder Item yang dapat dipulihkan dari kotak surat berbasis awan yang ditahan](https://docs.microsoft.com/microsoft-365/compliance/delete-items-in-the-recoverable-items-folder-of-mailboxes-on-hold).</span><span class="sxs-lookup"><span data-stu-id="a3cd7-115">For more information, see [Delete items in the Recoverable Items folder of cloud-based mailboxes on hold](https://docs.microsoft.com/microsoft-365/compliance/delete-items-in-the-recoverable-items-folder-of-mailboxes-on-hold).</span></span>

<span data-ttu-id="a3cd7-116">Untuk membantu mencegah folder Item yang dapat dipulihkan agar tidak penuh, admin bisa menambah batas penyimpanan folder Item yang dapat dipulihkan untuk kotak surat yang ditahan dan menyiapkan kebijakan penyimpanan kotak surat yang memindahkan item dari folder Item yang dapat dipulihkan ke kotak surat arsip pengguna.</span><span class="sxs-lookup"><span data-stu-id="a3cd7-116">To help prevent the Recoverable Items folder from becoming full, admins can increase the storage limit of the Recoverable Items folder for mailboxes on hold and set up a mailbox retention policy that moves items from the Recoverable Items folder to the user's archive mailbox.</span></span> <span data-ttu-id="a3cd7-117">Lihat [menambah kuota item yang dipulihkan untuk kotak surat yang ditahan](https://docs.microsoft.com/microsoft-365/compliance/increase-the-recoverable-quota-for-mailboxes-on-hold).</span><span class="sxs-lookup"><span data-stu-id="a3cd7-117">See [Increase the Recoverable Items quota for mailboxes on hold](https://docs.microsoft.com/microsoft-365/compliance/increase-the-recoverable-quota-for-mailboxes-on-hold).</span></span>
