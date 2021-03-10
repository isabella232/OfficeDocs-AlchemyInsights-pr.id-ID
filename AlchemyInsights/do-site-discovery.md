---
title: Melakukan pencarian situs
ms.author: v-smandalika
author: v-smandalika
manager: dansimp
ms.date: 03/08/2021
audience: Admin
ms.topic: article
ms.service: o365-administration
ROBOTS: NOINDEX, NOFOLLOW
localization_priority: Priority
ms.collection: Adm_O365
ms.custom:
- "9143"
- "9005291"
ms.openlocfilehash: bdf94220de45d92f63e56501ea4e35389224d25c
ms.sourcegitcommit: 475a9eaa095812091991857df6cf6490a8bbe179
ms.translationtype: MT
ms.contentlocale: id-ID
ms.lasthandoff: 03/08/2021
ms.locfileid: "50693485"
---
# <a name="do-site-discovery"></a><span data-ttu-id="41d9a-102">Melakukan pencarian situs</span><span class="sxs-lookup"><span data-stu-id="41d9a-102">Do site discovery</span></span>

<span data-ttu-id="41d9a-103">Jika organisasi masih menggunakan aplikasi dan paket web warisan untuk menggunakan mode Internet Explorer (yang dilakukan oleh sebagian besar pelanggan), maka Anda harus melakukan beberapa penemuan situs tambahan.</span><span class="sxs-lookup"><span data-stu-id="41d9a-103">If your organization still uses legacy web applications and plans to use Internet Explorer mode (which most customers do), then you should do some additional site discovery.</span></span>

<span data-ttu-id="41d9a-104">**Anda telah menerapkan versi Microsoft Edge yang lebih lama**</span><span class="sxs-lookup"><span data-stu-id="41d9a-104">**You've already deployed an older version of Microsoft Edge**</span></span>

<span data-ttu-id="41d9a-105">Jika Anda sudah mengonfigurasi daftar situs perusahaan Anda untuk bekerja untuk versi warisan Microsoft Edge, maka penemuan situs Anda hampir selesai.</span><span class="sxs-lookup"><span data-stu-id="41d9a-105">If you've already configured your Enterprise Site List to work for the legacy version of Microsoft Edge, then your site discovery is almost done.</span></span> <span data-ttu-id="41d9a-106">Satu hal yang mungkin perlu Anda lakukan adalah menambahkan situs netral.</span><span class="sxs-lookup"><span data-stu-id="41d9a-106">The one thing you might need to do is add neutral sites.</span></span>

<span data-ttu-id="41d9a-107">Situs netral biasanya adalah situs yang menyediakan masuk tunggal (SSO).</span><span class="sxs-lookup"><span data-stu-id="41d9a-107">Neutral sites are typically sites that provide single sign-on (SSO).</span></span> <span data-ttu-id="41d9a-108">Jika Anda masuk ke situs netral dari Microsoft Edge, maka Anda ingin tetap menggunakan Microsoft Edge untuk mengautentikasi.</span><span class="sxs-lookup"><span data-stu-id="41d9a-108">If you go to a neutral site from Microsoft Edge, then you want to stay in Microsoft Edge to authenticate.</span></span> <span data-ttu-id="41d9a-109">Jika Anda masuk ke situs netral dalam mode Internet Explorer, maka Anda ingin tetap menggunakan mode Internet Explorer untuk mengautentikasi.</span><span class="sxs-lookup"><span data-stu-id="41d9a-109">If you go to a neutral site in Internet Explorer mode, then you want to stay in Internet Explorer mode to authenticate.</span></span>

<span data-ttu-id="41d9a-110">Identifikasi SSO atau situs netral lainnya yang Anda gunakan dan tambahkan ke daftar situs perusahaan Anda.</span><span class="sxs-lookup"><span data-stu-id="41d9a-110">Identify any SSO or other neutral sites that you use and add these to your Enterprise Site List.</span></span>

<span data-ttu-id="41d9a-111">**Internet Explorer adalah browser default Anda**</span><span class="sxs-lookup"><span data-stu-id="41d9a-111">**Internet Explorer is your default browser**</span></span>

<span data-ttu-id="41d9a-112">Jika Anda hanya menggunakan Internet Explorer sekarang, Anda mungkin tidak mengetahui situs mana yang telah dimutakhirkan ke standar web modern dan yang masih memerlukan Internet Explorer.</span><span class="sxs-lookup"><span data-stu-id="41d9a-112">If you're only using Internet Explorer now, you might not know which sites have upgraded to modern web standards and which still require Internet Explorer.</span></span> <span data-ttu-id="41d9a-113">Anda akan ingin menemukan dan menambahkan situs ini ke daftar situs perusahaan sehingga Anda bisa menggunakan mode Internet Explorer hanya untuk situs tersebut.</span><span class="sxs-lookup"><span data-stu-id="41d9a-113">You'll want to find and add these sites to the Enterprise Site List so that you can use Internet Explorer mode only for those sites.</span></span>

