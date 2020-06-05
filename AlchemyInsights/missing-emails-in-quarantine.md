---
title: Email tidak ada di karantina
ms.author: pebaum
author: pebaum
manager: mnirkhe
ms.audience: Admin
ms.topic: article
ROBOTS: NOINDEX, NOFOLLOW
localization_priority: Normal
ms.collection: Adm_O365
ms.custom:
- "5668"
- "9002625"
ms.openlocfilehash: 61a926c363c62bc7acb5efefe42b834f33c78eb6
ms.sourcegitcommit: 8fdcd2acd31e8a4b9a8a0b91674f397d2f7889c1
ms.translationtype: MT
ms.contentlocale: id-ID
ms.lasthandoff: 06/03/2020
ms.locfileid: "44569232"
---
# <a name="missing-emails-in-quarantine"></a><span data-ttu-id="110f7-102">Email tidak ada di karantina "</span><span class="sxs-lookup"><span data-stu-id="110f7-102">Missing emails in quarantine"</span></span>

<span data-ttu-id="110f7-103">Administrator dapat [melihat, melepaskan, atau menghapus pesan ini.](https://docs.microsoft.com/microsoft-365/security/office-365-security/manage-quarantined-messages-and-files?view=o365-worldwide)</span><span class="sxs-lookup"><span data-stu-id="110f7-103">Administrators can [view, release, or delete these messages.](https://docs.microsoft.com/microsoft-365/security/office-365-security/manage-quarantined-messages-and-files?view=o365-worldwide)</span></span>

<span data-ttu-id="110f7-104">Untuk membuka pusat kepatuhan & keamanan, kunjungi [https://protection.office.com](https://protection.office.com/) .</span><span class="sxs-lookup"><span data-stu-id="110f7-104">To open the Security & Compliance Center, go to [https://protection.office.com](https://protection.office.com/).</span></span> <span data-ttu-id="110f7-105">Untuk membuka halaman karantina secara langsung, kunjungi [https://protection.office.com/quarantine](https://protection.office.com/quarantine) .</span><span class="sxs-lookup"><span data-stu-id="110f7-105">To open the Quarantine page directly, go to [https://protection.office.com/quarantine](https://protection.office.com/quarantine).</span></span>  

<span data-ttu-id="110f7-106">Anda dapat mencari dengan nilai berikut:</span><span class="sxs-lookup"><span data-stu-id="110f7-106">You can search by the following values:</span></span>  

- <span data-ttu-id="110f7-107">**Id pesan**: pengidentifikasi unik global pesan.</span><span class="sxs-lookup"><span data-stu-id="110f7-107">**Message ID**: The globally unique identifier of the message.</span></span> <span data-ttu-id="110f7-108">Jika Anda memilih pesan dalam daftar, nilai **id pesan** akan muncul di panel Flyout **rincian** yang muncul.</span><span class="sxs-lookup"><span data-stu-id="110f7-108">If you select a message in the list, the  **Message ID**  value appears in the  **Details**  flyout pane that appears.</span></span> <span data-ttu-id="110f7-109">Admin dapat menggunakan [pelacakan pesan](https://docs.microsoft.com/microsoft-365/security/office-365-security/message-trace-scc?view=o365-worldwide) untuk menemukan pesan dan nilai id pesan yang sesuai.</span><span class="sxs-lookup"><span data-stu-id="110f7-109">Admins can use [message trace](https://docs.microsoft.com/microsoft-365/security/office-365-security/message-trace-scc?view=o365-worldwide) to find messages and their corresponding Message ID values.</span></span>
- <span data-ttu-id="110f7-110">**Alamat email pengirim**: alamat email pengirim tunggal.</span><span class="sxs-lookup"><span data-stu-id="110f7-110">**Sender email address**: A single sender's email address.</span></span>
- <span data-ttu-id="110f7-111">**Alamat email penerima**: alamat email penerima tunggal.</span><span class="sxs-lookup"><span data-stu-id="110f7-111">**Recipient email address**: A single recipient's email address.</span></span>
- <span data-ttu-id="110f7-112">**Subjek**: Gunakan seluruh subjek pesan.</span><span class="sxs-lookup"><span data-stu-id="110f7-112">**Subject**: Use the entire subject of the message.</span></span> <span data-ttu-id="110f7-113">Pencarian tidak peka terhadap huruf besar-kecil.</span><span class="sxs-lookup"><span data-stu-id="110f7-113">The search is not case-sensitive.</span></span>

<span data-ttu-id="110f7-114">Setelah Anda memasukkan kriteria pencarian, klik Refresh ![ tombol ](https://docs.microsoft.com/microsoft-365/media/scc-quarantine-refresh.png?view=o365-worldwide) **refresh** untuk menyaring hasil.  </span><span class="sxs-lookup"><span data-stu-id="110f7-114">After you've entered the search criteria, click  ![Refresh button](https://docs.microsoft.com/microsoft-365/media/scc-quarantine-refresh.png?view=o365-worldwide)  **Refresh**  to filter the results.</span></span>

<span data-ttu-id="110f7-115">Cmdlet yang Anda gunakan untuk melihat dan mengelola pesan dan file dalam karantina adalah:</span><span class="sxs-lookup"><span data-stu-id="110f7-115">The cmdlets you use to view and manages messages and files in quarantine are:</span></span>
- [<span data-ttu-id="110f7-116">Hapus-QuarantineMessage</span><span class="sxs-lookup"><span data-stu-id="110f7-116">Delete-QuarantineMessage</span></span>](https://docs.microsoft.com/powershell/module/exchange/delete-quarantinemessage)
- [<span data-ttu-id="110f7-117">Ekspor-QuarantineMessage</span><span class="sxs-lookup"><span data-stu-id="110f7-117">Export-QuarantineMessage</span></span>](https://docs.microsoft.com/powershell/module/exchange/export-quarantinemessage)
- [<span data-ttu-id="110f7-118">Get-QuarantineMessage</span><span class="sxs-lookup"><span data-stu-id="110f7-118">Get-QuarantineMessage</span></span>](https://docs.microsoft.com/powershell/module/exchange/get-quarantinemessage)
- <span data-ttu-id="110f7-119">[Pratinjau-QuarantineMessage](https://docs.microsoft.com/powershell/module/exchange/preview-quarantinemessage): Perhatikan bahwa cmdlet ini hanya untuk pesan, bukan berkas MALWARE dari ATP untuk SharePoint online, OneDrive untuk bisnis, atau tim.</span><span class="sxs-lookup"><span data-stu-id="110f7-119">[Preview-QuarantineMessage](https://docs.microsoft.com/powershell/module/exchange/preview-quarantinemessage): Note that this cmdlet is only for messages, not malware files from ATP for SharePoint Online, OneDrive for Business, or Teams.</span></span>
- [<span data-ttu-id="110f7-120">Rilis-QuarantineMessage</span><span class="sxs-lookup"><span data-stu-id="110f7-120">Release-QuarantineMessage</span></span>](https://docs.microsoft.com/powershell/module/exchange/release-quarantinemessage)