---
title: Menyimpan situs atau daftar sebagai Templat
ms.author: pebaum
author: pebaum
ms.audience: ITPro
ms.topic: article
ms.service: o365-administration
ROBOTS: NOINDEX, NOFOLLOW
localization_priority: Normal
ms.assetid: 368ff1fa-82cf-4a07-986e-140b212ffc5c
ms.openlocfilehash: 37ae727aa6dd6af94d0d833ce972aec413d90194
ms.sourcegitcommit: c6692ce0fa1358ec3529e59ca0ecdfdea4cdc759
ms.translationtype: MT
ms.contentlocale: id-ID
ms.lasthandoff: 09/14/2020
ms.locfileid: "47727534"
---
# <a name="save-site-or-list-as-a-template"></a><span data-ttu-id="d214a-102">Menyimpan situs atau daftar sebagai Templat</span><span class="sxs-lookup"><span data-stu-id="d214a-102">Save site or list as a template</span></span>

<span data-ttu-id="d214a-103">Templat situs SharePoint adalah definisi bawaan yang dirancang untuk kebutuhan bisnis tertentu.</span><span class="sxs-lookup"><span data-stu-id="d214a-103">SharePoint site templates are prebuilt definitions designed around a particular business need.</span></span> <span data-ttu-id="d214a-104">Untuk informasi selengkapnya, lihat [menggunakan templat untuk membuat berbagai macam situs SharePoint](https://support.office.com/article/using-templates-to-create-different-kinds-of-sharepoint-sites-449eccec-ff99-4cf3-b62e-dcfee37e8da4).</span><span class="sxs-lookup"><span data-stu-id="d214a-104">For more information, see [Using templates to create different kinds of SharePoint sites](https://support.office.com/article/using-templates-to-create-different-kinds-of-sharepoint-sites-449eccec-ff99-4cf3-b62e-dcfee37e8da4).</span></span>

<span data-ttu-id="d214a-105">Berikut adalah beberapa masalah/solusi umum terkait penyimpanan situs atau daftar sebagai Templat di SharePoint online.</span><span class="sxs-lookup"><span data-stu-id="d214a-105">Here are some common issues/solutions regarding Saving a Site or List as a template in SharePoint Online.</span></span>

<span data-ttu-id="d214a-106">**Tombol Simpan situs/daftar Templat tidak tersedia atau tidak ada**.</span><span class="sxs-lookup"><span data-stu-id="d214a-106">**Save site/list template button is not available or missing**.</span></span> 

- <span data-ttu-id="d214a-107">Administrator perlu memperbolehkan skrip kustom untuk mengaktifkan fitur Templat.</span><span class="sxs-lookup"><span data-stu-id="d214a-107">Administrators will need to Allow Custom Script to enable the template features.</span></span> <span data-ttu-id="d214a-108">Untuk langkah, contoh dan pertimbangan mendetail, lihat [memperbolehkan atau mencegah skrip kustom](https://docs.microsoft.com/sharepoint/allow-or-prevent-custom-script).</span><span class="sxs-lookup"><span data-stu-id="d214a-108">For detailed steps, examples and considerations see [Allow or prevent custom script](https://docs.microsoft.com/sharepoint/allow-or-prevent-custom-script).</span></span>


- <span data-ttu-id="d214a-109">Perintah Simpan situs sebagai Templat tidak didukung dan bisa menyebabkan masalah pada situs yang menggunakan infrastruktur penerbitan SharePoint Server.</span><span class="sxs-lookup"><span data-stu-id="d214a-109">The Save site as template command is not supported and can cause problems on sites that use the SharePoint Server Publishing Infrastructure.</span></span>


<span data-ttu-id="d214a-110">**Templat situs tidak bisa dibuat atau tidak berfungsi dengan benar**</span><span class="sxs-lookup"><span data-stu-id="d214a-110">**The site template cannot be created or does not work correctly**</span></span>

- <span data-ttu-id="d214a-111">Templat mungkin kehilangan [fitur](https://social.technet.microsoft.com/wiki/contents/articles/14423.sharepoint-2013-existing-features-guid.aspx) dan tidak dapat diaktifkan.</span><span class="sxs-lookup"><span data-stu-id="d214a-111">The template may be missing a [feature](https://social.technet.microsoft.com/wiki/contents/articles/14423.sharepoint-2013-existing-features-guid.aspx) and won’t activate.</span></span> <span data-ttu-id="d214a-112">Jika fitur tidak tersedia untuk diaktifkan dalam kumpulan situs saat ini, Anda tidak bisa menggunakan templat situs untuk membuat situs.</span><span class="sxs-lookup"><span data-stu-id="d214a-112">If the feature is not available to activate in the current site collection, you cannot use the site template to create a site.</span></span>


- <span data-ttu-id="d214a-113">Periksa untuk melihat apakah ada daftar atau Pustaka yang melebihi [ambang batas batas tampilan daftar](https://support.office.com/article/Manage-large-lists-and-libraries-in-SharePoint-B8588DAE-9387-48C2-9248-C24122F07C59) item 5000 karena hal ini bisa memblokir pembuatan Templat situs.</span><span class="sxs-lookup"><span data-stu-id="d214a-113">Check to see if any lists or libraries exceed the [List View Limit Threshold](https://support.office.com/article/Manage-large-lists-and-libraries-in-SharePoint-B8588DAE-9387-48C2-9248-C24122F07C59) of 5000 items as this can block creation of a site template.</span></span>


- <span data-ttu-id="d214a-114">Situs tersebut mungkin menggunakan terlalu banyak sumber daya dan karena itu Templat situs melebihi batas 50 megabyte (MB).</span><span class="sxs-lookup"><span data-stu-id="d214a-114">The site may be using too many resources and therefore the site template exceeds the 50 megabyte (MB) limit.</span></span>


- <span data-ttu-id="d214a-115">Ada masalah menampilkan data dari daftar yang menggunakan kolom pencarian.</span><span class="sxs-lookup"><span data-stu-id="d214a-115">There are problems displaying data from a list that uses a lookup column.</span></span> <span data-ttu-id="d214a-116">Untuk informasi selengkapnya, lihat [Daftar yang dihasilkan Templat tidak menampilkan data dari daftar pencarian yang benar di SharePoint online](https://docs.microsoft.com/sharepoint/support/lists-and-libraries/template-generated-list-incorrect-data).</span><span class="sxs-lookup"><span data-stu-id="d214a-116">For more information, see [Template-generated list doesn’t display data from the correct lookup list in SharePoint Online](https://docs.microsoft.com/sharepoint/support/lists-and-libraries/template-generated-list-incorrect-data).</span></span>


<span data-ttu-id="d214a-117">Untuk informasi mendetail tentang masalah umum dan solusi, silakan rujuk, [membuat dan menggunakan templat situs](https://support.office.com/article/Create-and-use-site-templates-60371B0F-00E0-4C49-A844-34759EBDD989).</span><span class="sxs-lookup"><span data-stu-id="d214a-117">For more detailed information on common problems and solutions please reference, [Create and use site templates](https://support.office.com/article/Create-and-use-site-templates-60371B0F-00E0-4C49-A844-34759EBDD989).</span></span>