> [!NOTE]
> <span data-ttu-id="41d9a-114">[Penemuan situs perusahaan](https://docs.microsoft.com/internet-explorer/ie11-deploy-guide/collect-data-using-enterprise-site-discovery) menemukan situs yang mungkin memerlukan mode Internet Explorer.</span><span class="sxs-lookup"><span data-stu-id="41d9a-114">[Enterprise Site Discovery](https://docs.microsoft.com/internet-explorer/ie11-deploy-guide/collect-data-using-enterprise-site-discovery) discovers sites that might need Internet Explorer mode.</span></span> <span data-ttu-id="41d9a-115">Hal ini dapat mengumpulkan data pada komputer yang menjalankan Windows Internet Explorer 8 melalui Internet Explorer 11 di Windows 10, Windows 8,1, atau Windows 7.</span><span class="sxs-lookup"><span data-stu-id="41d9a-115">It can collect data on computers running Windows Internet Explorer 8 through Internet Explorer 11 on Windows 10, Windows 8.1, or Windows 7.</span></span>

<span data-ttu-id="41d9a-116">**Menganalisis data**</span><span class="sxs-lookup"><span data-stu-id="41d9a-116">**Analyze the data**</span></span>

<span data-ttu-id="41d9a-117">Setelah Anda mengumpulkan data situs, kami merekomendasikan proses empat langkah berikut ini untuk menganalisis data:</span><span class="sxs-lookup"><span data-stu-id="41d9a-117">After you've collected site data, we recommend the following four-step process to analyze the data:</span></span>
1. <span data-ttu-id="41d9a-118">Urutkan data menurut domain, lalu menurut URL.</span><span class="sxs-lookup"><span data-stu-id="41d9a-118">Sort the data by domain, and then by URL.</span></span>
2. <span data-ttu-id="41d9a-119">Tentukan batas aplikasi untuk mengonfigurasi mode Internet Explorer.</span><span class="sxs-lookup"><span data-stu-id="41d9a-119">Define the boundaries of an app to configure for Internet Explorer mode.</span></span> <span data-ttu-id="41d9a-120">Anda ingin menyertakan semua situs dan kontrol web yang menentukan aplikasi tersebut, tetapi Anda tidak ingin menyertakan situs dan kontrol tambahan.</span><span class="sxs-lookup"><span data-stu-id="41d9a-120">You want to include all the sites and web controls that define the app, but you don't want to include extra sites and controls.</span></span> <span data-ttu-id="41d9a-121">Beberapa situs mungkin sesederhana *https://contoso.com/app1* sementara yang lain mungkin mengharuskan Anda untuk menentukan beberapa situs dan halaman.</span><span class="sxs-lookup"><span data-stu-id="41d9a-121">Some sites might be as simple as *https://contoso.com/app1* while others might require you to define multiple sites and pages.</span></span>
3. <span data-ttu-id="41d9a-122">Uji aplikasi untuk memverifikasi bahwa aplikasi tidak berfungsi secara native.</span><span class="sxs-lookup"><span data-stu-id="41d9a-122">Test the app to verify that it doesn't work natively.</span></span> <span data-ttu-id="41d9a-123">Banyak situs akan menawarkan konten modern saat mereka mendeteksi browser modern dan hanya menawarkan konten warisan saat mereka mendeteksi Internet Explorer.</span><span class="sxs-lookup"><span data-stu-id="41d9a-123">Many sites will offer modern content when they detect a modern browser and only offer legacy content when they detect Internet Explorer.</span></span>
4. <span data-ttu-id="41d9a-124">Tambahkan aplikasi ke daftar situs perusahaan Anda jika pengujian gagal.</span><span class="sxs-lookup"><span data-stu-id="41d9a-124">Add the app to your Enterprise Site List if it fails testing.</span></span>

> [!NOTE]
> <span data-ttu-id="41d9a-125">Sebagai praktik terbaik, Kelompokkan semua situs yang terdiri dari aplikasi.</span><span class="sxs-lookup"><span data-stu-id="41d9a-125">As a best practice, group all of the sites that comprise an app.</span></span> <span data-ttu-id="41d9a-126">Dengan cara ini, saat Anda memutakhirkan aplikasi, lebih mudah untuk menghapus seluruh situs dari mode Internet Explorer dan mulai menggunakan browser modern untuk aplikasi tersebut.</span><span class="sxs-lookup"><span data-stu-id="41d9a-126">This way, when you upgrade an app, it's easier to remove the entire site from Internet Explorer mode and start using a modern browser for that app.</span></span>

<span data-ttu-id="41d9a-127">Setelah Anda selesai dengan penemuan situs dan Anda telah menganalisis data, Anda siap untuk mulai melihat strategi saluran Anda.</span><span class="sxs-lookup"><span data-stu-id="41d9a-127">Once you're done with site discovery and you've analyzed the data, you're ready to start looking at your channel strategy.</span></span>

