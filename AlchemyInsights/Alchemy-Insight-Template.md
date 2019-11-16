---
title: sama seperti nama file yang terbaik
ms.author: pebaum
author: pebaum
manager: jackiesm
ms.date: 4/27/2018
ms.audience: Admin
ms.topic: article
ROBOTS: NOINDEX, NOFOLLOW
localization_priority: Normal
ms.collection: Adm_O365
ms.custom: ''
ms.assetid: (guid of old soc version if any)
ms.openlocfilehash: 31a578800468e9f3a69fff4f6e2e1945943c779c
ms.sourcegitcommit: b43f77221f47b50c41197a448a9c26c423ce1ad5
ms.translationtype: MT
ms.contentlocale: id-ID
ms.lasthandoff: 11/15/2019
ms.locfileid: "35800048"
---
# <a name="required-alchemy-header-h1-h2s-dont-work"></a><span data-ttu-id="d143c-102">Diperlukan Alchemy header H1, H2's tidak bekerja.</span><span class="sxs-lookup"><span data-stu-id="d143c-102">Required Alchemy Header H1, H2's dont work.</span></span>
<span data-ttu-id="d143c-103">Praktik terbaik dan panduan untuk Alchemy authoring:</span><span class="sxs-lookup"><span data-stu-id="d143c-103">Best Practices and guidelines for Alchemy authoring:</span></span>

1. <span data-ttu-id="d143c-104">**Jangan sarang Alkimia wawasan dalam folder**-ini akan memecahkan struktur URL.</span><span class="sxs-lookup"><span data-stu-id="d143c-104">**Do not nest Alchemy Insights in folders**- this will break the url structure.</span></span> <span data-ttu-id="d143c-105">Kami sedang mencari untuk memperbaiki ini.</span><span class="sxs-lookup"><span data-stu-id="d143c-105">We're looking into fixing this.</span></span>
1. <span data-ttu-id="d143c-106">File di folder **Alchemyinsights** harus memiliki nama file huruf kecil dengan tanda hubung untuk spasi ex.</span><span class="sxs-lookup"><span data-stu-id="d143c-106">Files in the **AlchemyInsights** folder should have lowercase filenames with hyphens for spaces ex.</span></span> <span data-ttu-id="d143c-107">***bagaimana-untuk-mengaktifkan-litigasi-terus***.</span><span class="sxs-lookup"><span data-stu-id="d143c-107">***how-to-enable-litigation-hold***.</span></span>
    1. <span data-ttu-id="d143c-108">Sertakan ID aturan atau ID Bucket dari [portal partner Alkimia](https://alchemyportal.azurewebsites.net) di kolom ms. Custom.</span><span class="sxs-lookup"><span data-stu-id="d143c-108">Include the Rule ID or bucket ID from the [Alchemy Partner portal](https://alchemyportal.azurewebsites.net) in the ms.custom field.</span></span> <span data-ttu-id="d143c-109">Keluaran.</span><span class="sxs-lookup"><span data-stu-id="d143c-109">ex.</span></span> <span data-ttu-id="d143c-110">***Ms. Custom: 100021***</span><span class="sxs-lookup"><span data-stu-id="d143c-110">***ms.custom: 100021***</span></span>
1. <span data-ttu-id="d143c-111">Gunakan sisa metadata di bagian atas file ini sebagai template Anda.</span><span class="sxs-lookup"><span data-stu-id="d143c-111">Use the rest of the metadata at the top of this file as your template.</span></span>
1. <span data-ttu-id="d143c-112">Di [portal mitra Alkimia](https://alchemyportal.azurewebsites.net), navigasikan ke bagian **judul Insight pelanggan:** dan gunakan itu sebagai titik awal untuk judul H1 Anda untuk Insight.</span><span class="sxs-lookup"><span data-stu-id="d143c-112">In the [Alchemy Partner portal](https://alchemyportal.azurewebsites.net), navigate down to the section **Customer Insight Title:** and use that as a starting point for your H1 title for the insight.</span></span> 
    > [!NOTE]
    > <span data-ttu-id="d143c-113">Alkimia wawasan harus hanya satu H1 di bagian atas atau mereka akan pecah dalam produksi.</span><span class="sxs-lookup"><span data-stu-id="d143c-113">Alchemy Insights MUST have only a single H1 at the top or they will break in production.</span></span> <span data-ttu-id="d143c-114">H2s tidak membuat baik sehingga menggunakan **Bold** atau Konvensi lain untuk menandakan bagian yang terpisah.</span><span class="sxs-lookup"><span data-stu-id="d143c-114">H2s dont render either so use **bold** or other conventions to signify separate sections.</span></span>
1. <span data-ttu-id="d143c-115">Selanjutnya, isi teks tubuh menggunakan bahan draft di bagian customer Insights halaman aturan Alchemy</span><span class="sxs-lookup"><span data-stu-id="d143c-115">Next, fill in the body text using the draft material in the Customer Insights section of the Alchemy Rule page</span></span>
    1. <span data-ttu-id="d143c-116">Daftar Bullet yang baik</span><span class="sxs-lookup"><span data-stu-id="d143c-116">Bulleted lists are fine</span></span>
    1. <span data-ttu-id="d143c-117">Daftar bernomor juga</span><span class="sxs-lookup"><span data-stu-id="d143c-117">Numbered lists too</span></span>
    1. <span data-ttu-id="d143c-118">**Bold** dan *Italic* adalah-OK</span><span class="sxs-lookup"><span data-stu-id="d143c-118">**Bold** and *italic* are a-ok</span></span>
    1. <span data-ttu-id="d143c-119">Link harus selalu baik **"link ke web"/eksternal** atau **Deep-link ke elemen UI**, bukan link internal.</span><span class="sxs-lookup"><span data-stu-id="d143c-119">Links should always be either **"links to web"/external** OR **deep-links to UI elements**, not internal links.</span></span>
    1. <span data-ttu-id="d143c-120">Gambar tidak resmi didukung saat ini, tapi itu pada peta jalan.</span><span class="sxs-lookup"><span data-stu-id="d143c-120">Pictures are not officially supported at this time, but it's on the roadmap.</span></span>

<span data-ttu-id="d143c-121">Dan ini sebenarnya sudah agak terlalu lama.</span><span class="sxs-lookup"><span data-stu-id="d143c-121">And this is really already a bit too long.</span></span> <span data-ttu-id="d143c-122">Praktik terbaik adalah sekitar 400 karakter---------------------------------</span><span class="sxs-lookup"><span data-stu-id="d143c-122">Best practice is about 400 characters ---------------------------------</span></span>

<span data-ttu-id="d143c-123">Setelah konten Anda siap, tarik ke Live Branch.</span><span class="sxs-lookup"><span data-stu-id="d143c-123">Once your content is ready, pull it to the live branch.</span></span> <span data-ttu-id="d143c-124">Kemudian, pergi ke [portal mitra Alkimia](https://alchemyportal.azurewebsites.net) dan masukkan nama file ke dalam kolom URL.</span><span class="sxs-lookup"><span data-stu-id="d143c-124">Then, go to the [Alchemy Partner portal](https://alchemyportal.azurewebsites.net) and enter the filename into the url field.</span></span> 