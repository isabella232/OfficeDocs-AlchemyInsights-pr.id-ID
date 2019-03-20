---
title: sama seperti nama file terbaik
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
ms.openlocfilehash: ec979c2f2246fa06945b79bbb9348a7a57ad5180
ms.sourcegitcommit: b3cf5130ac8118f0fed66abe5286aa80ee91af52
ms.translationtype: MT
ms.contentlocale: id-ID
ms.lasthandoff: 03/19/2019
ms.locfileid: "30683852"
---
# <a name="required-alchemy-header-h1-h2s-dont-work"></a><span data-ttu-id="0519e-102">Diperlukan Alkimia Header H1, H2's tidak bekerja.</span><span class="sxs-lookup"><span data-stu-id="0519e-102">Required Alchemy Header H1, H2's dont work.</span></span>
<span data-ttu-id="0519e-103">Best Practices dan pedoman untuk authoring Alkimia:</span><span class="sxs-lookup"><span data-stu-id="0519e-103">Best Practices and guidelines for Alchemy authoring:</span></span>

1. <span data-ttu-id="0519e-104">**Tidak sarang Alkimia wawasan dalam folder**- ini akan merusak struktur url.</span><span class="sxs-lookup"><span data-stu-id="0519e-104">**Do not nest Alchemy Insights in folders**- this will break the url structure.</span></span> <span data-ttu-id="0519e-105">Kami melihat ke memperbaiki ini.</span><span class="sxs-lookup"><span data-stu-id="0519e-105">We're looking into fixing this.</span></span>
1. <span data-ttu-id="0519e-106">File dalam **AlchemyInsights** folder harus memiliki nama file huruf kecil dengan tanda hubung untuk ruang ex.</span><span class="sxs-lookup"><span data-stu-id="0519e-106">Files in the **AlchemyInsights** folder should have lowercase filenames with hyphens for spaces ex.</span></span> <span data-ttu-id="0519e-107">***bagaimana-untuk-Aktifkan--penahanan litigasi***.</span><span class="sxs-lookup"><span data-stu-id="0519e-107">***how-to-enable-litigation-hold***.</span></span>
    1. <span data-ttu-id="0519e-108">Termasuk aturan ID atau ember ID dari [portal Alkimia mitra](https://alchemyportal.azurewebsites.net) di bidang ms.custom.</span><span class="sxs-lookup"><span data-stu-id="0519e-108">Include the Rule ID or bucket ID from the [Alchemy Partner portal](https://alchemyportal.azurewebsites.net) in the ms.custom field.</span></span> <span data-ttu-id="0519e-109">mantan.</span><span class="sxs-lookup"><span data-stu-id="0519e-109">ex.</span></span> <span data-ttu-id="0519e-110">***Ms.Custom: 100021***</span><span class="sxs-lookup"><span data-stu-id="0519e-110">***ms.custom: 100021***</span></span>
1. <span data-ttu-id="0519e-111">Menggunakan sisa metadata di bagian atas dari file ini sebagai template Anda.</span><span class="sxs-lookup"><span data-stu-id="0519e-111">Use the rest of the metadata at the top of this file as your template.</span></span>
1. <span data-ttu-id="0519e-112">Di [portal mitra Alkimia](https://alchemyportal.azurewebsites.net), menavigasi ke bagian **judul wawasan pelanggan:** dan menggunakannya sebagai awal titik untuk judul H1 Anda untuk wawasan.</span><span class="sxs-lookup"><span data-stu-id="0519e-112">In the [Alchemy Partner portal](https://alchemyportal.azurewebsites.net), navigate down to the section **Customer Insight Title:** and use that as a starting point for your H1 title for the insight.</span></span> 
    > [!NOTE]
    > <span data-ttu-id="0519e-113">Alkimia wawasan harus memiliki hanya satu H1 di bagian atas atau mereka akan istirahat dalam produksi.</span><span class="sxs-lookup"><span data-stu-id="0519e-113">Alchemy Insights MUST have only a single H1 at the top or they will break in production.</span></span> <span data-ttu-id="0519e-114">H2s tidak membuat begitu menggunakan **bold** atau lain Konvensi untuk menandai bagian terpisah.</span><span class="sxs-lookup"><span data-stu-id="0519e-114">H2s dont render either so use **bold** or other conventions to signify separate sections.</span></span>
1. <span data-ttu-id="0519e-115">Selanjutnya, mengisi di dalam tubuh teks menggunakan bahan rancangan di bagian Customer wawasan halaman aturan Alkimia</span><span class="sxs-lookup"><span data-stu-id="0519e-115">Next, fill in the body text using the draft material in the Customer Insights section of the Alchemy Rule page</span></span>
    1. <span data-ttu-id="0519e-116">Bullet daftar baik-baik saja</span><span class="sxs-lookup"><span data-stu-id="0519e-116">Bulleted lists are fine</span></span>
    1. <span data-ttu-id="0519e-117">Nomor Daftar terlalu</span><span class="sxs-lookup"><span data-stu-id="0519e-117">Numbered lists too</span></span>
    1. <span data-ttu-id="0519e-118">**Tebal** dan *miring* adalah OK</span><span class="sxs-lookup"><span data-stu-id="0519e-118">**Bold** and *italic* are a-ok</span></span>
    1. <span data-ttu-id="0519e-119">Link harus selalu menjadi salah satu **"link web" / eksternal** OR **deep-link ke elemen UI**, tidak internal link.</span><span class="sxs-lookup"><span data-stu-id="0519e-119">Links should always be either **"links to web"/external** OR **deep-links to UI elements**, not internal links.</span></span>
    1. <span data-ttu-id="0519e-120">Gambar tidak secara resmi didukung saat ini, tetapi itu adalah pada peta jalan.</span><span class="sxs-lookup"><span data-stu-id="0519e-120">Pictures are not officially supported at this time, but it's on the roadmap.</span></span>

<span data-ttu-id="0519e-121">Dan ini benar-benar sudah agak terlalu lama.</span><span class="sxs-lookup"><span data-stu-id="0519e-121">And this is really already a bit too long.</span></span> <span data-ttu-id="0519e-122">Praktek terbaik adalah sekitar 400 karakter---</span><span class="sxs-lookup"><span data-stu-id="0519e-122">Best practice is about 400 characters ---------------------------------</span></span>

<span data-ttu-id="0519e-123">Setelah konten Anda siap, menariknya ke cabang hidup.</span><span class="sxs-lookup"><span data-stu-id="0519e-123">Once your content is ready, pull it to the live branch.</span></span> <span data-ttu-id="0519e-124">Kemudian, pergi ke [portal mitra Alkimia](https://alchemyportal.azurewebsites.net) dan masukkan nama file ke bidang url.</span><span class="sxs-lookup"><span data-stu-id="0519e-124">Then, go to the [Alchemy Partner portal](https://alchemyportal.azurewebsites.net) and enter the filename into the url field.</span></span> <span data-ttu-id="0519e-125">M</span><span class="sxs-lookup"><span data-stu-id="0519e-125">M</span></span>