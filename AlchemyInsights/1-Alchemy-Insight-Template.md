---
title: 'sama seperti nama file terbaik [aturan #-Deskripsi]'
ms.author: pebaum
author: pebaum
manager: jackiesm
ms.date: 4/27/2018
ms.audience: Admin
ms.topic: article
ROBOTS: NOINDEX, NOFOLLOW
localization_priority: Normal
ms.collection: Adm_O365
ms.custom: Adm_O365
ms.assetid: (guid of old soc version if any)
ms.openlocfilehash: e248c2ee3cbb9a86f21c1f36be10c893df76ff52
ms.sourcegitcommit: 3070905131e6d8449981231a3551c0bb4ca38ae6
ms.translationtype: MT
ms.contentlocale: id-ID
ms.lasthandoff: 03/14/2019
ms.locfileid: "30634507"
---
# <a name="required-alchemy-header-h1-h2s-dont-work"></a><span data-ttu-id="98453-102">Diperlukan Alkimia Header H1, H2's tidak bekerja.</span><span class="sxs-lookup"><span data-stu-id="98453-102">Required Alchemy Header H1, H2's dont work.</span></span>
<span data-ttu-id="98453-103">Best Practices dan pedoman untuk authoring Alkimia:</span><span class="sxs-lookup"><span data-stu-id="98453-103">Best Practices and guidelines for Alchemy authoring:</span></span>

1. <span data-ttu-id="98453-104">**Tidak sarang Alkimia wawasan dalam folder**- ini akan merusak struktur url.</span><span class="sxs-lookup"><span data-stu-id="98453-104">**Do not nest Alchemy Insights in folders**- this will break the url structure.</span></span> <span data-ttu-id="98453-105">Kami melihat ke memperbaiki ini.</span><span class="sxs-lookup"><span data-stu-id="98453-105">We're looking into fixing this.</span></span>
1. <span data-ttu-id="98453-106">File dalam **AlchemyInsights** folder harus memiliki ID aturan dan nama aturan dari [portal mitra Alkimia](https://alchemyportal.azurewebsites.net) dalam nama file.</span><span class="sxs-lookup"><span data-stu-id="98453-106">Files in the **AlchemyInsights** folder should have Rule ID and Rule Name from the [Alchemy Partner portal](https://alchemyportal.azurewebsites.net) in the filename.</span></span>
    1. <span data-ttu-id="98453-107">mantan.</span><span class="sxs-lookup"><span data-stu-id="98453-107">ex.</span></span> <span data-ttu-id="98453-108">***976-How-to-Enable-Litigation-Hold***</span><span class="sxs-lookup"><span data-stu-id="98453-108">***976-How-to-enable-litigation-hold***</span></span>
1. <span data-ttu-id="98453-109">Menggunakan metadata di bagian atas dari file ini sebagai template Anda.</span><span class="sxs-lookup"><span data-stu-id="98453-109">Use the metadata at the top of this file as your template.</span></span> <span data-ttu-id="98453-110">Tidak ada yang lain diperlukan.</span><span class="sxs-lookup"><span data-stu-id="98453-110">Nothing else is required.</span></span>
1. <span data-ttu-id="98453-111">Di [portal mitra Alkimia](https://alchemyportal.azurewebsites.net), menavigasi ke bagian **judul wawasan pelanggan:** dan menggunakannya sebagai awal titik untuk judul H1 Anda untuk wawasan.</span><span class="sxs-lookup"><span data-stu-id="98453-111">In the [Alchemy Partner portal](https://alchemyportal.azurewebsites.net), navigate down to the section **Customer Insight Title:** and use that as a starting point for your H1 title for the insight.</span></span> 
    > [!NOTE]
    > <span data-ttu-id="98453-112">Alkimia wawasan harus memiliki hanya satu H1 di bagian atas atau mereka akan istirahat dalam produksi.</span><span class="sxs-lookup"><span data-stu-id="98453-112">Alchemy Insights MUST have only a single H1 at the top or they will break in production.</span></span> <span data-ttu-id="98453-113">H2s tidak membuat begitu menggunakan **bold** atau lain Konvensi untuk menandai bagian terpisah.</span><span class="sxs-lookup"><span data-stu-id="98453-113">H2s dont render either so use **bold** or other conventions to signify separate sections.</span></span>
1. <span data-ttu-id="98453-114">Selanjutnya, mengisi di dalam tubuh teks menggunakan bahan rancangan di bagian Customer wawasan halaman aturan Alkimia</span><span class="sxs-lookup"><span data-stu-id="98453-114">Next, fill in the body text using the draft material in the Customer Insights section of the Alchemy Rule page</span></span>
    1. <span data-ttu-id="98453-115">Bullet daftar baik-baik saja</span><span class="sxs-lookup"><span data-stu-id="98453-115">Bulleted lists are fine</span></span>
    1. <span data-ttu-id="98453-116">Nomor Daftar terlalu</span><span class="sxs-lookup"><span data-stu-id="98453-116">Numbered lists too</span></span>
    1. <span data-ttu-id="98453-117">**Tebal** dan *miring* adalah OK</span><span class="sxs-lookup"><span data-stu-id="98453-117">**Bold** and *italic* are a-ok</span></span>
    1. <span data-ttu-id="98453-118">Link harus selalu menjadi salah satu **"link web" / eksternal** OR **deep-link ke elemen UI**, tidak internal link.</span><span class="sxs-lookup"><span data-stu-id="98453-118">Links should always be either **"links to web"/external** OR **deep-links to UI elements**, not internal links.</span></span>

<span data-ttu-id="98453-119">Dan ini benar-benar sudah agak terlalu lama.</span><span class="sxs-lookup"><span data-stu-id="98453-119">And this is really already a bit too long.</span></span> <span data-ttu-id="98453-120">Praktek terbaik adalah sekitar 400 karakter---</span><span class="sxs-lookup"><span data-stu-id="98453-120">Best practice is about 400 characters ---------------------------------</span></span>

<span data-ttu-id="98453-121">Setelah konten Anda siap, menariknya ke cabang hidup.</span><span class="sxs-lookup"><span data-stu-id="98453-121">Once your content is ready, pull it to the live branch.</span></span> <span data-ttu-id="98453-122">Kemudian, pergi ke [portal mitra Alkimia](https://alchemyportal.azurewebsites.net) dan masukkan nama file ke bidang url.</span><span class="sxs-lookup"><span data-stu-id="98453-122">Then, go to the [Alchemy Partner portal](https://alchemyportal.azurewebsites.net) and enter the filename into the url field.</span></span> <span data-ttu-id="98453-123">Pastikan wawasan ditinjau dan diterbitkan mengatakan "ya" dan kemudian klik Update aturan.</span><span class="sxs-lookup"><span data-stu-id="98453-123">Make sure Insight reviewed and published says "yes" and then click Update Rule.</span></span> <span data-ttu-id="98453-124">**(Ini akan tampak cantik dalam versi baru dari portal - merilis segera.)** 
 ![bidang url](media/for-content-team.PNG)</span><span class="sxs-lookup"><span data-stu-id="98453-124">**(This will look prettier in the new version of the portal - releasing soon.)**
![url field](media/for-content-team.PNG)</span></span>

