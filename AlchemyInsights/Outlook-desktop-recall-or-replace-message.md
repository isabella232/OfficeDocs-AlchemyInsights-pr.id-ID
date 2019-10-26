---
title: Outlook desktop ingat atau mengganti pesan email
ms.author: daeite
author: daeite
manager: joallard
ms.date: 3/13/2019
ms.audience: Admin
ms.topic: article
ms.custom: 9000260
ROBOTS: NOINDEX, NOFOLLOW
localization_priority: Normal
ms.openlocfilehash: 3d3a6c253317137b7069a978b907c97d61bf7313
ms.sourcegitcommit: 0b06093dabd685f76cc39b1d7c0f8b03883b6e79
ms.translationtype: MT
ms.contentlocale: id-ID
ms.lasthandoff: 10/25/2019
ms.locfileid: "36496114"
---
# <a name="recall-or-replace-an-outlook-email-message"></a><span data-ttu-id="70af9-102">Ingat atau ganti pesan email Outlook</span><span class="sxs-lookup"><span data-stu-id="70af9-102">Recall or replace an Outlook email message</span></span>

- <span data-ttu-id="70af9-103">Sebagai admin, Anda dapat **memanggil kembali pesan atas nama pengguna menggunakan PowerShell**.</span><span class="sxs-lookup"><span data-stu-id="70af9-103">As the admin, you can **recall messages on behalf of users using PowerShell**.</span></span> <span data-ttu-id="70af9-104">Anda tidak dapat mengingat pesan dari Pusat admin.</span><span class="sxs-lookup"><span data-stu-id="70af9-104">You can't recall messages from the admin center.</span></span>
- <span data-ttu-id="70af9-105">Anda **hanya dapat mengingat pesan yang dikirim ke orang di organisasi Anda**.</span><span class="sxs-lookup"><span data-stu-id="70af9-105">You can **only recall messages that are sent to people in your organization**.</span></span> <span data-ttu-id="70af9-106">Jika pesan dikirim ke alamat Gmail, misalnya, Anda tidak dapat mengingatnya.</span><span class="sxs-lookup"><span data-stu-id="70af9-106">If the message was sent to a Gmail address, for example, you can't recall it.</span></span>
- <span data-ttu-id="70af9-107">Anda **hanya dapat mengingat pesan yang dikirim dari Outlook 2016 pada PC**.</span><span class="sxs-lookup"><span data-stu-id="70af9-107">You can **only recall messages sent from Outlook 2016 on the PC**.</span></span> <span data-ttu-id="70af9-108">Jika pengguna mengirim pesan menggunakan Outlook untuk Mac atau Outlook di web, Anda tidak dapat mengingatnya.</span><span class="sxs-lookup"><span data-stu-id="70af9-108">If a user sends a message using Outlook for Mac or Outlook on the web, you can't recall it.</span></span>

<span data-ttu-id="70af9-109">Untuk mengingat atau mengganti pesan email:</span><span class="sxs-lookup"><span data-stu-id="70af9-109">To recall or replace an email message:</span></span>

1. <span data-ttu-id="70af9-110">Di panel folder di sebelah kiri jendela Outlook, pilih folder Item Terkirim.</span><span class="sxs-lookup"><span data-stu-id="70af9-110">In the folder pane on the left of the Outlook window, select the Sent Items folder.</span></span>
1. <span data-ttu-id="70af9-111">Klik pesan dua kali yang ingin Anda ingat untuk membukanya.</span><span class="sxs-lookup"><span data-stu-id="70af9-111">Double-click the message you want to recall to open it.</span></span>
1. <span data-ttu-id="70af9-112">Pilih tab **pesan** , dan kemudian pilih **tindakan** > yang**ingat pesan ini**.</span><span class="sxs-lookup"><span data-stu-id="70af9-112">Select the **Message** tab, and then select **Actions** > **Recall This Message**.</span></span>
1. <span data-ttu-id="70af9-113">Pilih **Hapus salinan pesan yang belum dibaca** atau **Hapus salinan yang belum dibaca dan ganti dengan pesan baru**, lalu pilih **OK**.</span><span class="sxs-lookup"><span data-stu-id="70af9-113">Select **Delete unread copies of this message** or **Delete unread copies and replace with a new message**, and then select **OK**.</span></span>
1. <span data-ttu-id="70af9-114">Jika Anda mengirim pesan pengganti, tulis pesan, lalu pilih **kirim**.</span><span class="sxs-lookup"><span data-stu-id="70af9-114">If you're sending a replacement message, compose the message, and then select **Send**.</span></span>
1. <span data-ttu-id="70af9-115">Keberhasilan atau kegagalan pesan ingat tergantung pada pengaturan penerima di Outlook.</span><span class="sxs-lookup"><span data-stu-id="70af9-115">The success or failure of a message recall depends on the recipient's settings in Outlook.</span></span> <span data-ttu-id="70af9-116">Untuk langkah untuk memeriksa Recall, lihat [artikel ini](https://support.office.com/article/35027f88-d655-4554-b4f8-6c0729a723a0).</span><span class="sxs-lookup"><span data-stu-id="70af9-116">For steps to check on the recall, see [this article](https://support.office.com/article/35027f88-d655-4554-b4f8-6c0729a723a0).</span></span>

