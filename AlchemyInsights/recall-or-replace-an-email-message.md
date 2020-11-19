---
title: Memanggil kembali atau mengganti pesan email
ms.author: daeite
author: daeite
manager: joallard
ms.date: 04/21/2020
ms.audience: Admin
ms.topic: article
ms.service: o365-administration
ROBOTS: NOINDEX, NOFOLLOW
localization_priority: Normal
ms.collection: Adm_O365
ms.custom:
- "1860"
- "9000260"
ms.assetid: ''
ms.openlocfilehash: 05016213a1387c5290cb5899359f1f10b5a413c0
ms.sourcegitcommit: 4e0ae808ee2a586339b396320e3edb8ba066a91a
ms.translationtype: MT
ms.contentlocale: id-ID
ms.lasthandoff: 11/19/2020
ms.locfileid: "49353509"
---
# <a name="recall-or-replace-an-email-message-in-microsoft-365"></a><span data-ttu-id="18f7d-102">Memanggil kembali atau mengganti pesan email di Microsoft 365</span><span class="sxs-lookup"><span data-stu-id="18f7d-102">Recall or replace an email message in Microsoft 365</span></span>

- <span data-ttu-id="18f7d-103">Anda **hanya bisa mengingat pesan yang dikirim ke orang di dalam organisasi Anda**.</span><span class="sxs-lookup"><span data-stu-id="18f7d-103">You can **only recall messages that are sent to people in your organization**.</span></span> <span data-ttu-id="18f7d-104">Misalnya, jika pesan dikirim ke alamat Gmail, Anda tidak dapat mengingatnya.</span><span class="sxs-lookup"><span data-stu-id="18f7d-104">For example, if the message was sent to a Gmail address, you can't recall it.</span></span>
- <span data-ttu-id="18f7d-105">Anda **hanya dapat mengingat pesan yang dikirim dari Outlook untuk PC**.</span><span class="sxs-lookup"><span data-stu-id="18f7d-105">You can **only recall messages sent from Outlook for the PC**.</span></span> <span data-ttu-id="18f7d-106">Jika pengguna mengirim pesan menggunakan Outlook untuk Mac atau Outlook di web, Anda tidak bisa mengingatnya.</span><span class="sxs-lookup"><span data-stu-id="18f7d-106">If a user sends a message using Outlook for Mac or Outlook on the web, you can't recall it.</span></span>
- <span data-ttu-id="18f7d-107">Sebagai administrator penyewa, Anda bisa **mengingat pesan atas nama pengguna menggunakan PowerShell** (untuk informasi selengkapnya, lihat: [mencari dan menghapus pesan email](https://docs.microsoft.com/microsoft-365/compliance/search-for-and-delete-messages-in-your-organization)).</span><span class="sxs-lookup"><span data-stu-id="18f7d-107">As a tenant administrator, you can **recall messages on behalf of users by using PowerShell** (For more information, see: [Search for and delete email messages](https://docs.microsoft.com/microsoft-365/compliance/search-for-and-delete-messages-in-your-organization)).</span></span>
- <span data-ttu-id="18f7d-108">Anda tidak bisa mengingat pesan dari Pusat admin.</span><span class="sxs-lookup"><span data-stu-id="18f7d-108">You can't recall messages from the admin center.</span></span> <span data-ttu-id="18f7d-109">Gulir ke bawah ke "Cari dan Hapus pesan email di organisasi Anda" untuk informasi selengkapnya.</span><span class="sxs-lookup"><span data-stu-id="18f7d-109">Scroll down to "Search for and delete email messages in your organization" for more information.</span></span>

<span data-ttu-id="18f7d-110">**Memanggil kembali atau mengganti pesan email yang Anda kirim**</span><span class="sxs-lookup"><span data-stu-id="18f7d-110">**Recall or replace an email message that you sent**</span></span>

1. <span data-ttu-id="18f7d-111">Di panel folder di sebelah kiri jendela Outlook, pilih folder Item Terkirim.</span><span class="sxs-lookup"><span data-stu-id="18f7d-111">In the folder pane on the left of the Outlook window, choose the Sent Items folder.</span></span>
2. <span data-ttu-id="18f7d-112">Buka pesan yang ingin Anda ingat.</span><span class="sxs-lookup"><span data-stu-id="18f7d-112">Open the message that you want to recall.</span></span> <span data-ttu-id="18f7d-113">Anda harus mengklik ganda untuk membuka pesan.</span><span class="sxs-lookup"><span data-stu-id="18f7d-113">You must double-click to open the message.</span></span> <span data-ttu-id="18f7d-114">Memilih pesan sehingga muncul di panel baca tidak akan memperbolehkan Anda untuk mengingat pesan.</span><span class="sxs-lookup"><span data-stu-id="18f7d-114">Selecting the message so it appears in the reading pane won't allow you to recall the message.</span></span>
3. <span data-ttu-id="18f7d-115">Dari tab Pesan, pilih **tindakan**  >  **ingat pesan ini**.</span><span class="sxs-lookup"><span data-stu-id="18f7d-115">From the Message tab, select **Actions** > **Recall This Message**.</span></span>
4. <span data-ttu-id="18f7d-116">Pilih **Hapus salinan yang belum dibaca dari pesan ini** atau **Hapus salinan yang belum dibaca dan ganti dengan pesan baru**, lalu pilih **OK**.</span><span class="sxs-lookup"><span data-stu-id="18f7d-116">Choose **Delete unread copies of this message** or **Delete unread copies and replace with a new message**, then select **OK**.</span></span>
5. <span data-ttu-id="18f7d-117">Jika Anda mengirim pesan pengganti, tulis pesan, lalu pilih **kirim**.</span><span class="sxs-lookup"><span data-stu-id="18f7d-117">If you're sending a replacement message, compose the message, then select **Send**.</span></span>
6. <span data-ttu-id="18f7d-118">Keberhasilan atau kegagalan penarikan kembali pesan bergantung pada pengaturan penerima di Outlook.</span><span class="sxs-lookup"><span data-stu-id="18f7d-118">The success or failure of a message recall depends on the recipients' settings in Outlook.</span></span>

<span data-ttu-id="18f7d-119">Untuk informasi selengkapnya, termasuk cara memeriksa penarikan kembali, lihat memanggil kembali [atau mengganti pesan email yang Anda kirim](https://support.office.com/article/35027f88-d655-4554-b4f8-6c0729a723a0).</span><span class="sxs-lookup"><span data-stu-id="18f7d-119">For more information, including how to check on the recall, see [Recall or replace an email message that you sent](https://support.office.com/article/35027f88-d655-4554-b4f8-6c0729a723a0).</span></span>

<span data-ttu-id="18f7d-120">**_Untuk mencari dan menghapus pesan email di organisasi Anda_**, sangat mudah jika Anda adalah admin global. Jika Anda bukan admin global, akun Anda harus ditambahkan ke grup peran Manajer eDiscovery, atau ke peran manajemen pencarian kepatuhan.</span><span class="sxs-lookup"><span data-stu-id="18f7d-120">**_To search for and delete email messages in your organization_**, it's easiest if you're a global admin. If you're not a global admin, your account must be added to the eDiscovery Manager role group, or to the Compliance Search management role.</span></span> <span data-ttu-id="18f7d-121">Untuk menghapus pesan, Anda harus bergabung dalam grup peran manajemen organisasi atau peran manajemen pencarian dan penghapusan.</span><span class="sxs-lookup"><span data-stu-id="18f7d-121">To delete messages, you'll need to join the Organization Management role group or the Search and Purge management role.</span></span> <span data-ttu-id="18f7d-122">Izin untuk peran ini ditetapkan di [pusat kepatuhan & keamanan](https://protection.office.com/).</span><span class="sxs-lookup"><span data-stu-id="18f7d-122">Permissions to these roles are assigned in the [Security & compliance center](https://protection.office.com/).</span></span>

1. <span data-ttu-id="18f7d-123">[Buat pencarian konten](https://docs.microsoft.com/microsoft-365/compliance/content-search) untuk menemukan pesan yang akan dihapus.</span><span class="sxs-lookup"><span data-stu-id="18f7d-123">[Create a content search](https://docs.microsoft.com/microsoft-365/compliance/content-search) to find the message to delete.</span></span>
2. <span data-ttu-id="18f7d-124">[Sambungkan ke pusat kepatuhan & keamanan PowerShell](https://docs.microsoft.com/powershell/exchange/office-365-scc/connect-to-scc-powershell/connect-to-scc-powershell).</span><span class="sxs-lookup"><span data-stu-id="18f7d-124">[Connect to Security & Compliance Center PowerShell](https://docs.microsoft.com/powershell/exchange/office-365-scc/connect-to-scc-powershell/connect-to-scc-powershell).</span></span>

<span data-ttu-id="18f7d-125">Jika Anda menggunakan MFA (multi-Factor Authentication), lihat [menyambungkan ke Microsoft 365 Security & pusat kepatuhan PowerShell menggunakan autentikasi multifaktor](https://docs.microsoft.com/powershell/exchange/office-365-scc/connect-to-scc-powershell/mfa-connect-to-scc-powershell).</span><span class="sxs-lookup"><span data-stu-id="18f7d-125">If you're using MFA (multi-factor authentication), see [Connect to Microsoft 365 Security & Compliance Center PowerShell using multi-factor authentication](https://docs.microsoft.com/powershell/exchange/office-365-scc/connect-to-scc-powershell/mfa-connect-to-scc-powershell).</span></span>
