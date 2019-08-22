---
title: Ingat Desktop Outlook atau mengganti pesan email
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
ms.sourcegitcommit: 1d98db8acb9959aba3b5e308a567ade6b62da56c
ms.translationtype: MT
ms.contentlocale: id-ID
ms.lasthandoff: 08/22/2019
ms.locfileid: "36496114"
---
# <a name="recall-or-replace-an-outlook-email-message"></a><span data-ttu-id="e7e13-102">Ingat atau mengganti pesan email Outlook</span><span class="sxs-lookup"><span data-stu-id="e7e13-102">Recall or replace an Outlook email message</span></span>

- <span data-ttu-id="e7e13-103">Sebagai admin, Anda dapat **mengingat pesan atas nama pengguna menggunakan PowerShell**.</span><span class="sxs-lookup"><span data-stu-id="e7e13-103">As the admin, you can **recall messages on behalf of users using PowerShell**.</span></span> <span data-ttu-id="e7e13-104">Anda tidak bisa mengingat pesan dari di admin center.</span><span class="sxs-lookup"><span data-stu-id="e7e13-104">You can't recall messages from the admin center.</span></span>
- <span data-ttu-id="e7e13-105">Anda dapat **hanya ingat pesan yang dikirim ke pengguna di organisasi Anda**.</span><span class="sxs-lookup"><span data-stu-id="e7e13-105">You can **only recall messages that are sent to people in your organization**.</span></span> <span data-ttu-id="e7e13-106">Jika pesan dikirim ke alamat Gmail, misalnya, Anda tidak bisa mengingat itu.</span><span class="sxs-lookup"><span data-stu-id="e7e13-106">If the message was sent to a Gmail address, for example, you can't recall it.</span></span>
- <span data-ttu-id="e7e13-107">Anda dapat **hanya ingat pesan yang dikirim dari Outlook 2016 pada PC**.</span><span class="sxs-lookup"><span data-stu-id="e7e13-107">You can **only recall messages sent from Outlook 2016 on the PC**.</span></span> <span data-ttu-id="e7e13-108">Jika pengguna mengirim pesan menggunakan Outlook untuk Mac atau Outlook di web, Anda tidak bisa mengingat itu.</span><span class="sxs-lookup"><span data-stu-id="e7e13-108">If a user sends a message using Outlook for Mac or Outlook on the web, you can't recall it.</span></span>

<span data-ttu-id="e7e13-109">Untuk ingat atau mengganti pesan email:</span><span class="sxs-lookup"><span data-stu-id="e7e13-109">To recall or replace an email message:</span></span>

1. <span data-ttu-id="e7e13-110">Di panel map di sebelah kiri jendela Outlook, pilih folder Item Terkirim.</span><span class="sxs-lookup"><span data-stu-id="e7e13-110">In the folder pane on the left of the Outlook window, select the Sent Items folder.</span></span>
1. <span data-ttu-id="e7e13-111">Klik dua kali pesan yang ingin Anda ingat untuk membukanya.</span><span class="sxs-lookup"><span data-stu-id="e7e13-111">Double-click the message you want to recall to open it.</span></span>
1. <span data-ttu-id="e7e13-112">Pilih tab **pesan** , dan kemudian pilih **tindakan** > **Ingat pesan ini**.</span><span class="sxs-lookup"><span data-stu-id="e7e13-112">Select the **Message** tab, and then select **Actions** > **Recall This Message**.</span></span>
1. <span data-ttu-id="e7e13-113">Pilih **Hapus belum dibaca salinan pesan ini** atau **menghapus salinan yang belum dibaca dan menggantinya dengan pesan baru**, dan kemudian pilih **OK**.</span><span class="sxs-lookup"><span data-stu-id="e7e13-113">Select **Delete unread copies of this message** or **Delete unread copies and replace with a new message**, and then select **OK**.</span></span>
1. <span data-ttu-id="e7e13-114">Jika Anda mengirim pesan penggantian, menulis pesan, dan pilih **kirim**.</span><span class="sxs-lookup"><span data-stu-id="e7e13-114">If you're sending a replacement message, compose the message, and then select **Send**.</span></span>
1. <span data-ttu-id="e7e13-115">Keberhasilan atau kegagalan mengingat pesan tergantung pada pengaturan penerima di Outlook.</span><span class="sxs-lookup"><span data-stu-id="e7e13-115">The success or failure of a message recall depends on the recipient's settings in Outlook.</span></span> <span data-ttu-id="e7e13-116">Langkah-langkah untuk memeriksa ingat, lihat [artikel ini](https://support.office.com/article/35027f88-d655-4554-b4f8-6c0729a723a0).</span><span class="sxs-lookup"><span data-stu-id="e7e13-116">For steps to check on the recall, see [this article](https://support.office.com/article/35027f88-d655-4554-b4f8-6c0729a723a0).</span></span>

