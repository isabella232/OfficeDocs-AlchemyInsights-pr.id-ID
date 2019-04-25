---
title: Menyimpan situs atau daftar sebagai template
ms.author: kirks
author: Techwriter40
ms.audience: ITPro
ms.topic: article
ROBOTS: NOINDEX, NOFOLLOW
localization_priority: Normal
ms.assetid: 368ff1fa-82cf-4a07-986e-140b212ffc5c
ms.openlocfilehash: 7930551c0938501d006f791491594f9d6d9ba260
ms.sourcegitcommit: 03258ec4f5476a1ea6dd3a31d17bda815bc5a18a
ms.translationtype: MT
ms.contentlocale: id-ID
ms.lasthandoff: 04/24/2019
ms.locfileid: "33243437"
---
# <a name="save-site-or-list-as-a-template"></a><span data-ttu-id="86c3e-102">Menyimpan situs atau daftar sebagai template</span><span class="sxs-lookup"><span data-stu-id="86c3e-102">Save site or list as a template</span></span>

<span data-ttu-id="86c3e-103">Template situs SharePoint adalah prebuilt definisi yang dirancang di sekitar kebutuhan bisnis tertentu.</span><span class="sxs-lookup"><span data-stu-id="86c3e-103">SharePoint site templates are prebuilt definitions designed around a particular business need.</span></span> <span data-ttu-id="86c3e-104">Untuk selengkapnya, lihat [menggunakan template untuk membuat berbagai jenis situs SharePoint](https://support.office.com/en-us/article/using-templates-to-create-different-kinds-of-sharepoint-sites-449eccec-ff99-4cf3-b62e-dcfee37e8da4).</span><span class="sxs-lookup"><span data-stu-id="86c3e-104">For more information, see [Using templates to create different kinds of SharePoint sites](https://support.office.com/en-us/article/using-templates-to-create-different-kinds-of-sharepoint-sites-449eccec-ff99-4cf3-b62e-dcfee37e8da4).</span></span>

<span data-ttu-id="86c3e-105">Berikut adalah beberapa masalah/solusi umum mengenai menyimpan situs atau daftar sebagai template dalam SharePoint Online.</span><span class="sxs-lookup"><span data-stu-id="86c3e-105">Here are some common issues/solutions regarding Saving a Site or List as a template in SharePoint Online.</span></span>

<span data-ttu-id="86c3e-106">**Menyimpan daftar situs/template tombol ini tidak tersedia atau hilang**.</span><span class="sxs-lookup"><span data-stu-id="86c3e-106">**Save site/list template button is not available or missing**.</span></span> 

- <span data-ttu-id="86c3e-107">Administrator akan perlu untuk membolehkan Custom Script untuk mengaktifkan fitur template.</span><span class="sxs-lookup"><span data-stu-id="86c3e-107">Administrators will need to Allow Custom Script to enable the template features.</span></span> <span data-ttu-id="86c3e-108">Untuk langkah-langkah rinci, contoh dan pertimbangan Lihat [Bolehkan atau mencegah script kustom](https://docs.microsoft.com/en-us/sharepoint/allow-or-prevent-custom-script).</span><span class="sxs-lookup"><span data-stu-id="86c3e-108">For detailed steps, examples and considerations see [Allow or prevent custom script](https://docs.microsoft.com/en-us/sharepoint/allow-or-prevent-custom-script).</span></span>


- <span data-ttu-id="86c3e-109">Situs Simpan sebagai perintah template tidak didukung dan dapat menyebabkan masalah pada situs yang menggunakan SharePoint Server Publishing infrastruktur.</span><span class="sxs-lookup"><span data-stu-id="86c3e-109">The Save site as template command is not supported and can cause problems on sites that use the SharePoint Server Publishing Infrastructure.</span></span>


<span data-ttu-id="86c3e-110">**Situs template tidak dapat dibuat atau tidak berfungsi dengan benar**</span><span class="sxs-lookup"><span data-stu-id="86c3e-110">**The site template cannot be created or does not work correctly**</span></span>

- <span data-ttu-id="86c3e-111">Template mungkin hilang [fitur](https://social.technet.microsoft.com/wiki/contents/articles/14423.sharepoint-2013-existing-features-guid.aspx) dan tidak akan diaktifkan.</span><span class="sxs-lookup"><span data-stu-id="86c3e-111">The template may be missing a [feature](https://social.technet.microsoft.com/wiki/contents/articles/14423.sharepoint-2013-existing-features-guid.aspx) and won’t activate.</span></span> <span data-ttu-id="86c3e-112">Jika fitur ini tidak tersedia untuk mengaktifkan dalam koleksi situs saat ini, Anda tidak dapat menggunakan situs template untuk membuat situs.</span><span class="sxs-lookup"><span data-stu-id="86c3e-112">If the feature is not available to activate in the current site collection, you cannot use the site template to create a site.</span></span>


- <span data-ttu-id="86c3e-113">Periksa untuk melihat jika atau daftar perpustakaan melebihi [Ambang batas daftar View](https://support.office.com/en-us/article/Manage-large-lists-and-libraries-in-SharePoint-B8588DAE-9387-48C2-9248-C24122F07C59) 5000 item seperti ini dapat menghalangi pembentukan situs template.</span><span class="sxs-lookup"><span data-stu-id="86c3e-113">Check to see if any lists or libraries exceed the [List View Limit Threshold](https://support.office.com/en-us/article/Manage-large-lists-and-libraries-in-SharePoint-B8588DAE-9387-48C2-9248-C24122F07C59) of 5000 items as this can block creation of a site template.</span></span>


- <span data-ttu-id="86c3e-114">Situs mungkin menggunakan terlalu banyak sumber daya dan karena itu situs template melebihi batas 50 megabyte (MB).</span><span class="sxs-lookup"><span data-stu-id="86c3e-114">The site may be using too many resources and therefore the site template exceeds the 50 megabyte (MB) limit.</span></span>


- <span data-ttu-id="86c3e-115">Ada masalah yang menampilkan data dari daftar yang menggunakan kolom pencarian.</span><span class="sxs-lookup"><span data-stu-id="86c3e-115">There are problems displaying data from a list that uses a lookup column.</span></span> <span data-ttu-id="86c3e-116">Untuk informasi lebih lanjut, lihat [Daftar Template yang dihasilkan tidak menampilkan data dari daftar SharePoint Online benar lookup](https://support.office.com/en-us/article/template-generated-list-doesn-t-display-correct-data-for-a-column-in-sharepoint-online-20430b62-e40c-4f6f-8889-aa24e80d605a).</span><span class="sxs-lookup"><span data-stu-id="86c3e-116">For more information, see [Template-generated list doesn’t display data from the correct lookup list in SharePoint Online](https://support.office.com/en-us/article/template-generated-list-doesn-t-display-correct-data-for-a-column-in-sharepoint-online-20430b62-e40c-4f6f-8889-aa24e80d605a).</span></span>


<span data-ttu-id="86c3e-117">Untuk informasi lebih rinci tentang masalah umum dan solusi silakan referensi, [membuat dan menggunakan situs template](https://support.office.com/en-us/article/Create-and-use-site-templates-60371B0F-00E0-4C49-A844-34759EBDD989).</span><span class="sxs-lookup"><span data-stu-id="86c3e-117">For more detailed information on common problems and solutions please reference, [Create and use site templates](https://support.office.com/en-us/article/Create-and-use-site-templates-60371B0F-00E0-4C49-A844-34759EBDD989).</span></span>

