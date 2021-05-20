---
title: Email yang hilang di karantina
ms.author: pebaum
author: pebaum
manager: scotv
ms.audience: Admin
ms.topic: article
ms.service: o365-administration
ROBOTS: NOINDEX, NOFOLLOW
localization_priority: Normal
ms.collection: Adm_O365
ms.custom:
- "5668"
- "9002625"
ms.openlocfilehash: 563f76f624f428a46894268b478cf05eb757b497
ms.sourcegitcommit: f4866e94918c7b591ad0cd3b58169d340bcc7f00
ms.translationtype: MT
ms.contentlocale: id-ID
ms.lasthandoff: 05/19/2021
ms.locfileid: "52539827"
---
# <a name="missing-emails-in-quarantine"></a><span data-ttu-id="111a1-102">Email yang hilang di karantina"</span><span class="sxs-lookup"><span data-stu-id="111a1-102">Missing emails in quarantine"</span></span>

<span data-ttu-id="111a1-103">Administrator bisa [menampilkan, merilis, atau menghapus pesan ini.](/microsoft-365/security/office-365-security/manage-quarantined-messages-and-files)</span><span class="sxs-lookup"><span data-stu-id="111a1-103">Administrators can [view, release, or delete these messages.](/microsoft-365/security/office-365-security/manage-quarantined-messages-and-files)</span></span>

<span data-ttu-id="111a1-104">Untuk membuka Pusat & Keamanan, masuk ke [https://protection.office.com](https://protection.office.com/) .</span><span class="sxs-lookup"><span data-stu-id="111a1-104">To open the Security & Compliance Center, go to [https://protection.office.com](https://protection.office.com/).</span></span> <span data-ttu-id="111a1-105">Untuk membuka halaman Karantina secara langsung, masuk ke [https://protection.office.com/quarantine](https://protection.office.com/quarantine) .</span><span class="sxs-lookup"><span data-stu-id="111a1-105">To open the Quarantine page directly, go to [https://protection.office.com/quarantine](https://protection.office.com/quarantine).</span></span>  

<span data-ttu-id="111a1-106">Anda bisa mencari dengan nilai berikut:</span><span class="sxs-lookup"><span data-stu-id="111a1-106">You can search by the following values:</span></span>  

- <span data-ttu-id="111a1-107">**ID Pesan**: Pengidentifikasi pesan secara global unik.</span><span class="sxs-lookup"><span data-stu-id="111a1-107">**Message ID**: The globally unique identifier of the message.</span></span> <span data-ttu-id="111a1-108">Jika Anda memilih pesan dalam daftar, nilai  **ID Pesan**  muncul di panel  **flyout**  Detail yang muncul.</span><span class="sxs-lookup"><span data-stu-id="111a1-108">If you select a message in the list, the  **Message ID**  value appears in the  **Details**  flyout pane that appears.</span></span> <span data-ttu-id="111a1-109">Admin dapat menggunakan jejak [pesan untuk](/microsoft-365/security/office-365-security/message-trace-scc) menemukan pesan dan nilai ID Pesan terkait.</span><span class="sxs-lookup"><span data-stu-id="111a1-109">Admins can use [message trace](/microsoft-365/security/office-365-security/message-trace-scc) to find messages and their corresponding Message ID values.</span></span>
- <span data-ttu-id="111a1-110">**Alamat email** pengirim : Alamat email pengirim tunggal.</span><span class="sxs-lookup"><span data-stu-id="111a1-110">**Sender email address**: A single sender's email address.</span></span>
- <span data-ttu-id="111a1-111">**Alamat email** penerima: Alamat email penerima tunggal.</span><span class="sxs-lookup"><span data-stu-id="111a1-111">**Recipient email address**: A single recipient's email address.</span></span>
- <span data-ttu-id="111a1-112">**Subjek**: Gunakan seluruh subjek pesan.</span><span class="sxs-lookup"><span data-stu-id="111a1-112">**Subject**: Use the entire subject of the message.</span></span> <span data-ttu-id="111a1-113">Pencarian tidak peka huruf besar/kecil.</span><span class="sxs-lookup"><span data-stu-id="111a1-113">The search is not case-sensitive.</span></span>

<span data-ttu-id="111a1-114">Setelah Anda memasukkan kriteria pencarian, klik ![ Tombol Refresh ](/microsoft-365/media/scc-quarantine-refresh.png?view=o365-worldwide) **Refresh** untuk memfilter hasil.</span><span class="sxs-lookup"><span data-stu-id="111a1-114">After you've entered the search criteria, click ![Refresh button](/microsoft-365/media/scc-quarantine-refresh.png?view=o365-worldwide) **Refresh** to filter the results.</span></span>

<span data-ttu-id="111a1-115">Cmdlets yang Anda gunakan untuk menampilkan dan mengelola pesan dan file di karantina adalah:</span><span class="sxs-lookup"><span data-stu-id="111a1-115">The cmdlets you use to view and manages messages and files in quarantine are:</span></span>
- [<span data-ttu-id="111a1-116">Delete-QuarantineMessage</span><span class="sxs-lookup"><span data-stu-id="111a1-116">Delete-QuarantineMessage</span></span>](/powershell/module/exchange/delete-quarantinemessage)
- [<span data-ttu-id="111a1-117">Export-QuarantineMessage</span><span class="sxs-lookup"><span data-stu-id="111a1-117">Export-QuarantineMessage</span></span>](/powershell/module/exchange/export-quarantinemessage)
- [<span data-ttu-id="111a1-118">Get-QuarantineMessage</span><span class="sxs-lookup"><span data-stu-id="111a1-118">Get-QuarantineMessage</span></span>](/powershell/module/exchange/get-quarantinemessage)
- <span data-ttu-id="111a1-119">[Pratinjau-KarantinaPesan:](/powershell/module/exchange/preview-quarantinemessage)Perhatikan bahwa cmdlet ini hanya untuk pesan, bukan file malware dari Pertahanan Microsoft untuk Office 365 untuk SharePoint Online, OneDrive for Business, atau Teams.</span><span class="sxs-lookup"><span data-stu-id="111a1-119">[Preview-QuarantineMessage](/powershell/module/exchange/preview-quarantinemessage): Note that this cmdlet is only for messages, not malware files from Microsoft Defender for Office 365 for SharePoint Online, OneDrive for Business, or Teams.</span></span>
- [<span data-ttu-id="111a1-120">Release-QuarantineMessage</span><span class="sxs-lookup"><span data-stu-id="111a1-120">Release-QuarantineMessage</span></span>](/powershell/module/exchange/release-quarantinemessage)