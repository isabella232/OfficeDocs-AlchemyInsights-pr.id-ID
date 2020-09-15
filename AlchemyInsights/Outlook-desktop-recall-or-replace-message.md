---
title: Outlook desktop memanggil kembali atau mengganti pesan email
ms.author: daeite
author: daeite
manager: joallard
ms.date: 04/21/2020
ms.audience: Admin
ms.topic: article
ms.service: o365-administration
ms.custom: 9000260
ROBOTS: NOINDEX, NOFOLLOW
localization_priority: Normal
ms.openlocfilehash: 578e2690061286bde74ee0b4b74a197630716f59
ms.sourcegitcommit: c6692ce0fa1358ec3529e59ca0ecdfdea4cdc759
ms.translationtype: MT
ms.contentlocale: id-ID
ms.lasthandoff: 09/14/2020
ms.locfileid: "47663993"
---
# <a name="recall-or-replace-an-outlook-email-message"></a><span data-ttu-id="ece6d-102">Memanggil kembali atau mengganti pesan email Outlook</span><span class="sxs-lookup"><span data-stu-id="ece6d-102">Recall or replace an Outlook email message</span></span>

- <span data-ttu-id="ece6d-103">Sebagai admin, Anda dapat **memanggil kembali pesan atas nama pengguna menggunakan PowerShell**.</span><span class="sxs-lookup"><span data-stu-id="ece6d-103">As the admin, you can **recall messages on behalf of users using PowerShell**.</span></span> <span data-ttu-id="ece6d-104">Anda tidak bisa mengingat pesan dari Pusat admin.</span><span class="sxs-lookup"><span data-stu-id="ece6d-104">You can't recall messages from the admin center.</span></span>
- <span data-ttu-id="ece6d-105">Anda **hanya bisa mengingat pesan yang dikirim ke orang di dalam organisasi Anda**.</span><span class="sxs-lookup"><span data-stu-id="ece6d-105">You can **only recall messages that are sent to people in your organization**.</span></span> <span data-ttu-id="ece6d-106">Jika pesan dikirim ke alamat Gmail, misalnya, Anda tidak bisa mengingatnya.</span><span class="sxs-lookup"><span data-stu-id="ece6d-106">If the message was sent to a Gmail address, for example, you can't recall it.</span></span>
- <span data-ttu-id="ece6d-107">Anda **hanya dapat mengingat pesan yang dikirim dari Outlook 2016 di PC**.</span><span class="sxs-lookup"><span data-stu-id="ece6d-107">You can **only recall messages sent from Outlook 2016 on the PC**.</span></span> <span data-ttu-id="ece6d-108">Jika pengguna mengirim pesan menggunakan Outlook untuk Mac atau Outlook di web, Anda tidak bisa mengingatnya.</span><span class="sxs-lookup"><span data-stu-id="ece6d-108">If a user sends a message using Outlook for Mac or Outlook on the web, you can't recall it.</span></span>

<span data-ttu-id="ece6d-109">Untuk memanggil kembali atau mengganti pesan email:</span><span class="sxs-lookup"><span data-stu-id="ece6d-109">To recall or replace an email message:</span></span>

