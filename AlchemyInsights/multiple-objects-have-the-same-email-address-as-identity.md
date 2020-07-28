---
title: Beberapa objek memiliki alamat email yang sama sebagai identitas
ms.author: pebaum
author: pebaum
manager: scotv
ms.date: 07/27/2020
ms.audience: Admin
ms.topic: article
ROBOTS: NOINDEX, NOFOLLOW
localization_priority: Priority
ms.collection: Adm_O365
ms.custom:
- "1834"
- "9000247"
ms.openlocfilehash: cc932aa7ecbd1e338c409a7a6525e2c4e673b232
ms.sourcegitcommit: b10cea11b4975354b91193327b58aa4740d34833
ms.translationtype: MT
ms.contentlocale: id-ID
ms.lasthandoff: 07/28/2020
ms.locfileid: "45439192"
---
# <a name="multiple-objects-have-the-same-email-address-as-identity"></a><span data-ttu-id="6c1fa-102">Beberapa objek memiliki alamat email yang sama sebagai identitas</span><span class="sxs-lookup"><span data-stu-id="6c1fa-102">Multiple objects have the same email address as identity</span></span>

<span data-ttu-id="6c1fa-103">**Beberapa objek**</span><span class="sxs-lookup"><span data-stu-id="6c1fa-103">**Multiple objects**</span></span>

<span data-ttu-id="6c1fa-104">Salah satu dari alasan umum galat ini tidak dapat mengarahkan permintaan Outlook Web Access dengan benar di kehadiran beberapa objek yang memiliki alamat email yang sama sebagai identitas.</span><span class="sxs-lookup"><span data-stu-id="6c1fa-104">One of the common reasons of this error is not being able to route an Outlook Web Access request properly in a presence of multiple objects having the same email address as identity.</span></span> <span data-ttu-id="6c1fa-105">Untuk menemukan objek ini, jalankan perintah berikut:</span><span class="sxs-lookup"><span data-stu-id="6c1fa-105">To find these objects, run the following commands:</span></span>

<span data-ttu-id="6c1fa-106">· Penerima Get<email address></span><span class="sxs-lookup"><span data-stu-id="6c1fa-106">· Get-Recipient <email address></span></span>

<span data-ttu-id="6c1fa-107">· Dapatkan-pengguna<email address></span><span class="sxs-lookup"><span data-stu-id="6c1fa-107">· Get-User <email address></span></span>

<span data-ttu-id="6c1fa-108">· Get-pengguna <email address> -softdeleteduser</span><span class="sxs-lookup"><span data-stu-id="6c1fa-108">· Get-User <email address> -SoftDeletedUser</span></span>

<span data-ttu-id="6c1fa-109">· Get-kontak<email address></span><span class="sxs-lookup"><span data-stu-id="6c1fa-109">· Get-Contact <email address></span></span>

<span data-ttu-id="6c1fa-110">· Get-kotak surat <email address> -publicfolder</span><span class="sxs-lookup"><span data-stu-id="6c1fa-110">· Get-Mailbox <email address> -PublicFolder</span></span>

<span data-ttu-id="6c1fa-111">· Get-kotak surat <email address> -includesoftdeletedmailbox</span><span class="sxs-lookup"><span data-stu-id="6c1fa-111">· Get-Mailbox <email address> -IncludeSoftDeletedMailbox</span></span>

<span data-ttu-id="6c1fa-112">· Get-kotak surat <email address> -inactivemailboxonly</span><span class="sxs-lookup"><span data-stu-id="6c1fa-112">· Get-Mailbox <email address> -InactiveMailboxOnly</span></span>

<span data-ttu-id="6c1fa-113">Untuk mengatasi masalah ini, Hapus beberapa objek dengan identitas email yang sama dan pastikan bahwa ada satu objek dengan identitas email tertentu dan jenis Penerimanya adalah UserMailbox.</span><span class="sxs-lookup"><span data-stu-id="6c1fa-113">To resolve the issue, remove multiple objects with the same email identity and make sure that there is a single object with the specific email identity and that its recipient type is UserMailbox.</span></span>

<span data-ttu-id="6c1fa-114">**Alamat yang sama digunakan untuk kotak surat bisnis dan konsumen**</span><span class="sxs-lookup"><span data-stu-id="6c1fa-114">**Same address is used for business and consumer mailboxes**</span></span>

<span data-ttu-id="6c1fa-115">Penyebab lain adalah ketika alamat yang sama digunakan untuk bisnis dan kotak surat konsumen.</span><span class="sxs-lookup"><span data-stu-id="6c1fa-115">Another cause is when the same address is used for business and consumer mailboxes.</span></span> <span data-ttu-id="6c1fa-116">Dalam hal ini, pengguna harus mengubah alias konsumen utama mereka sampai Cafe mendukung skenario ini.</span><span class="sxs-lookup"><span data-stu-id="6c1fa-116">In this case, the user must change their primary consumer alias until Cafe supports this scenario.</span></span> <span data-ttu-id="6c1fa-117">Ini adalah kesalahan permanen yang tidak hilang tanpa intervensi.</span><span class="sxs-lookup"><span data-stu-id="6c1fa-117">This is a permanent error that does not go away without intervention.</span></span>

<span data-ttu-id="6c1fa-118">Untuk detailnya, lihat [mengubah alamat email atau nomor telepon untuk akun Microsoft Anda](https://support.microsoft.com/help/11545/microsoft-account-rename-your-personal-account).</span><span class="sxs-lookup"><span data-stu-id="6c1fa-118">For details, see [Change the email address or phone number for your Microsoft account](https://support.microsoft.com/help/11545/microsoft-account-rename-your-personal-account).</span></span>