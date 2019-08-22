---
title: Menambahkan pengguna eksternal ke grup distribusi
ms.author: v-crytho
author: CrystalThomasMS
ms.date: 8/22/2017
ms.audience: ITPro
ms.topic: article
ROBOTS: NOINDEX, NOFOLLOW
localization_priority: Normal
ms.assetid: caa0f310-0bb7-48e3-8ad2-cb358b53bbba
ms.openlocfilehash: ce0c589e1661fb4607452fe2e8f897758b2718e8
ms.sourcegitcommit: 1d98db8acb9959aba3b5e308a567ade6b62da56c
ms.translationtype: MT
ms.contentlocale: id-ID
ms.lasthandoff: 08/22/2019
ms.locfileid: "36494530"
---
# <a name="add-external-users-to-a-distribution-group"></a><span data-ttu-id="71ae2-102">Menambahkan pengguna eksternal ke grup distribusi?</span><span class="sxs-lookup"><span data-stu-id="71ae2-102">Add external users to a Distribution Group?</span></span>

<span data-ttu-id="71ae2-103">Menambahkan kontak eksternal ke grup distribusi (DG) adalah 2-langkah proses:</span><span class="sxs-lookup"><span data-stu-id="71ae2-103">Adding an external contact to a Distribution Group (DG) is a 2-step process:</span></span>
  
1. <span data-ttu-id="71ae2-104">Membuat kontak pesan pengguna eksternal:</span><span class="sxs-lookup"><span data-stu-id="71ae2-104">Create a Mail Contact for the external user:</span></span>
    
    1. <span data-ttu-id="71ae2-105">Di pusat admin, pergi ke **pengguna** > halaman[kontak](https://admin.microsoft.com/adminportal/home#/Contact) .</span><span class="sxs-lookup"><span data-stu-id="71ae2-105">In the admin center, go to the **Users** > [Contacts](https://admin.microsoft.com/adminportal/home#/Contact) page.</span></span> 
    
    2. <span data-ttu-id="71ae2-106">Pilih **Tambah Kontak**.</span><span class="sxs-lookup"><span data-stu-id="71ae2-106">Select **Add a contact**.</span></span>
    
    3. <span data-ttu-id="71ae2-107">Jenis informasi kontak Anda dan pilih **Tambah**.</span><span class="sxs-lookup"><span data-stu-id="71ae2-107">Type the information for your contact and select **Add**.</span></span>
    
2. <span data-ttu-id="71ae2-108">Menambahkan kontak ke DG Anda:</span><span class="sxs-lookup"><span data-stu-id="71ae2-108">Add the Mail Contact to your DG:</span></span>
    
    1. <span data-ttu-id="71ae2-109">Di pusat admin, pergi ke **kelompok** > halaman[Groups](https://admin.microsoft.com/adminportal/home#/groups) .</span><span class="sxs-lookup"><span data-stu-id="71ae2-109">In the admin center, go to the **Groups** > [Groups](https://admin.microsoft.com/adminportal/home#/groups) page.</span></span> 
    
    2. <span data-ttu-id="71ae2-110">Menemukan DG yang Anda ingin menambahkan pengguna eksternal, dan pilih untuk membuka edit dialog.</span><span class="sxs-lookup"><span data-stu-id="71ae2-110">Find the DG you want to add the external user to, and select it to open the edit dialog.</span></span>
    
    3. <span data-ttu-id="71ae2-111">Pada tab **anggota** , pilih **Tampilkan semua dan mengelola anggota**.</span><span class="sxs-lookup"><span data-stu-id="71ae2-111">On the **Members** tab, select **View all and manage members**.</span></span> 
    
    4. <span data-ttu-id="71ae2-112">Pilih **tambah anggota**.</span><span class="sxs-lookup"><span data-stu-id="71ae2-112">Select **Add members**.</span></span>
    
    5. <span data-ttu-id="71ae2-113">Pilih kontak pesan yang Anda buat pada langkah sebelumnya, dan kemudian pilih **Simpan**.</span><span class="sxs-lookup"><span data-stu-id="71ae2-113">Select the Mail Contact you created on the previous step, and then select **Save**.</span></span>
    
<span data-ttu-id="71ae2-114">Jika setelah mengikuti langkah-langkah eksternal pengguna tidak dapat mengirim email ke DG atau tidak menerima email dari itu, bisa jadi bahwa DG ditandai untuk hanya membolehkan email dari pengguna internal.</span><span class="sxs-lookup"><span data-stu-id="71ae2-114">If after following these steps your external users can't send emails to the DG or don't receive emails from it, it could be that the DG is marked to only allow emails from internal users.</span></span> <span data-ttu-id="71ae2-115">Anda dapat memeriksa konfigurasi ini dan memperbaikinya mengikuti petunjuk [di sini](https://support.office.com/article/Fix-email-delivery-issues-for-error-code-5-7-133-in-Office-365-991abc19-7756-438f-abcb-39f69b80f284.aspx).</span><span class="sxs-lookup"><span data-stu-id="71ae2-115">You can check this configuration and fix it following the directions [here](https://support.office.com/article/Fix-email-delivery-issues-for-error-code-5-7-133-in-Office-365-991abc19-7756-438f-abcb-39f69b80f284.aspx).</span></span>
  
 <span data-ttu-id="71ae2-116">**Catatan:** Petunjuk ini tidak berlaku jika grup Anda jenis "Office 365 grup" bukan "Grup distribusi."</span><span class="sxs-lookup"><span data-stu-id="71ae2-116">**Note:** These instructions don't apply if your group's type is "Office 365 group" instead of "Distribution group."</span></span> <span data-ttu-id="71ae2-117">Jika ini terjadi, Anda dapat menambahkan pengguna eksternal langsung ke grup dari Outlook.</span><span class="sxs-lookup"><span data-stu-id="71ae2-117">If that is the case, you can add the external user directly to the group from Outlook.</span></span> <span data-ttu-id="71ae2-118">Informasi rinci pada Office 365 kelompok tamu serta petunjuk untuk menambahkan eksternal tamu dapat ditemukan di [artikel ini](https://support.office.com/article/Guest-access-in-Office-365-Groups-bfc7a840-868f-4fd6-a390-f347bf51aff6.aspx).</span><span class="sxs-lookup"><span data-stu-id="71ae2-118">Detailed information on Office 365 groups guests as well as instructions for adding external guests can be found in [this article](https://support.office.com/article/Guest-access-in-Office-365-Groups-bfc7a840-868f-4fd6-a390-f347bf51aff6.aspx).</span></span>
  