---
title: Membuat email menangkap semua
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
- "9001524"
- "3732"
ms.openlocfilehash: 262d2c6a7181d94094f3d840c4ba3ebd07000cf4
ms.sourcegitcommit: c6692ce0fa1358ec3529e59ca0ecdfdea4cdc759
ms.translationtype: MT
ms.contentlocale: id-ID
ms.lasthandoff: 09/14/2020
ms.locfileid: "47712989"
---
# <a name="create-an-email-catch-all"></a><span data-ttu-id="b5272-102">Membuat email menangkap semua</span><span class="sxs-lookup"><span data-stu-id="b5272-102">Create an email catch all</span></span>

<span data-ttu-id="b5272-103">Penggunaan menangkap semua sangat dianjurkan.</span><span class="sxs-lookup"><span data-stu-id="b5272-103">Use of a catch all is strongly discouraged.</span></span> <span data-ttu-id="b5272-104">Lebih baik untuk memberikan pentalan kembali ke pengirim yang memperbolehkan pengirim mengetahui pesan mereka tidak dapat dikirim seperti yang dibahas sehingga mereka dapat melakukan tindakan.</span><span class="sxs-lookup"><span data-stu-id="b5272-104">It is better to provide a bounce back to the sender letting senders know their message could not be delivered as addressed so they can take action.</span></span> <span data-ttu-id="b5272-105">Anda juga bisa membatasi kotak surat terpantau untuk hanya menangkap alamat email yang sebelumnya valid.</span><span class="sxs-lookup"><span data-stu-id="b5272-105">You can also limit the monitored mailbox to only catch formerly valid email addresses.</span></span> 

<span data-ttu-id="b5272-106">Setiap kotak surat menangkap semua akan menerima spam yang baik dan mungkin akhirnya mengisi jika tidak diawasi secara ketat.</span><span class="sxs-lookup"><span data-stu-id="b5272-106">Any catch all mailbox will receive a good deal of spam and may eventually fill if not closely monitored.</span></span> <span data-ttu-id="b5272-107">(Ada batas penerimaan.)</span><span class="sxs-lookup"><span data-stu-id="b5272-107">(There are receiving limits.)</span></span> 

<span data-ttu-id="b5272-108">Jika Anda memutuskan untuk melanjutkan, ikuti langkah-langkah berikut:</span><span class="sxs-lookup"><span data-stu-id="b5272-108">If you decide to proceed, follow these steps:</span></span>

1. <span data-ttu-id="b5272-109">Membuat grup distribusi dinamis & menyertakan "semua tipe Penerima."</span><span class="sxs-lookup"><span data-stu-id="b5272-109">Create a Dynamic Distribution Group & include "All Recipient Types."</span></span>

2. <span data-ttu-id="b5272-110">Membuat kotak surat khusus untuk menangkap email, misalnya, catchall@domain.com.</span><span class="sxs-lookup"><span data-stu-id="b5272-110">Create a dedicated Mailbox to catch emails, for example, catchall@domain.com.</span></span>

3. <span data-ttu-id="b5272-111">Untuk domain tertentu, atur DomainType ke "InternalRelay".</span><span class="sxs-lookup"><span data-stu-id="b5272-111">For the specific domain, set the DomainType to “InternalRelay”.</span></span> <span data-ttu-id="b5272-112">Jika nanti Anda menghapus semua tangkapan, pastikan untuk mengatur kembali domain ke otoritatif.</span><span class="sxs-lookup"><span data-stu-id="b5272-112">If you later remove the catch all, be sure to set the domain back to Authoritative.</span></span>

4. <span data-ttu-id="b5272-113">Membuat aturan transpor Mailflow sebagai berikut:</span><span class="sxs-lookup"><span data-stu-id="b5272-113">Create a Mailflow Transport Rule as follows:</span></span>

    - <span data-ttu-id="b5272-114">Jika pengirim adalah "di luar organisasi"</span><span class="sxs-lookup"><span data-stu-id="b5272-114">If the Sender is "Outside the Organization"</span></span>
    - <span data-ttu-id="b5272-115">Mengalihkan pesan ke Catchall@domain.com</span><span class="sxs-lookup"><span data-stu-id="b5272-115">Redirect the message to Catchall@domain.com</span></span>
    - <span data-ttu-id="b5272-116">Kecuali jika Penerima adalah anggota allusers@domain.com (grup distribusi berisi semua anggota)</span><span class="sxs-lookup"><span data-stu-id="b5272-116">Except if the recipient is a member of allusers@domain.com (Distribution Group contains all members)</span></span>
    - <span data-ttu-id="b5272-117">Pastikan untuk memvalidasi bahwa kotak surat baru ditambahkan ke dalam grup distribusi dinamis</span><span class="sxs-lookup"><span data-stu-id="b5272-117">Ensure to validate that new mailboxes are added into the Dynamic Distribution Group</span></span>
