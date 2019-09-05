---
title: Menambahkan pengguna eksternal ke grup distribusi
ms.author: chrisda
author: chrisda
ms.audience: ITPro
ms.topic: article
ROBOTS: NOINDEX, NOFOLLOW
localization_priority: Normal
ms.assetid: caa0f310-0bb7-48e3-8ad2-cb358b53bbba
ms.openlocfilehash: e84a5b04d6fc805deaa47cb10c91081f37411e5b
ms.sourcegitcommit: a256e8680379c006287ae30996763051c4d9ff85
ms.translationtype: MT
ms.contentlocale: id-ID
ms.lasthandoff: 09/04/2019
ms.locfileid: "36737876"
---
# <a name="add-external-users-to-a-distribution-group"></a><span data-ttu-id="0b5ec-102">Menambahkan pengguna eksternal ke grup distribusi</span><span class="sxs-lookup"><span data-stu-id="0b5ec-102">Add external users to a Distribution Group</span></span>

<span data-ttu-id="0b5ec-103">Menambahkan kontak eksternal ke grup distribusi (DG) adalah proses dua langkah:</span><span class="sxs-lookup"><span data-stu-id="0b5ec-103">Adding an external contact to a Distribution Group (DG) is a two-step process:</span></span>
  
1. <span data-ttu-id="0b5ec-104">Membuat kontak E-mail untuk pengguna eksternal:</span><span class="sxs-lookup"><span data-stu-id="0b5ec-104">Create a Mail Contact for the external user:</span></span>
    
    1. <span data-ttu-id="0b5ec-105">Di pusat admin, buka halaman[kontak](https://admin.microsoft.com/adminportal/home#/Contact) **pengguna** > .</span><span class="sxs-lookup"><span data-stu-id="0b5ec-105">In the admin center, go to the **Users** > [Contacts](https://admin.microsoft.com/adminportal/home#/Contact) page.</span></span> 
    
    2. <span data-ttu-id="0b5ec-106">Pilih **Tambah Kontak**.</span><span class="sxs-lookup"><span data-stu-id="0b5ec-106">Select **Add a contact**.</span></span>
    
    3. <span data-ttu-id="0b5ec-107">Ketik informasi kontak Anda dan pilih **Tambah**.</span><span class="sxs-lookup"><span data-stu-id="0b5ec-107">Type the information for your contact and select **Add**.</span></span>
    
2. <span data-ttu-id="0b5ec-108">Tambahkan kontak E-mail ke DG Anda:</span><span class="sxs-lookup"><span data-stu-id="0b5ec-108">Add the Mail Contact to your DG:</span></span>
    
    1. <span data-ttu-id="0b5ec-109">Di pusat admin, buka[](https://admin.microsoft.com/adminportal/home#/groups)  >  **halaman grup grup**.</span><span class="sxs-lookup"><span data-stu-id="0b5ec-109">In the admin center, go to the **Groups** > [Groups](https://admin.microsoft.com/adminportal/home#/groups) page.</span></span> 
    
    2. <span data-ttu-id="0b5ec-110">Temukan DG yang ingin Anda tambahkan pengguna eksternal, dan pilih untuk membuka dialog Edit.</span><span class="sxs-lookup"><span data-stu-id="0b5ec-110">Find the DG you want to add the external user to, and select it to open the edit dialog.</span></span>
    
    3. <span data-ttu-id="0b5ec-111">Pada tab **anggota** , pilih **Lihat semua dan Kelola anggota**.</span><span class="sxs-lookup"><span data-stu-id="0b5ec-111">On the **Members** tab, select **View all and manage members**.</span></span> 
    
    4. <span data-ttu-id="0b5ec-112">Pilih **Tambahkan anggota**.</span><span class="sxs-lookup"><span data-stu-id="0b5ec-112">Select **Add members**.</span></span>
    
    5. <span data-ttu-id="0b5ec-113">Pilih kontak E-mail yang Anda buat di langkah sebelumnya, lalu pilih **Simpan**.</span><span class="sxs-lookup"><span data-stu-id="0b5ec-113">Select the Mail Contact you created on the previous step, and then select **Save**.</span></span>
    
<span data-ttu-id="0b5ec-114">Jika setelah mengikuti langkah ini, pengguna eksternal tidak dapat mengirim email ke DG atau tidak menerima email darinya, bisa jadi DG ditandai hanya untuk mengizinkan email dari pengguna internal.</span><span class="sxs-lookup"><span data-stu-id="0b5ec-114">If after following these steps your external users can't send emails to the DG or don't receive emails from it, it could be that the DG is marked to only allow emails from internal users.</span></span> <span data-ttu-id="0b5ec-115">Anda dapat memeriksa konfigurasi ini dan memperbaikinya mengikuti petunjuk [di sini](https://docs.microsoft.com/exchange/mail-flow-best-practices/non-delivery-reports-in-exchange-online/fix-error-code-5-7-133-in-exchange-online).</span><span class="sxs-lookup"><span data-stu-id="0b5ec-115">You can check this configuration and fix it following the directions [here](https://docs.microsoft.com/exchange/mail-flow-best-practices/non-delivery-reports-in-exchange-online/fix-error-code-5-7-133-in-exchange-online).</span></span>
  
 <span data-ttu-id="0b5ec-116">**Catatan:** Petunjuk ini tidak berlaku jika jenis grup Anda adalah "Office 365 grup" bukannya "grup distribusi."</span><span class="sxs-lookup"><span data-stu-id="0b5ec-116">**Note:** These instructions don't apply if your group's type is "Office 365 group" instead of "Distribution group."</span></span> <span data-ttu-id="0b5ec-117">Jika demikian, Anda dapat menambahkan pengguna eksternal langsung ke grup dari Outlook.</span><span class="sxs-lookup"><span data-stu-id="0b5ec-117">If that is the case, you can add the external user directly to the group from Outlook.</span></span> <span data-ttu-id="0b5ec-118">Informasi rinci tentang kantor 365 kelompok tamu serta petunjuk untuk menambahkan tamu eksternal dapat ditemukan di [artikel ini](https://support.office.com/article/Guest-access-in-Office-365-Groups-bfc7a840-868f-4fd6-a390-f347bf51aff6.aspx).</span><span class="sxs-lookup"><span data-stu-id="0b5ec-118">Detailed information on Office 365 groups guests as well as instructions for adding external guests can be found in [this article](https://support.office.com/article/Guest-access-in-Office-365-Groups-bfc7a840-868f-4fd6-a390-f347bf51aff6.aspx).</span></span>
  