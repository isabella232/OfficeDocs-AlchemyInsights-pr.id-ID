---
title: Email yang hilang dalam karantina
ms.author: pebaum
author: pebaum
manager: mnirkhe
ms.audience: Admin
ms.topic: article
ms.service: o365-administration
ROBOTS: NOINDEX, NOFOLLOW
localization_priority: Normal
ms.collection: Adm_O365
ms.custom:
- "5668"
- "9002625"
ms.openlocfilehash: 55ed9a92675939c05477fbf6d12bbedd6eb931d6
ms.sourcegitcommit: c6692ce0fa1358ec3529e59ca0ecdfdea4cdc759
ms.translationtype: MT
ms.contentlocale: id-ID
ms.lasthandoff: 09/14/2020
ms.locfileid: "47673717"
---
# <a name="missing-emails-in-quarantine"></a><span data-ttu-id="1f34a-102">Email yang hilang dalam karantina "</span><span class="sxs-lookup"><span data-stu-id="1f34a-102">Missing emails in quarantine"</span></span>

<span data-ttu-id="1f34a-103">Administrator bisa [menampilkan, melepaskan, atau menghapus pesan ini.](https://docs.microsoft.com/microsoft-365/security/office-365-security/manage-quarantined-messages-and-files?view=o365-worldwide)</span><span class="sxs-lookup"><span data-stu-id="1f34a-103">Administrators can [view, release, or delete these messages.](https://docs.microsoft.com/microsoft-365/security/office-365-security/manage-quarantined-messages-and-files?view=o365-worldwide)</span></span>

<span data-ttu-id="1f34a-104">Untuk membuka pusat kepatuhan & keamanan, masuk ke [https://protection.office.com](https://protection.office.com/) .</span><span class="sxs-lookup"><span data-stu-id="1f34a-104">To open the Security & Compliance Center, go to [https://protection.office.com](https://protection.office.com/).</span></span> <span data-ttu-id="1f34a-105">Untuk membuka halaman karantina secara langsung, masuk ke [https://protection.office.com/quarantine](https://protection.office.com/quarantine) .</span><span class="sxs-lookup"><span data-stu-id="1f34a-105">To open the Quarantine page directly, go to [https://protection.office.com/quarantine](https://protection.office.com/quarantine).</span></span>  

<span data-ttu-id="1f34a-106">Anda dapat mencari menurut nilai berikut ini:</span><span class="sxs-lookup"><span data-stu-id="1f34a-106">You can search by the following values:</span></span>  

- <span data-ttu-id="1f34a-107">**Id pesan**: pengidentifikasi pesan yang unik secara global.</span><span class="sxs-lookup"><span data-stu-id="1f34a-107">**Message ID**: The globally unique identifier of the message.</span></span> <span data-ttu-id="1f34a-108">Jika Anda memilih pesan dalam daftar, nilai  **id pesan**  muncul di panel  **rincian**  Flyout yang muncul.</span><span class="sxs-lookup"><span data-stu-id="1f34a-108">If you select a message in the list, the  **Message ID**  value appears in the  **Details**  flyout pane that appears.</span></span> <span data-ttu-id="1f34a-109">Admin dapat menggunakan [pelacakan pesan](https://docs.microsoft.com/microsoft-365/security/office-365-security/message-trace-scc?view=o365-worldwide) untuk menemukan pesan dan nilai id pesan terkait.</span><span class="sxs-lookup"><span data-stu-id="1f34a-109">Admins can use [message trace](https://docs.microsoft.com/microsoft-365/security/office-365-security/message-trace-scc?view=o365-worldwide) to find messages and their corresponding Message ID values.</span></span>
- <span data-ttu-id="1f34a-110">**Alamat email pengirim**: alamat email pengirim tunggal.</span><span class="sxs-lookup"><span data-stu-id="1f34a-110">**Sender email address**: A single sender's email address.</span></span>
- <span data-ttu-id="1f34a-111">**Alamat email penerima**: alamat email penerima tunggal.</span><span class="sxs-lookup"><span data-stu-id="1f34a-111">**Recipient email address**: A single recipient's email address.</span></span>
- <span data-ttu-id="1f34a-112">**Subjek**: Gunakan seluruh subjek pesan.</span><span class="sxs-lookup"><span data-stu-id="1f34a-112">**Subject**: Use the entire subject of the message.</span></span> <span data-ttu-id="1f34a-113">Pencarian tidak peka huruf besar-kecil.</span><span class="sxs-lookup"><span data-stu-id="1f34a-113">The search is not case-sensitive.</span></span>

<span data-ttu-id="1f34a-114">Setelah memasukkan kriteria pencarian, klik Refresh tombol refresh ![ ](https://docs.microsoft.com/microsoft-365/media/scc-quarantine-refresh.png?view=o365-worldwide) **Refresh** untuk memfilter hasil.  </span><span class="sxs-lookup"><span data-stu-id="1f34a-114">After you've entered the search criteria, click  ![Refresh button](https://docs.microsoft.com/microsoft-365/media/scc-quarantine-refresh.png?view=o365-worldwide)  **Refresh**  to filter the results.</span></span>

<span data-ttu-id="1f34a-115">Cmdlet yang Anda gunakan untuk menampilkan dan mengelola pesan dan file dalam karantina adalah:</span><span class="sxs-lookup"><span data-stu-id="1f34a-115">The cmdlets you use to view and manages messages and files in quarantine are:</span></span>
- [<span data-ttu-id="1f34a-116">Hapus-QuarantineMessage</span><span class="sxs-lookup"><span data-stu-id="1f34a-116">Delete-QuarantineMessage</span></span>](https://docs.microsoft.com/powershell/module/exchange/delete-quarantinemessage)
- [<span data-ttu-id="1f34a-117">Ekspor-QuarantineMessage</span><span class="sxs-lookup"><span data-stu-id="1f34a-117">Export-QuarantineMessage</span></span>](https://docs.microsoft.com/powershell/module/exchange/export-quarantinemessage)
- [<span data-ttu-id="1f34a-118">Dapatkan-QuarantineMessage</span><span class="sxs-lookup"><span data-stu-id="1f34a-118">Get-QuarantineMessage</span></span>](https://docs.microsoft.com/powershell/module/exchange/get-quarantinemessage)
- <span data-ttu-id="1f34a-119">[Pratinjau-QuarantineMessage](https://docs.microsoft.com/powershell/module/exchange/preview-quarantinemessage): Perhatikan bahwa cmdlet ini hanya untuk pesan, bukan file MALWARE dari ATP untuk SharePoint online, OneDrive for Business, atau teams.</span><span class="sxs-lookup"><span data-stu-id="1f34a-119">[Preview-QuarantineMessage](https://docs.microsoft.com/powershell/module/exchange/preview-quarantinemessage): Note that this cmdlet is only for messages, not malware files from ATP for SharePoint Online, OneDrive for Business, or Teams.</span></span>
- [<span data-ttu-id="1f34a-120">Rilis-QuarantineMessage</span><span class="sxs-lookup"><span data-stu-id="1f34a-120">Release-QuarantineMessage</span></span>](https://docs.microsoft.com/powershell/module/exchange/release-quarantinemessage)