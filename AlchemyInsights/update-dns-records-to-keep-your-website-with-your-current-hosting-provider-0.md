---
title: Pembaruan data DNS untuk menjaga website Anda dengan penyedia hosting Anda saat ini
ms.author: pebaum
author: pebaum
manager: mnirkhe
ms.date: 5/2/2018
ms.audience: Admin
ms.topic: article
ROBOTS: NOINDEX, NOFOLLOW
localization_priority: Normal
ms.collection: Adm_O365
ms.custom: ''
ms.assetid: 48251355-7383-4fdc-a1e1-9dc2c85a8d29
ms.openlocfilehash: f2cdb319e56b82c09b7a9856c81a45e69dee6759
ms.sourcegitcommit: 9d78905c512192ffc4675468abd2efc5f2e4baf4
ms.translationtype: MT
ms.contentlocale: id-ID
ms.lasthandoff: 04/23/2019
ms.locfileid: "32423726"
---
# <a name="update-dns-records-to-keep-your-website-with-your-current-hosting-provider"></a><span data-ttu-id="3c25d-102">Pembaruan data DNS untuk menjaga website Anda dengan penyedia hosting Anda saat ini</span><span class="sxs-lookup"><span data-stu-id="3c25d-102">Update DNS records to keep your website with your current hosting provider</span></span>

1. <span data-ttu-id="3c25d-103">Pada halaman [domain](https://portal.office.com/adminportal/home#/Domains) , dalam daftar domain, pilih domain yang Anda gunakan untuk website Anda, dan kemudian pilih **pengaturan DNS** di panel manajemen.</span><span class="sxs-lookup"><span data-stu-id="3c25d-103">On the [Domains](https://portal.office.com/adminportal/home#/Domains) page, in the list of domains, select the domain you're using for your website, and then select **DNS settings** in the management pane.</span></span> 
    
2. <span data-ttu-id="3c25d-104">Pilih **+ catatan kustom baru** dan masukkan yang berikut:</span><span class="sxs-lookup"><span data-stu-id="3c25d-104">Select **+ New custom record** and enter the following:</span></span> 
    
  - <span data-ttu-id="3c25d-105">Untuk **jenis DNS** masukkan: **(alamat)**</span><span class="sxs-lookup"><span data-stu-id="3c25d-105">For **DNS type** enter: **A (Address)**</span></span>
    
  - <span data-ttu-id="3c25d-106">Untuk **nama Host atau Alias**, ketik berikut ini:**@**</span><span class="sxs-lookup"><span data-stu-id="3c25d-106">For **Host name or Alias**, type the following: **@**</span></span>
    
  - <span data-ttu-id="3c25d-107">Untuk **Alamat IP**, ketik alamat IP statis untuk situs web tempat itu saat ini host (misalnya, 172.16.140.1).</span><span class="sxs-lookup"><span data-stu-id="3c25d-107">For **IP Address**, type the static IP address for your website where it's currently hosted (for example, 172.16.140.1).</span></span> 
    
    <span data-ttu-id="3c25d-108">Ini harus menjadi alamat IP *statis* untuk website, bukan alamat IP *dinamis* .</span><span class="sxs-lookup"><span data-stu-id="3c25d-108">This must be a  *static*  IP address for the website, not a  *dynamic*  IP address.</span></span> <span data-ttu-id="3c25d-109">Periksa dengan situs mana situs web adalah host untuk memastikan Anda bisa mendapatkan alamat IP statis untuk situs umum.</span><span class="sxs-lookup"><span data-stu-id="3c25d-109">Check with site where your website is hosted to make sure you can get a static IP address for your public website.</span></span> 
    
3. <span data-ttu-id="3c25d-110">Pilih **Simpan**.</span><span class="sxs-lookup"><span data-stu-id="3c25d-110">Select **Save**.</span></span> 
    
<span data-ttu-id="3c25d-111">Selain itu, Anda dapat membuat CNAME untuk membantu pelanggan menemukan situs web Anda.</span><span class="sxs-lookup"><span data-stu-id="3c25d-111">In addition, you can create a CNAME record to help customers find your website.</span></span>
  
1. <span data-ttu-id="3c25d-112">Pilih **+ catatan kustom baru** dan masukkan yang berikut:</span><span class="sxs-lookup"><span data-stu-id="3c25d-112">Select **+ New custom record** and enter the following:</span></span> 
    
  - <span data-ttu-id="3c25d-113">Untuk **jenis DNS** masukkan: **CNAME (Alias)**</span><span class="sxs-lookup"><span data-stu-id="3c25d-113">For **DNS type** enter: **CNAME (Alias)**</span></span>
    
  - <span data-ttu-id="3c25d-114">Untuk **nama Host atau Alias**, ketik berikut: **www**</span><span class="sxs-lookup"><span data-stu-id="3c25d-114">For **Host name or Alias**, type the following: **www**</span></span>
    
  - <span data-ttu-id="3c25d-115">Untuk **poin ke alamat**, ketik nama domain sepenuhnya memenuhi syarat (FQDN) untuk situs web Anda (misalnya, contoso.com).</span><span class="sxs-lookup"><span data-stu-id="3c25d-115">For **Points to address**, type the fully qualified domain name (FQDN) for your website (for example, contoso.com).</span></span> 
    
2. <span data-ttu-id="3c25d-116">Pilih **Simpan**.</span><span class="sxs-lookup"><span data-stu-id="3c25d-116">Select **Save**.</span></span> 
    

