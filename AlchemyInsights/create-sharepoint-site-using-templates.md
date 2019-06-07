---
title: Membuat situs di SharePoint Online
ms.author: kirks
author: Techwriter40
manager: pamgreen
ms.audience: Admin
ms.topic: article
ROBOTS: NOINDEX, NOFOLLOW
localization_priority: Normal
ms.collection: Adm_O365
ms.custom: ''
ms.assetid: 84f2b70e-2b23-4039-8305-85783798feed
ms.openlocfilehash: a964751e52972875a8794ce311546f5816a36ca6
ms.sourcegitcommit: 4b7e478ce700c0b781efec3857ac4dce5bdf00c6
ms.translationtype: MT
ms.contentlocale: id-ID
ms.lasthandoff: 06/07/2019
ms.locfileid: "34753711"
---
# <a name="create-sharepoint-sites-using-templates"></a><span data-ttu-id="9e4ca-102">Buat situs SharePoint menggunakan template</span><span class="sxs-lookup"><span data-stu-id="9e4ca-102">Create SharePoint sites using templates</span></span>

<span data-ttu-id="9e4ca-103">Template situs SharePoint adalah prebuilt definisi yang dirancang di sekitar kebutuhan bisnis tertentu.</span><span class="sxs-lookup"><span data-stu-id="9e4ca-103">SharePoint site templates are prebuilt definitions designed around a particular business need.</span></span> <span data-ttu-id="9e4ca-104">Untuk selengkapnya, lihat [menggunakan template untuk membuat berbagai jenis situs SharePoint](https://support.office.com/article/using-templates-to-create-different-kinds-of-sharepoint-sites-449eccec-ff99-4cf3-b62e-dcfee37e8da4).</span><span class="sxs-lookup"><span data-stu-id="9e4ca-104">For more information, see [Using templates to create different kinds of SharePoint sites](https://support.office.com/article/using-templates-to-create-different-kinds-of-sharepoint-sites-449eccec-ff99-4cf3-b62e-dcfee37e8da4).</span></span>

<span data-ttu-id="9e4ca-105">Berikut adalah beberapa masalah/solusi umum mengenai menyimpan situs atau daftar sebagai template dalam Sharepoint Online.</span><span class="sxs-lookup"><span data-stu-id="9e4ca-105">Here are some common issues/solutions regarding Saving a Site or List as a template in Sharepoint Online.</span></span> 

<span data-ttu-id="9e4ca-106">**Menyimpan daftar situs/template tombol ini tidak tersedia atau hilang**</span><span class="sxs-lookup"><span data-stu-id="9e4ca-106">**Save site/list template button is not available or missing**</span></span>

<span data-ttu-id="9e4ca-107">Administrator akan perlu untuk membolehkan Custom Script untuk mengaktifkan fitur template.</span><span class="sxs-lookup"><span data-stu-id="9e4ca-107">Administrators will need to Allow Custom Script to enable the template features.</span></span> <span data-ttu-id="9e4ca-108">Untuk langkah-langkah rinci contoh dan pertimbangan Lihat</span><span class="sxs-lookup"><span data-stu-id="9e4ca-108">For detailed steps, examples and considerations see</span></span> 

- [<span data-ttu-id="9e4ca-109">Membolehkan atau mencegah script kustom</span><span class="sxs-lookup"><span data-stu-id="9e4ca-109">Allow or prevent custom script</span></span>](https://docs.microsoft.com/sharepoint/allow-or-prevent-custom-script)

- <span data-ttu-id="9e4ca-110">Situs Simpan sebagai perintah template tidak didukung dan dapat menyebabkan masalah pada situs yang menggunakan SharePoint Server Publishing infrastruktur.</span><span class="sxs-lookup"><span data-stu-id="9e4ca-110">The Save site as template command is not supported and can cause problems on sites that use the SharePoint Server Publishing Infrastructure.</span></span>

<span data-ttu-id="9e4ca-111">Situs template tidak dapat dibuat atau tidak bekerja dengan benar.</span><span class="sxs-lookup"><span data-stu-id="9e4ca-111">The site template cannot be created or does not work correctly.</span></span>

<span data-ttu-id="9e4ca-112">Template mungkin hilang [fitur](https://social.technet.microsoft.com/wiki/contents/articles/14423.sharepoint-2013-existing-features-guid.aspx) dan tidak akan diaktifkan.</span><span class="sxs-lookup"><span data-stu-id="9e4ca-112">The template may be missing a [feature](https://social.technet.microsoft.com/wiki/contents/articles/14423.sharepoint-2013-existing-features-guid.aspx) and won't activate.</span></span> <span data-ttu-id="9e4ca-113">Jika fitur ini tidak tersedia untuk mengaktifkan dalam koleksi situs saat ini, Anda tidak dapat menggunakan situs template untuk membuat situs.</span><span class="sxs-lookup"><span data-stu-id="9e4ca-113">If the feature is not available to activate in the current site collection, you cannot use the site template to create a site.</span></span>

- <span data-ttu-id="9e4ca-114">Periksa untuk melihat jika atau daftar perpustakaan melebihi [Ambang batas daftar View](https://support.office.com/article/Manage-large-lists-and-libraries-in-SharePoint-B8588DAE-9387-48C2-9248-C24122F07C59) 5000 item seperti ini dapat menghalangi pembentukan situs template.</span><span class="sxs-lookup"><span data-stu-id="9e4ca-114">Check to see if any lists or libraries exceed the [List View Limit Threshold](https://support.office.com/article/Manage-large-lists-and-libraries-in-SharePoint-B8588DAE-9387-48C2-9248-C24122F07C59) of 5000 items as this can block creation of a site template.</span></span>

- <span data-ttu-id="9e4ca-115">Situs mungkin menggunakan terlalu banyak sumber daya dan karena itu situs template melebihi batas 50 MB.</span><span class="sxs-lookup"><span data-stu-id="9e4ca-115">The site may be using too many resources and therefore the site template exceeds the 50 MB limit.</span></span>


- <span data-ttu-id="9e4ca-116">Ada masalah yang menampilkan data dari daftar yang menggunakan kolom pencarian.</span><span class="sxs-lookup"><span data-stu-id="9e4ca-116">There are problems displaying data from a list that uses a lookup column.</span></span> <span data-ttu-id="9e4ca-117">Untuk informasi lebih lanjut, lihat [Daftar Template yang dihasilkan tidak menampilkan data dari daftar SharePoint Online benar lookup](https://support.office.com/article/template-generated-list-doesn-t-display-correct-data-for-a-column-in-sharepoint-online-20430b62-e40c-4f6f-8889-aa24e80d605a).</span><span class="sxs-lookup"><span data-stu-id="9e4ca-117">For more information, see [Template-generated list doesn't display data from the correct lookup list in SharePoint Online](https://support.office.com/article/template-generated-list-doesn-t-display-correct-data-for-a-column-in-sharepoint-online-20430b62-e40c-4f6f-8889-aa24e80d605a).</span></span>

<span data-ttu-id="9e4ca-118">Untuk informasi lebih rinci tentang umum masalah dan solusi, silahkan cek [membuat dan menggunakan situs template](https://support.office.com/article/Create-and-use-site-templates-60371B0F-00E0-4C49-A844-34759EBDD989).</span><span class="sxs-lookup"><span data-stu-id="9e4ca-118">For more detailed information on common problems and solutions, please check [Create and use site templates](https://support.office.com/article/Create-and-use-site-templates-60371B0F-00E0-4C49-A844-34759EBDD989).</span></span>



