---
title: Mengatur balasan otomatis untuk kotak surat
ms.author: pebaum
author: pebaum
manager: mnirkhe
ms.audience: Admin
ms.topic: article
ROBOTS: NOINDEX, NOFOLLOW
localization_priority: Priority
ms.collection: Adm_O365
ms.custom:
- "9000761"
- "3514"
ms.openlocfilehash: 4ffe8d77dad7db5fd5806fe879cf4934e5ca7c4a
ms.sourcegitcommit: 89ae9e8b36d1980f89f07b016fff0ec48f96b620
ms.translationtype: HT
ms.contentlocale: id-ID
ms.lasthandoff: 04/23/2020
ms.locfileid: "43788885"
---
# <a name="set-auto-replies-for-a-users-mailbox"></a><span data-ttu-id="18ede-102">Mengatur balasan otomatis untuk kotak surat pengguna</span><span class="sxs-lookup"><span data-stu-id="18ede-102">Set auto replies for a user's mailbox</span></span>

<span data-ttu-id="18ede-103">**Metode 1**</span><span class="sxs-lookup"><span data-stu-id="18ede-103">**Method 1**</span></span>

1. <span data-ttu-id="18ede-104">Masuk ke portal Microsoft 365.</span><span class="sxs-lookup"><span data-stu-id="18ede-104">Sign in to the Microsoft 365 portal.</span></span>

2. <span data-ttu-id="18ede-105">Masuk ke **Pengguna > Pengguna aktif** (atau **Grup > Kotak surat bersama** jika Anda menetapkannya di kotak surat bersama).</span><span class="sxs-lookup"><span data-stu-id="18ede-105">Go to **Users > Active users** (or **Groups > Shared mailboxes** if you set this on a shared mailbox).</span></span>

3. <span data-ttu-id="18ede-106">Pilih pengguna yang memiliki kotak surat Microsoft Exchange.</span><span class="sxs-lookup"><span data-stu-id="18ede-106">Select a user who has a Microsoft Exchange mailbox.</span></span>

4. <span data-ttu-id="18ede-107">Pada menu fly-out di sebelah kanan, masuk ke **Pengaturan email > Balasan otomatis** (jika ini adalah kotak surat bersama, cukup klik **Balasan otomatis** pada fly-out).</span><span class="sxs-lookup"><span data-stu-id="18ede-107">On the fly-out menu on the right, go to **Mail settings > Automatic replies** (if it's a shared mailbox, just click **Automatic replies** on the fly-out).</span></span>

<span data-ttu-id="18ede-108">**Metode 2**</span><span class="sxs-lookup"><span data-stu-id="18ede-108">**Method 2**</span></span>

1. <span data-ttu-id="18ede-109">Masuk ke portal admin Microsoft 365 menggunakan kredensial administrator.</span><span class="sxs-lookup"><span data-stu-id="18ede-109">Sign in to the Microsoft 365 admin portal by using administrator credentials.</span></span>

2. <span data-ttu-id="18ede-110">Perluas **Pusat Admin**, lalu klik **Exchange**.</span><span class="sxs-lookup"><span data-stu-id="18ede-110">Expand **Admin Centers**, and then click **Exchange**.</span></span>

3. <span data-ttu-id="18ede-111">Klik gambar di sudut kanan atas, klik **Pengguna Lain**, lalu pilih kotak surat pengguna yang ingin Anda ubah.</span><span class="sxs-lookup"><span data-stu-id="18ede-111">Click the picture in the upper-right corner, click **Another User**, and then select the user mailbox that you want to change.</span></span>

4. <span data-ttu-id="18ede-112">Di sisi kiri, pilih **Opsi**, klik **Atur Email**, lalu klik **Balasan otomatis.**</span><span class="sxs-lookup"><span data-stu-id="18ede-112">On the left side, select **Options**, click **Organize E-mail**, and then click **Automatic replies.**</span></span>

<span data-ttu-id="18ede-113">**Metode 3**</span><span class="sxs-lookup"><span data-stu-id="18ede-113">**Method 3**</span></span>

<span data-ttu-id="18ede-114">Jalankan cmdlet berikut ini di Exchange Online PowerShell:</span><span class="sxs-lookup"><span data-stu-id="18ede-114">Run the following cmdlet in Exchange Online PowerShell:</span></span>

<span data-ttu-id="18ede-115">PowerShellCopy</span><span class="sxs-lookup"><span data-stu-id="18ede-115">PowerShellCopy</span></span>

```
    Set-MailboxAutoReplyConfiguration
```

<span data-ttu-id="18ede-116">Untuk informasi selengkapnya tentang cmdlet ini, lihat [Set-MailboxAutoReplyConfiguration](https://docs.microsoft.com/powershell/module/exchange/mailboxes/set-mailboxautoreplyconfiguration).</span><span class="sxs-lookup"><span data-stu-id="18ede-116">For more information about this cmdlet, see [Set-MailboxAutoReplyConfiguration](https://docs.microsoft.com/powershell/module/exchange/mailboxes/set-mailboxautoreplyconfiguration).</span></span>
