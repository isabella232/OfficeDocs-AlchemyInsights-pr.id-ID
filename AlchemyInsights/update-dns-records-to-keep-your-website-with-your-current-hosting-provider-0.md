---
title: Memperbarui catatan DNS untuk mempertahankan situs web Anda dengan penyedia hosting Anda saat ini
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
- "42"
- "43"
- "100002"
ms.assetid: 48251355-7383-4fdc-a1e1-9dc2c85a8d29
ms.openlocfilehash: 2f2d4f7c093d62267bb859e96493ec6d09452c7e
ms.sourcegitcommit: c6692ce0fa1358ec3529e59ca0ecdfdea4cdc759
ms.translationtype: MT
ms.contentlocale: id-ID
ms.lasthandoff: 09/14/2020
ms.locfileid: "47699522"
---
# <a name="update-dns-records-to-keep-your-website-with-your-current-hosting-provider"></a><span data-ttu-id="362e1-102">Memperbarui catatan DNS untuk mempertahankan situs web Anda dengan penyedia hosting Anda saat ini</span><span class="sxs-lookup"><span data-stu-id="362e1-102">Update DNS records to keep your website with your current hosting provider</span></span>

1. <span data-ttu-id="362e1-103">Di pusat admin Microsoft 365, masuk ke halaman domain **penyetelan**  >  [Domains](https://portal.office.com/adminportal/home#/Domains) , dan di daftar domain, pilih domain yang Anda gunakan untuk situs web Anda.</span><span class="sxs-lookup"><span data-stu-id="362e1-103">In the Microsoft 365 admin center, go to the **Setup** > [Domains](https://portal.office.com/adminportal/home#/Domains) page, and in the list of domains, select the domain you're using for your website.</span></span>

2. <span data-ttu-id="362e1-104">Pilih **+ catatan kustom baru** , lalu masukkan yang berikut ini:</span><span class="sxs-lookup"><span data-stu-id="362e1-104">Select **+ New custom record** and enter the following:</span></span>

  - <span data-ttu-id="362e1-105">Untuk **tipe DNS** , masukkan: **A (address)**</span><span class="sxs-lookup"><span data-stu-id="362e1-105">For **DNS type** enter: **A (Address)**</span></span>

  - <span data-ttu-id="362e1-106">Untuk **nama host atau alias**, ketikkan yang berikut ini: **@**</span><span class="sxs-lookup"><span data-stu-id="362e1-106">For **Host name or Alias**, type the following: **@**</span></span>

  - <span data-ttu-id="362e1-107">Untuk **Alamat IP**, KETIKKAN alamat IP statis untuk situs web Anda saat ini dihosting (misalnya, 172.16.140.1).</span><span class="sxs-lookup"><span data-stu-id="362e1-107">For **IP Address**, type the static IP address for your website where it's currently hosted (for example, 172.16.140.1).</span></span>

    <span data-ttu-id="362e1-108">Ini harus berupa alamat IP  *statis*  untuk situs web, bukan alamat IP  *dinamis*  .</span><span class="sxs-lookup"><span data-stu-id="362e1-108">This must be a  *static*  IP address for the website, not a  *dynamic*  IP address.</span></span> <span data-ttu-id="362e1-109">Periksa situs tempat situs web Anda dihosting untuk memastikan Anda bisa mendapatkan alamat IP statis untuk situs web publik Anda.</span><span class="sxs-lookup"><span data-stu-id="362e1-109">Check with site where your website is hosted to make sure you can get a static IP address for your public website.</span></span>

3. <span data-ttu-id="362e1-110">Pilih **Simpan**.</span><span class="sxs-lookup"><span data-stu-id="362e1-110">Select **Save**.</span></span>

<span data-ttu-id="362e1-111">Selain itu, Anda bisa membuat catatan CNAME untuk membantu pelanggan menemukan situs web Anda.</span><span class="sxs-lookup"><span data-stu-id="362e1-111">In addition, you can create a CNAME record to help customers find your website.</span></span>
  
1. <span data-ttu-id="362e1-112">Pilih **+ catatan kustom baru** , lalu masukkan yang berikut ini:</span><span class="sxs-lookup"><span data-stu-id="362e1-112">Select **+ New custom record** and enter the following:</span></span>

  - <span data-ttu-id="362e1-113">Untuk **tipe DNS** masukkan: **CNAME (alias)**</span><span class="sxs-lookup"><span data-stu-id="362e1-113">For **DNS type** enter: **CNAME (Alias)**</span></span>

  - <span data-ttu-id="362e1-114">Untuk **nama host atau alias**, ketikkan yang berikut: **www**</span><span class="sxs-lookup"><span data-stu-id="362e1-114">For **Host name or Alias**, type the following: **www**</span></span>

  - <span data-ttu-id="362e1-115">Untuk **Alamat**target, ketikkan nama domain yang sepenuhnya memenuhi syarat (FQDN) untuk situs web Anda (misalnya, contoso.com).</span><span class="sxs-lookup"><span data-stu-id="362e1-115">For **Points to address**, type the fully qualified domain name (FQDN) for your website (for example, contoso.com).</span></span>

2. <span data-ttu-id="362e1-116">Pilih **Simpan**.</span><span class="sxs-lookup"><span data-stu-id="362e1-116">Select **Save**.</span></span>
