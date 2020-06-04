---
title: Perbarui data DNS untuk menjaga situs web Anda dengan penyedia hosting Anda saat ini
ms.author: pebaum
author: pebaum
manager: mnirkhe
ms.audience: Admin
ms.topic: article
ROBOTS: NOINDEX, NOFOLLOW
localization_priority: Normal
ms.collection: Adm_O365
ms.custom:
- "42"
- "43"
- "100002"
ms.assetid: 48251355-7383-4fdc-a1e1-9dc2c85a8d29
ms.openlocfilehash: 7bd36c3954d12d3ee4ac624a2f827d8e5cd88082
ms.sourcegitcommit: bc7d6f4f3c9f7060d073f5130e1ec856e248d020
ms.translationtype: MT
ms.contentlocale: id-ID
ms.lasthandoff: 06/02/2020
ms.locfileid: "36665763"
---
# <a name="update-dns-records-to-keep-your-website-with-your-current-hosting-provider"></a><span data-ttu-id="501f8-102">Perbarui data DNS untuk menjaga situs web Anda dengan penyedia hosting Anda saat ini</span><span class="sxs-lookup"><span data-stu-id="501f8-102">Update DNS records to keep your website with your current hosting provider</span></span>

1. <span data-ttu-id="501f8-103">Di pusat admin Microsoft 365, pergi ke halaman **setup**  >  [domain](https://portal.office.com/adminportal/home#/Domains) , dan dalam daftar domain, pilih domain yang Anda gunakan untuk situs web Anda.</span><span class="sxs-lookup"><span data-stu-id="501f8-103">In the Microsoft 365 admin center, go to the **Setup** > [Domains](https://portal.office.com/adminportal/home#/Domains) page, and in the list of domains, select the domain you're using for your website.</span></span>

2. <span data-ttu-id="501f8-104">Pilih **+ rekaman kustom baru** dan masukkan yang berikut:</span><span class="sxs-lookup"><span data-stu-id="501f8-104">Select **+ New custom record** and enter the following:</span></span>

  - <span data-ttu-id="501f8-105">Untuk **tipe DNS** , masukkan: **A (alamat)**</span><span class="sxs-lookup"><span data-stu-id="501f8-105">For **DNS type** enter: **A (Address)**</span></span>

  - <span data-ttu-id="501f8-106">Untuk **nama host atau alias**, ketik berikut ini:**@**</span><span class="sxs-lookup"><span data-stu-id="501f8-106">For **Host name or Alias**, type the following: **@**</span></span>

  - <span data-ttu-id="501f8-107">Untuk **Alamat IP**, KETIK alamat IP statis untuk situs web tempat saat ini dihosting (misalnya, 172.16.140.1).</span><span class="sxs-lookup"><span data-stu-id="501f8-107">For **IP Address**, type the static IP address for your website where it's currently hosted (for example, 172.16.140.1).</span></span>

    <span data-ttu-id="501f8-108">Ini harus alamat IP *statis* untuk situs web, bukan alamat IP *dinamis* .</span><span class="sxs-lookup"><span data-stu-id="501f8-108">This must be a  *static*  IP address for the website, not a  *dynamic*  IP address.</span></span> <span data-ttu-id="501f8-109">Periksa dengan situs di mana situs web Anda di-host untuk memastikan Anda bisa mendapatkan alamat IP statis untuk situs web publik Anda.</span><span class="sxs-lookup"><span data-stu-id="501f8-109">Check with site where your website is hosted to make sure you can get a static IP address for your public website.</span></span>

3. <span data-ttu-id="501f8-110">Pilih **Simpan**.</span><span class="sxs-lookup"><span data-stu-id="501f8-110">Select **Save**.</span></span>

<span data-ttu-id="501f8-111">Selain itu, Anda dapat membuat data CNAME untuk membantu pelanggan menemukan situs web Anda.</span><span class="sxs-lookup"><span data-stu-id="501f8-111">In addition, you can create a CNAME record to help customers find your website.</span></span>
  
1. <span data-ttu-id="501f8-112">Pilih **+ rekaman kustom baru** dan masukkan yang berikut:</span><span class="sxs-lookup"><span data-stu-id="501f8-112">Select **+ New custom record** and enter the following:</span></span>

  - <span data-ttu-id="501f8-113">Untuk **tipe DNS** , masukkan: **CNAME (alias)**</span><span class="sxs-lookup"><span data-stu-id="501f8-113">For **DNS type** enter: **CNAME (Alias)**</span></span>

  - <span data-ttu-id="501f8-114">Untuk **nama host atau alias**, ketik berikut ini: **www**</span><span class="sxs-lookup"><span data-stu-id="501f8-114">For **Host name or Alias**, type the following: **www**</span></span>

  - <span data-ttu-id="501f8-115">Untuk **titik alamat**, ketik nama domain yang sepenuhnya memenuhi syarat (FQDN) untuk situs web Anda (misalnya, contoso.com).</span><span class="sxs-lookup"><span data-stu-id="501f8-115">For **Points to address**, type the fully qualified domain name (FQDN) for your website (for example, contoso.com).</span></span>

2. <span data-ttu-id="501f8-116">Pilih **Simpan**.</span><span class="sxs-lookup"><span data-stu-id="501f8-116">Select **Save**.</span></span>
