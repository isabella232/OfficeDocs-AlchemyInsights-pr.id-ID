---
title: Memperbarui catatan DNS untuk mempertahankan situs web Anda dengan penyedia hosting Anda saat ini
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
- "42"
- "43"
- "100002"
ms.assetid: 48251355-7383-4fdc-a1e1-9dc2c85a8d29
ms.openlocfilehash: 89bce2aa5931c0c20706efabd42d2351be43938b
ms.sourcegitcommit: 8bc60ec34bc1e40685e3976576e04a2623f63a7c
ms.translationtype: MT
ms.contentlocale: id-ID
ms.lasthandoff: 04/15/2021
ms.locfileid: "51827524"
---
# <a name="update-dns-records-to-keep-your-website-with-your-current-hosting-provider"></a><span data-ttu-id="98a4e-102">Memperbarui catatan DNS untuk mempertahankan situs web Anda dengan penyedia hosting Anda saat ini</span><span class="sxs-lookup"><span data-stu-id="98a4e-102">Update DNS records to keep your website with your current hosting provider</span></span>

1. <span data-ttu-id="98a4e-103">Di pusat admin Microsoft 365, masuk ke halaman **Penyiapan** Domain, lalu dalam daftar domain, pilih domain yang digunakan untuk  >  [](https://admin.microsoft.com/Adminportal#/Domains) situs web Anda.</span><span class="sxs-lookup"><span data-stu-id="98a4e-103">In the Microsoft 365 admin center, go to the **Setup** > [Domains](https://admin.microsoft.com/Adminportal#/Domains) page, and in the list of domains, select the domain you're using for your website.</span></span>

2. <span data-ttu-id="98a4e-104">Pilih **+ Catatan kustom baru,** lalu masukkan hal berikut:</span><span class="sxs-lookup"><span data-stu-id="98a4e-104">Select **+ New custom record** and enter the following:</span></span>

  - <span data-ttu-id="98a4e-105">Untuk **tipe DNS,** masukkan: **A (Alamat)**</span><span class="sxs-lookup"><span data-stu-id="98a4e-105">For **DNS type** enter: **A (Address)**</span></span>

  - <span data-ttu-id="98a4e-106">Untuk **Nama host atau Alias,** ketikkan: **@**</span><span class="sxs-lookup"><span data-stu-id="98a4e-106">For **Host name or Alias**, type the following: **@**</span></span>

  - <span data-ttu-id="98a4e-107">Untuk **Alamat IP,** ketikkan alamat IP statis tempat situs web dihosting saat ini (misalnya, 172.16.140.1).</span><span class="sxs-lookup"><span data-stu-id="98a4e-107">For **IP Address**, type the static IP address for your website where it's currently hosted (for example, 172.16.140.1).</span></span>

    <span data-ttu-id="98a4e-108">Ini harus merupakan  *alamat*  IP statis untuk situs web, bukan  *alamat*  IP dinamis.</span><span class="sxs-lookup"><span data-stu-id="98a4e-108">This must be a  *static*  IP address for the website, not a  *dynamic*  IP address.</span></span> <span data-ttu-id="98a4e-109">Periksa situs tempat situs web Anda dihosting untuk memastikan Anda bisa mendapatkan alamat IP statis untuk situs web publik.</span><span class="sxs-lookup"><span data-stu-id="98a4e-109">Check with site where your website is hosted to make sure you can get a static IP address for your public website.</span></span>

3. <span data-ttu-id="98a4e-110">Pilih **Simpan.**</span><span class="sxs-lookup"><span data-stu-id="98a4e-110">Select **Save**.</span></span>

<span data-ttu-id="98a4e-111">Selain itu, Anda bisa membuat catatan CNAME untuk membantu pelanggan menemukan situs web Anda.</span><span class="sxs-lookup"><span data-stu-id="98a4e-111">In addition, you can create a CNAME record to help customers find your website.</span></span>
  
1. <span data-ttu-id="98a4e-112">Pilih **+ Catatan kustom baru,** lalu masukkan hal berikut:</span><span class="sxs-lookup"><span data-stu-id="98a4e-112">Select **+ New custom record** and enter the following:</span></span>

  - <span data-ttu-id="98a4e-113">Untuk **Tipe DNS,** masukkan: **CNAME (Alias)**</span><span class="sxs-lookup"><span data-stu-id="98a4e-113">For **DNS type** enter: **CNAME (Alias)**</span></span>

  - <span data-ttu-id="98a4e-114">Untuk **Nama host atau Alias,** ketikkan: **www**</span><span class="sxs-lookup"><span data-stu-id="98a4e-114">For **Host name or Alias**, type the following: **www**</span></span>

  - <span data-ttu-id="98a4e-115">Untuk **Alamat tujuan,** ketikkan FQDN (nama domain yang sepenuhnya memenuhi syarat) untuk situs web Anda (misalnya, contoso.com).</span><span class="sxs-lookup"><span data-stu-id="98a4e-115">For **Points to address**, type the fully qualified domain name (FQDN) for your website (for example, contoso.com).</span></span>

2. <span data-ttu-id="98a4e-116">Pilih **Simpan.**</span><span class="sxs-lookup"><span data-stu-id="98a4e-116">Select **Save**.</span></span>