1. <span data-ttu-id="ece6d-110">Di panel folder di sebelah kiri jendela Outlook, pilih folder Item Terkirim.</span><span class="sxs-lookup"><span data-stu-id="ece6d-110">In the folder pane on the left of the Outlook window, select the Sent Items folder.</span></span>
1. <span data-ttu-id="ece6d-111">Klik ganda pesan yang ingin Anda ingat untuk membukanya.</span><span class="sxs-lookup"><span data-stu-id="ece6d-111">Double-click the message you want to recall to open it.</span></span>
1. <span data-ttu-id="ece6d-112">Pilih tab **pesan** , lalu pilih **tindakan**  >  **ingat pesan ini**.</span><span class="sxs-lookup"><span data-stu-id="ece6d-112">Select the **Message** tab, and then select **Actions** > **Recall This Message**.</span></span>
1. <span data-ttu-id="ece6d-113">Pilih **Hapus salinan yang belum dibaca dari pesan ini** atau **Hapus salinan yang belum dibaca dan ganti dengan pesan baru**, lalu pilih **OK**.</span><span class="sxs-lookup"><span data-stu-id="ece6d-113">Select **Delete unread copies of this message** or **Delete unread copies and replace with a new message**, and then select **OK**.</span></span>
1. <span data-ttu-id="ece6d-114">Jika Anda mengirim pesan pengganti, tulis pesan, lalu pilih **kirim**.</span><span class="sxs-lookup"><span data-stu-id="ece6d-114">If you're sending a replacement message, compose the message, and then select **Send**.</span></span>
1. <span data-ttu-id="ece6d-115">Keberhasilan atau kegagalan penarikan kembali pesan bergantung pada pengaturan penerima di Outlook.</span><span class="sxs-lookup"><span data-stu-id="ece6d-115">The success or failure of a message recall depends on the recipient's settings in Outlook.</span></span> <span data-ttu-id="ece6d-116">Untuk langkah-langkah untuk memeriksa penarikan kembali, lihat [artikel ini](https://support.office.com/article/35027f88-d655-4554-b4f8-6c0729a723a0).</span><span class="sxs-lookup"><span data-stu-id="ece6d-116">For steps to check on the recall, see [this article](https://support.office.com/article/35027f88-d655-4554-b4f8-6c0729a723a0).</span></span>

<span data-ttu-id="ece6d-117">Mencari dan menghapus pesan email di organisasi Anda</span><span class="sxs-lookup"><span data-stu-id="ece6d-117">Search for and delete email messages in your organization</span></span>

- <span data-ttu-id="ece6d-118">Jika Anda bukan admin global, akun Anda harus ditambahkan ke peran Manajer eDiscovery atau peran manajemen pencarian kepatuhan untuk mencari pesan.</span><span class="sxs-lookup"><span data-stu-id="ece6d-118">If you're not a global admin, your account must be added to the eDiscovery Manager role or Compliance Search management role to search for messages.</span></span> <span data-ttu-id="ece6d-119">Untuk menghapus pesan, Anda harus bergabung dalam grup peran manajemen organisasi atau peran manajemen pencarian dan penghapusan.</span><span class="sxs-lookup"><span data-stu-id="ece6d-119">To delete messages, you'll need to join the Organization Management role group or the Search and Purge management role.</span></span> <span data-ttu-id="ece6d-120">Izin untuk peran ini ditetapkan di [pusat keamanan dan kepatuhan](https://go.microsoft.com/fwlink/?linkid=2083731).</span><span class="sxs-lookup"><span data-stu-id="ece6d-120">Permissions for these roles are assigned in the [Security and compliance center](https://go.microsoft.com/fwlink/?linkid=2083731).</span></span>
- <span data-ttu-id="ece6d-121">[Buat pencarian konten](https://docs.microsoft.com/microsoft-365/compliance/content-search) untuk menemukan pesan yang akan dihapus.</span><span class="sxs-lookup"><span data-stu-id="ece6d-121">[Create a content search](https://docs.microsoft.com/microsoft-365/compliance/content-search) to find the message to delete.</span></span>
- <span data-ttu-id="ece6d-122">[Sambungkan ke pusat keamanan dan kepatuhan PowerShell](https://docs.microsoft.com/powershell/exchange/office-365-scc/connect-to-scc-powershell/connect-to-scc-powershell?view=exchange-ps).</span><span class="sxs-lookup"><span data-stu-id="ece6d-122">[Connect to Security and Compliance Center PowerShell](https://docs.microsoft.com/powershell/exchange/office-365-scc/connect-to-scc-powershell/connect-to-scc-powershell?view=exchange-ps).</span></span>

<span data-ttu-id="ece6d-123">Jika Anda menggunakan autentikasi multifaktor, lihat [menyambungkan ke Microsoft 365 Security and Compliance Center PowerShell menggunakan autentikasi multifaktor](https://docs.microsoft.com/powershell/exchange/office-365-scc/connect-to-scc-powershell/mfa-connect-to-scc-powershell?view=exchange-ps).</span><span class="sxs-lookup"><span data-stu-id="ece6d-123">If you're using multi-factor authentication, see [Connect to Microsoft 365 security and Compliance Center PowerShell using multi-factor authentication](https://docs.microsoft.com/powershell/exchange/office-365-scc/connect-to-scc-powershell/mfa-connect-to-scc-powershell?view=exchange-ps).</span></span>