<span data-ttu-id="e7e13-117">Mencari dan menghapus pesan email di organisasi Anda</span><span class="sxs-lookup"><span data-stu-id="e7e13-117">Search for and delete email messages in your organization</span></span>

- <span data-ttu-id="e7e13-118">Jika Anda tidak global admin, akun Anda harus ditambahkan ke peran Manajer eDiscovery atau peran manajemen pencarian kepatuhan untuk mencari pesan.</span><span class="sxs-lookup"><span data-stu-id="e7e13-118">If you're not a global admin, your account must be added to the eDiscovery Manager role or Compliance Search management role to search for messages.</span></span> <span data-ttu-id="e7e13-119">Untuk menghapus pesan, Anda akan perlu untuk bergabung dengan grup peran manajemen organisasi atau peran manajemen pencarian dan pembersihan.</span><span class="sxs-lookup"><span data-stu-id="e7e13-119">To delete messages, you'll need to join the Organization Management role group or the Search and Purge management role.</span></span> <span data-ttu-id="e7e13-120">Izin untuk peran ini ditetapkan di [pusat keamanan dan kepatuhan](https://go.microsoft.com/fwlink/?linkid=2083731).</span><span class="sxs-lookup"><span data-stu-id="e7e13-120">Permissions for these roles are assigned in the [Security and compliance center](https://go.microsoft.com/fwlink/?linkid=2083731).</span></span>
- <span data-ttu-id="e7e13-121">[Buat konten pencarian](https://docs.microsoft.com/office365/securitycompliance/content-search) untuk menemukan pesan untuk menghapus.</span><span class="sxs-lookup"><span data-stu-id="e7e13-121">[Create a content search](https://docs.microsoft.com/office365/securitycompliance/content-search) to find the message to delete.</span></span>
- <span data-ttu-id="e7e13-122">[Terhubung ke keamanan dan kepatuhan pusat PowerShell](https://docs.microsoft.com/powershell/exchange/office-365-scc/connect-to-scc-powershell/connect-to-scc-powershell?view=exchange-ps).</span><span class="sxs-lookup"><span data-stu-id="e7e13-122">[Connect to Security and Compliance Center PowerShell](https://docs.microsoft.com/powershell/exchange/office-365-scc/connect-to-scc-powershell/connect-to-scc-powershell?view=exchange-ps).</span></span>

<span data-ttu-id="e7e13-123">Jika Anda menggunakan otentikasi faktor multi, lihat [tersambung ke kantor 365 keamanan dan kepatuhan pusat PowerShell menggunakan multi faktor otentikasi](https://docs.microsoft.com/powershell/exchange/office-365-scc/connect-to-scc-powershell/mfa-connect-to-scc-powershell?view=exchange-ps).</span><span class="sxs-lookup"><span data-stu-id="e7e13-123">If you're using multi-factor authentication, see [Connect to Office 365 Security and Compliance Center PowerShell using multi-factor authentication](https://docs.microsoft.com/powershell/exchange/office-365-scc/connect-to-scc-powershell/mfa-connect-to-scc-powershell?view=exchange-ps).</span></span>