<span data-ttu-id="70af9-117">Mencari dan menghapus pesan email di organisasi Anda</span><span class="sxs-lookup"><span data-stu-id="70af9-117">Search for and delete email messages in your organization</span></span>

- <span data-ttu-id="70af9-118">Jika Anda bukan admin global, akun Anda harus ditambahkan ke peran pengelola eDiscovery atau peran manajemen penelusuran kepatuhan untuk mencari pesan.</span><span class="sxs-lookup"><span data-stu-id="70af9-118">If you're not a global admin, your account must be added to the eDiscovery Manager role or Compliance Search management role to search for messages.</span></span> <span data-ttu-id="70af9-119">Untuk menghapus pesan, Anda harus bergabung dengan grup peran manajemen organisasi atau peran manajemen pencarian dan pembersihan.</span><span class="sxs-lookup"><span data-stu-id="70af9-119">To delete messages, you'll need to join the Organization Management role group or the Search and Purge management role.</span></span> <span data-ttu-id="70af9-120">Izin untuk peran ini ditetapkan di [pusat keamanan dan kepatuhan](https://go.microsoft.com/fwlink/?linkid=2083731).</span><span class="sxs-lookup"><span data-stu-id="70af9-120">Permissions for these roles are assigned in the [Security and compliance center](https://go.microsoft.com/fwlink/?linkid=2083731).</span></span>
- <span data-ttu-id="70af9-121">[Membuat pencarian konten](https://docs.microsoft.com/office365/securitycompliance/content-search) untuk menemukan pesan yang akan dihapus.</span><span class="sxs-lookup"><span data-stu-id="70af9-121">[Create a content search](https://docs.microsoft.com/office365/securitycompliance/content-search) to find the message to delete.</span></span>
- <span data-ttu-id="70af9-122">[Sambungkan ke pusat keamanan dan kepatuhan PowerShell](https://docs.microsoft.com/powershell/exchange/office-365-scc/connect-to-scc-powershell/connect-to-scc-powershell?view=exchange-ps).</span><span class="sxs-lookup"><span data-stu-id="70af9-122">[Connect to Security and Compliance Center PowerShell](https://docs.microsoft.com/powershell/exchange/office-365-scc/connect-to-scc-powershell/connect-to-scc-powershell?view=exchange-ps).</span></span>

<span data-ttu-id="70af9-123">Jika Anda menggunakan otentikasi multi faktor, lihat [tersambung ke Office 365 keamanan dan kepatuhan pusat PowerShell menggunakan otentikasi multi faktor](https://docs.microsoft.com/powershell/exchange/office-365-scc/connect-to-scc-powershell/mfa-connect-to-scc-powershell?view=exchange-ps).</span><span class="sxs-lookup"><span data-stu-id="70af9-123">If you're using multi-factor authentication, see [Connect to Office 365 Security and Compliance Center PowerShell using multi-factor authentication](https://docs.microsoft.com/powershell/exchange/office-365-scc/connect-to-scc-powershell/mfa-connect-to-scc-powershell?view=exchange-ps).</span></span>