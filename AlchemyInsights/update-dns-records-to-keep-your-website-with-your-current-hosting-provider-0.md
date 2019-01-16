---
title: Pembaruan data DNS untuk menjaga website Anda dengan penyedia hosting Anda saat ini
ms.author: pebaum
author: pebaum
manager: mnirkhe
ms.date: 5/2/2018
ms.audience: Admin
ms.topic: article
ROBOTS: NOINDEX, NOFOLLOW
localization_priority: Priority
ms.collection: Adm_O365
ms.custom: Adm_O365
ms.assetid: 48251355-7383-4fdc-a1e1-9dc2c85a8d29
ms.openlocfilehash: a79302259e294ea5bf3b1d29393a412edb27a388
ms.sourcegitcommit: d6ea5e9458a2b8ceaab3ac4bd483e1130b9a398a
ms.translationtype: MT
ms.contentlocale: id-ID
ms.lasthandoff: 01/15/2019
ms.locfileid: "28294871"
---
# <a name="update-dns-records-to-keep-your-website-with-your-current-hosting-provider"></a><span data-ttu-id="b3d4c-102">Pembaruan data DNS untuk menjaga website Anda dengan penyedia hosting Anda saat ini</span><span class="sxs-lookup"><span data-stu-id="b3d4c-102">Update DNS records to keep your website with your current hosting provider</span></span>

1. <span data-ttu-id="b3d4c-103">Pada halaman [domain](https://portal.office.com/adminportal/home#/Domains) , dalam daftar domain, pilih domain yang Anda gunakan untuk website Anda, dan kemudian pilih **pengaturan DNS** di panel manajemen.</span><span class="sxs-lookup"><span data-stu-id="b3d4c-103">On the [Domains](https://portal.office.com/adminportal/home#/Domains) page, in the list of domains, select the domain you're using for your website, and then select **DNS settings** in the management pane.</span></span> 
    
2. <span data-ttu-id="b3d4c-104">Pilih **+ catatan kustom baru** dan masukkan yang berikut:</span><span class="sxs-lookup"><span data-stu-id="b3d4c-104">Select **+ New custom record** and enter the following:</span></span> 
    
  - <span data-ttu-id="b3d4c-105">Untuk **jenis DNS** masukkan: **(alamat)**</span><span class="sxs-lookup"><span data-stu-id="b3d4c-105">For **DNS type** enter: **A (Address)**</span></span>
    
  - <span data-ttu-id="b3d4c-106">Untuk **nama Host atau Alias**, ketik berikut ini:**@**</span><span class="sxs-lookup"><span data-stu-id="b3d4c-106">For **Host name or Alias**, type the following: **@**</span></span>
    
  - <span data-ttu-id="b3d4c-107">Untuk **Alamat IP**, ketik alamat IP statis untuk situs web tempat itu saat ini host (misalnya, 172.16.140.1).</span><span class="sxs-lookup"><span data-stu-id="b3d4c-107">For **IP Address**, type the static IP address for your website where it's currently hosted (for example, 172.16.140.1).</span></span> 
    
    <span data-ttu-id="b3d4c-p101">Ini harus menjadi alamat IP *statis* untuk website, bukan alamat IP *dinamis* . Periksa dengan situs mana situs web adalah host untuk memastikan Anda bisa mendapatkan alamat IP statis untuk situs umum.</span><span class="sxs-lookup"><span data-stu-id="b3d4c-p101">This must be a  *static*  IP address for the website, not a  *dynamic*  IP address. Check with site where your website is hosted to make sure you can get a static IP address for your public website.</span></span> 
    
3. <span data-ttu-id="b3d4c-110">Pilih **Simpan**.</span><span class="sxs-lookup"><span data-stu-id="b3d4c-110">Select **Save**.</span></span> 
    
<span data-ttu-id="b3d4c-111">Selain itu, Anda dapat membuat CNAME untuk membantu pelanggan menemukan situs web Anda.</span><span class="sxs-lookup"><span data-stu-id="b3d4c-111">In addition, you can create a CNAME record to help customers find your website.</span></span>
  
1. <span data-ttu-id="b3d4c-112">Pilih **+ catatan kustom baru** dan masukkan yang berikut:</span><span class="sxs-lookup"><span data-stu-id="b3d4c-112">Select **+ New custom record** and enter the following:</span></span> 
    
  - <span data-ttu-id="b3d4c-113">Untuk **jenis DNS** masukkan: **CNAME (Alias)**</span><span class="sxs-lookup"><span data-stu-id="b3d4c-113">For **DNS type** enter: **CNAME (Alias)**</span></span>
    
  - <span data-ttu-id="b3d4c-114">Untuk **nama Host atau Alias**, ketik berikut: **www**</span><span class="sxs-lookup"><span data-stu-id="b3d4c-114">For **Host name or Alias**, type the following: **www**</span></span>
    
  - <span data-ttu-id="b3d4c-115">Untuk **poin ke alamat**, ketik nama domain sepenuhnya memenuhi syarat (FQDN) untuk situs web Anda (misalnya, contoso.com).</span><span class="sxs-lookup"><span data-stu-id="b3d4c-115">For **Points to address**, type the fully qualified domain name (FQDN) for your website (for example, contoso.com).</span></span> 
    
2. <span data-ttu-id="b3d4c-116">Pilih **Simpan**.</span><span class="sxs-lookup"><span data-stu-id="b3d4c-116">Select **Save**.</span></span> 
    

