---
title: Buat email berisi semua
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
- "9001524"
- "3732"
ms.openlocfilehash: 2b9131a620139a93ddb844fd49d8fa2ed68e52c2
ms.sourcegitcommit: 8bc60ec34bc1e40685e3976576e04a2623f63a7c
ms.translationtype: MT
ms.contentlocale: id-ID
ms.lasthandoff: 04/15/2021
ms.locfileid: "51816203"
---
# <a name="create-an-email-catch-all"></a><span data-ttu-id="f0e17-102">Buat email berisi semua</span><span class="sxs-lookup"><span data-stu-id="f0e17-102">Create an email catch all</span></span>

<span data-ttu-id="f0e17-103">Penggunaan tangkapan semua tidak disarankan.</span><span class="sxs-lookup"><span data-stu-id="f0e17-103">Use of a catch all is strongly discouraged.</span></span> <span data-ttu-id="f0e17-104">Akan lebih baik jika memberikan informasi terpental kembali kepada pengirim yang memberi tahu pengirim bahwa pesan mereka tidak dapat terkirim sesuai alamat sehingga mereka dapat melakukan tindakan.</span><span class="sxs-lookup"><span data-stu-id="f0e17-104">It is better to provide a bounce back to the sender letting senders know their message could not be delivered as addressed so they can take action.</span></span> <span data-ttu-id="f0e17-105">Anda juga bisa membatasi kotak surat yang dipantau agar hanya menemukan alamat email yang sebelumnya valid.</span><span class="sxs-lookup"><span data-stu-id="f0e17-105">You can also limit the monitored mailbox to only catch formerly valid email addresses.</span></span> 

<span data-ttu-id="f0e17-106">Semua tangkapan semua kotak surat akan menerima banyak spam dan pada akhirnya dapat mengisi jika tidak dipantau dengan jelas.</span><span class="sxs-lookup"><span data-stu-id="f0e17-106">Any catch all mailbox will receive a good deal of spam and may eventually fill if not closely monitored.</span></span> <span data-ttu-id="f0e17-107">(Terdapat batasan penerimaan.)</span><span class="sxs-lookup"><span data-stu-id="f0e17-107">(There are receiving limits.)</span></span> 

<span data-ttu-id="f0e17-108">Jika memutuskan untuk melanjutkan, ikuti langkah-langkah berikut:</span><span class="sxs-lookup"><span data-stu-id="f0e17-108">If you decide to proceed, follow these steps:</span></span>

1. <span data-ttu-id="f0e17-109">Membuat grup distribusi dinamis & menyertakan "Semua Tipe Penerima."</span><span class="sxs-lookup"><span data-stu-id="f0e17-109">Create a Dynamic Distribution Group & include "All Recipient Types."</span></span>

2. <span data-ttu-id="f0e17-110">Buat Kotak Surat khusus untuk menemukan email, misalnya, catchall@domain.com.</span><span class="sxs-lookup"><span data-stu-id="f0e17-110">Create a dedicated Mailbox to catch emails, for example, catchall@domain.com.</span></span>

3. <span data-ttu-id="f0e17-111">Untuk domain tertentu, setel DomainType ke "Internal Fonty".</span><span class="sxs-lookup"><span data-stu-id="f0e17-111">For the specific domain, set the DomainType to “InternalRelay”.</span></span> <span data-ttu-id="f0e17-112">Jika nanti Anda menghapus semua tangkapan, pastikan untuk mengatur kembali domain ke Otoritatif.</span><span class="sxs-lookup"><span data-stu-id="f0e17-112">If you later remove the catch all, be sure to set the domain back to Authoritative.</span></span>

4. <span data-ttu-id="f0e17-113">Membuat Aturan Transpor Alur Email seperti berikut:</span><span class="sxs-lookup"><span data-stu-id="f0e17-113">Create a Mailflow Transport Rule as follows:</span></span>

    - <span data-ttu-id="f0e17-114">Jika Pengirim adalah "Di Luar Organisasi"</span><span class="sxs-lookup"><span data-stu-id="f0e17-114">If the Sender is "Outside the Organization"</span></span>
    - <span data-ttu-id="f0e17-115">Alihkan pesan ke Catchall@domain.com</span><span class="sxs-lookup"><span data-stu-id="f0e17-115">Redirect the message to Catchall@domain.com</span></span>
    - <span data-ttu-id="f0e17-116">Kecuali jika penerima adalah anggota dari grup allusers@domain.com (Grup Distribusi berisi semua anggota)</span><span class="sxs-lookup"><span data-stu-id="f0e17-116">Except if the recipient is a member of allusers@domain.com (Distribution Group contains all members)</span></span>
    - <span data-ttu-id="f0e17-117">Pastikan untuk memvalidasi bahwa kotak surat baru ditambahkan ke dalam Grup Distribusi Dinamis</span><span class="sxs-lookup"><span data-stu-id="f0e17-117">Ensure to validate that new mailboxes are added into the Dynamic Distribution Group</span></span>
