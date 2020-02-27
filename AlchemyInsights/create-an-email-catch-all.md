---
title: Buat email menangkap semua
ms.author: pebaum
author: pebaum
manager: mnirkhe
ms.audience: Admin
ms.topic: article
ROBOTS: NOINDEX, NOFOLLOW
localization_priority: Normal
ms.collection: Adm_O365
ms.custom:
- "9001524"
- "3732"
ms.openlocfilehash: 35f31c1662547d57c2fc9978ffb495ac29abcc01
ms.sourcegitcommit: 67015549afcbe05f3b77ea314e2ef7e0e439f9f2
ms.translationtype: MT
ms.contentlocale: id-ID
ms.lasthandoff: 02/26/2020
ms.locfileid: "42286196"
---
# <a name="create-an-email-catch-all"></a><span data-ttu-id="9124b-102">Buat email menangkap semua</span><span class="sxs-lookup"><span data-stu-id="9124b-102">Create an email catch all</span></span>

<span data-ttu-id="9124b-103">Penggunaan menangkap semua sangat dianjurkan.</span><span class="sxs-lookup"><span data-stu-id="9124b-103">Use of a catch all is strongly discouraged.</span></span> <span data-ttu-id="9124b-104">Lebih baik untuk memberikan bouncing kembali ke pengirim membiarkan pengirim tahu pesan mereka tidak dapat dikirim seperti yang dibahas sehingga mereka dapat mengambil tindakan.</span><span class="sxs-lookup"><span data-stu-id="9124b-104">It is better to provide a bounce back to the sender letting senders know their message could not be delivered as addressed so they can take action.</span></span> <span data-ttu-id="9124b-105">Anda juga dapat membatasi kotak pesan yang dipantau untuk hanya menangkap alamat email yang sebelumnya valid.</span><span class="sxs-lookup"><span data-stu-id="9124b-105">You can also limit the monitored mailbox to only catch formerly valid email addresses.</span></span> 

<span data-ttu-id="9124b-106">Setiap menangkap semua kotak surat akan menerima banyak spam dan akhirnya dapat mengisi jika tidak diawasi dengan cermat.</span><span class="sxs-lookup"><span data-stu-id="9124b-106">Any catch all mailbox will receive a good deal of spam and may eventually fill if not closely monitored.</span></span> <span data-ttu-id="9124b-107">(Ada batas penerimaan.)</span><span class="sxs-lookup"><span data-stu-id="9124b-107">(There are receiving limits.)</span></span> 

<span data-ttu-id="9124b-108">Jika Anda memutuskan untuk melanjutkan, ikuti langkah berikut:</span><span class="sxs-lookup"><span data-stu-id="9124b-108">If you decide to proceed, follow these steps:</span></span>

1. <span data-ttu-id="9124b-109">Membuat grup distribusi dinamis & mencakup "semua jenis penerima."</span><span class="sxs-lookup"><span data-stu-id="9124b-109">Create a Dynamic Distribution Group & include "All Recipient Types."</span></span>

2. <span data-ttu-id="9124b-110">Buat kotak surat khusus untuk menangkap email, misalnya, catchall@domain.com.</span><span class="sxs-lookup"><span data-stu-id="9124b-110">Create a dedicated Mailbox to catch emails, for example, catchall@domain.com.</span></span>

3. <span data-ttu-id="9124b-111">Untuk domain tertentu, tetapkan DomainType ke "InternalRelay".</span><span class="sxs-lookup"><span data-stu-id="9124b-111">For the specific domain, set the DomainType to “InternalRelay”.</span></span> <span data-ttu-id="9124b-112">Jika Anda kemudian menghapus menangkap semua, pastikan untuk mengatur domain kembali ke otoritatif.</span><span class="sxs-lookup"><span data-stu-id="9124b-112">If you later remove the catch all, be sure to set the domain back to Authoritative.</span></span>

4. <span data-ttu-id="9124b-113">Buat aturan transpor Mailflow sebagai berikut:</span><span class="sxs-lookup"><span data-stu-id="9124b-113">Create a Mailflow Transport Rule as follows:</span></span>

    - <span data-ttu-id="9124b-114">Jika pengirim adalah "di luar organisasi"</span><span class="sxs-lookup"><span data-stu-id="9124b-114">If the Sender is "Outside the Organization"</span></span>
    - <span data-ttu-id="9124b-115">Mengalihkan pesan ke Catchall@domain.com</span><span class="sxs-lookup"><span data-stu-id="9124b-115">Redirect the message to Catchall@domain.com</span></span>
    - <span data-ttu-id="9124b-116">Kecuali jika Penerima adalah anggota allusers@domain.com (grup distribusi berisi semua anggota)</span><span class="sxs-lookup"><span data-stu-id="9124b-116">Except if the recipient is a member of allusers@domain.com (Distribution Group contains all members)</span></span>
    - <span data-ttu-id="9124b-117">Pastikan untuk memvalidasi bahwa kotak pesan baru ditambahkan ke grup distribusi dinamis</span><span class="sxs-lookup"><span data-stu-id="9124b-117">Ensure to validate that new mailboxes are added into the Dynamic Distribution Group</span></span>
