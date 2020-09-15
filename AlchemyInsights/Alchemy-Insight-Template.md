---
title: sama seperti nama file yang terbaik
ms.author: pebaum
author: pebaum
manager: jackiesm
ms.date: 04/21/2020
ms.audience: Admin
ms.topic: article
ms.service: o365-administration
ROBOTS: NOINDEX, NOFOLLOW
localization_priority: Normal
ms.collection: Adm_O365
ms.custom: ''
ms.assetid: (guid of old soc version if any)
ms.openlocfilehash: 113d01e0fc92cc9845e585919ab05f386d6892bb
ms.sourcegitcommit: c6692ce0fa1358ec3529e59ca0ecdfdea4cdc759
ms.translationtype: MT
ms.contentlocale: id-ID
ms.lasthandoff: 09/14/2020
ms.locfileid: "47664137"
---
# <a name="required-alchemy-header-h1-h2s-dont-work"></a><span data-ttu-id="9c1d1-102">"Header Alchemy yang diperlukan H1, H2's tidak berfungsi."</span><span class="sxs-lookup"><span data-stu-id="9c1d1-102">"Required Alchemy Header H1, H2's dont work."</span></span>
<span data-ttu-id="9c1d1-103">Praktik terbaik dan panduan untuk Alkimia penulisan:</span><span class="sxs-lookup"><span data-stu-id="9c1d1-103">Best Practices and guidelines for Alchemy authoring:</span></span>

1. <span data-ttu-id="9c1d1-104">**Jangan bersarang wawasan Alchemy dalam folder**-ini akan merusak struktur URL.</span><span class="sxs-lookup"><span data-stu-id="9c1d1-104">**Do not nest Alchemy Insights in folders**- this will break the url structure.</span></span> <span data-ttu-id="9c1d1-105">Kami sedang berusaha memperbaiki hal ini.</span><span class="sxs-lookup"><span data-stu-id="9c1d1-105">We're looking into fixing this.</span></span>
1. <span data-ttu-id="9c1d1-106">File dalam folder **Alchemyinsights** harus memiliki nama file huruf kecil dengan tanda hubung untuk spasi.</span><span class="sxs-lookup"><span data-stu-id="9c1d1-106">Files in the **AlchemyInsights** folder should have lowercase filenames with hyphens for spaces ex.</span></span> <span data-ttu-id="9c1d1-107">***cara-untuk-mengaktifkan-litigasi-Hold***.</span><span class="sxs-lookup"><span data-stu-id="9c1d1-107">***how-to-enable-litigation-hold***.</span></span>
    1. <span data-ttu-id="9c1d1-108">Sertakan ID aturan atau ID Bucket dari [portal mitra Alkimia](https://alchemyportal.azurewebsites.net) di bidang ms. kustom.</span><span class="sxs-lookup"><span data-stu-id="9c1d1-108">Include the Rule ID or bucket ID from the [Alchemy Partner portal](https://alchemyportal.azurewebsites.net) in the ms.custom field.</span></span> <span data-ttu-id="9c1d1-109">KS.</span><span class="sxs-lookup"><span data-stu-id="9c1d1-109">ex.</span></span> <span data-ttu-id="9c1d1-110">***Ms. kustom: 100021***</span><span class="sxs-lookup"><span data-stu-id="9c1d1-110">***ms.custom: 100021***</span></span>
1. <span data-ttu-id="9c1d1-111">Gunakan sisa metadata di bagian atas file ini sebagai Templat Anda.</span><span class="sxs-lookup"><span data-stu-id="9c1d1-111">Use the rest of the metadata at the top of this file as your template.</span></span>
1. <span data-ttu-id="9c1d1-112">Di [portal mitra Alkimia](https://alchemyportal.azurewebsites.net), navigasikan ke bagian **judul Insight pelanggan:** dan gunakan sebagai titik awal untuk judul H1 Anda untuk Insight.</span><span class="sxs-lookup"><span data-stu-id="9c1d1-112">In the [Alchemy Partner portal](https://alchemyportal.azurewebsites.net), navigate down to the section **Customer Insight Title:** and use that as a starting point for your H1 title for the insight.</span></span> 
    > [!NOTE]
    > <span data-ttu-id="9c1d1-113">Wawasan Alkimia harus memiliki hanya satu H1 di bagian atas atau akan hancur dalam produksi.</span><span class="sxs-lookup"><span data-stu-id="9c1d1-113">Alchemy Insights MUST have only a single H1 at the top or they will break in production.</span></span> <span data-ttu-id="9c1d1-114">H2s tidak merender baik gunakan **tebal** atau Konvensi lainnya untuk menandakan bagian terpisah.</span><span class="sxs-lookup"><span data-stu-id="9c1d1-114">H2s dont render either so use **bold** or other conventions to signify separate sections.</span></span>
1. <span data-ttu-id="9c1d1-115">Berikutnya, isi teks isi menggunakan materi draf di bagian wawasan pelanggan dari halaman aturan Alchemy</span><span class="sxs-lookup"><span data-stu-id="9c1d1-115">Next, fill in the body text using the draft material in the Customer Insights section of the Alchemy Rule page</span></span>
    1. <span data-ttu-id="9c1d1-116">Daftar berpoin baik-baik saja</span><span class="sxs-lookup"><span data-stu-id="9c1d1-116">Bulleted lists are fine</span></span>
    1. <span data-ttu-id="9c1d1-117">Daftar bernomor terlalu</span><span class="sxs-lookup"><span data-stu-id="9c1d1-117">Numbered lists too</span></span>
    1. <span data-ttu-id="9c1d1-118">**Tebal** dan *miring* adalah-OK</span><span class="sxs-lookup"><span data-stu-id="9c1d1-118">**Bold** and *italic* are a-ok</span></span>
    1. <span data-ttu-id="9c1d1-119">Link harus selalu berupa **"link ke web"/eksternal** atau **Deep-link ke elemen UI**, bukan link internal.</span><span class="sxs-lookup"><span data-stu-id="9c1d1-119">Links should always be either **"links to web"/external** OR **deep-links to UI elements**, not internal links.</span></span>
    1. <span data-ttu-id="9c1d1-120">Gambar tidak didukung secara resmi pada saat ini, tetapi pada peta jalan.</span><span class="sxs-lookup"><span data-stu-id="9c1d1-120">Pictures are not officially supported at this time, but it's on the roadmap.</span></span>

<span data-ttu-id="9c1d1-121">Dan ini sudah terlalu panjang.</span><span class="sxs-lookup"><span data-stu-id="9c1d1-121">And this is really already a bit too long.</span></span> <span data-ttu-id="9c1d1-122">Praktik terbaik adalah sekitar 400 karakter---------------------------------</span><span class="sxs-lookup"><span data-stu-id="9c1d1-122">Best practice is about 400 characters ---------------------------------</span></span>

<span data-ttu-id="9c1d1-123">Setelah konten Anda siap, tarik ke cabang langsung.</span><span class="sxs-lookup"><span data-stu-id="9c1d1-123">Once your content is ready, pull it to the live branch.</span></span> <span data-ttu-id="9c1d1-124">Lalu, masuk ke [portal mitra Alkimia](https://alchemyportal.azurewebsites.net) dan masukkan nama file ke dalam bidang URL.</span><span class="sxs-lookup"><span data-stu-id="9c1d1-124">Then, go to the [Alchemy Partner portal](https://alchemyportal.azurewebsites.net) and enter the filename into the url field.</span></span> 