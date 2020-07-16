---
title: Masalah membuka atau men-download file di heboh
ms.author: pebaum
author: pebaum
manager: scotv
ms.date: 07/15/2020
ms.audience: Admin
ms.topic: article
ROBOTS: NOINDEX, NOFOLLOW
localization_priority: Priority
ms.collection: Adm_O365
ms.custom:
- "6041"
- "9003112"
ms.openlocfilehash: 6dfcbe9abfc23219a61e81785d31c11f7a0fa95c
ms.sourcegitcommit: b677b85395b7244b2bf2b753468b696b4cf27c8d
ms.translationtype: MT
ms.contentlocale: id-ID
ms.lasthandoff: 07/16/2020
ms.locfileid: "45148332"
---
# <a name="issue-opening-or-downloading-files-in-yammer"></a><span data-ttu-id="18200-102">Masalah membuka atau men-download file di heboh</span><span class="sxs-lookup"><span data-stu-id="18200-102">Issue opening or downloading files in Yammer</span></span>

<span data-ttu-id="18200-103">Klasik heboh mendukung beberapa pilihan untuk file upload ke pesan dan kelompok.</span><span class="sxs-lookup"><span data-stu-id="18200-103">Classic Yammer supports multiple option for file uploads to messages and groups.</span></span> <span data-ttu-id="18200-104">Tergantung pada konfigurasi jaringan, file default ke penyimpanan di SharePoint.</span><span class="sxs-lookup"><span data-stu-id="18200-104">Depending on network configuration, files default to storage in SharePoint.</span></span>

<span data-ttu-id="18200-105">Pemilih file di heboh baru belum mendukung semua pilihan yang tersedia dalam klasik heboh.</span><span class="sxs-lookup"><span data-stu-id="18200-105">The file picker in new Yammer does not yet support all the options available in classic Yammer.</span></span> <span data-ttu-id="18200-106">Pembaruan berikutnya akan menambahkan fitur tambahan.</span><span class="sxs-lookup"><span data-stu-id="18200-106">A future update will add additional features.</span></span> <span data-ttu-id="18200-107">Untuk informasi lebih lanjut, lihat [melampirkan file atau gambar ke posting percakapan heboh](https://support.microsoft.com/office/attach-a-file-or-image-to-a-yammer-conversation-post-8d2d17f7-8f37-4535-961e-518d751be7e8).</span><span class="sxs-lookup"><span data-stu-id="18200-107">For more info, see [Attach a file or image to a Yammer conversation post](https://support.microsoft.com/office/attach-a-file-or-image-to-a-yammer-conversation-post-8d2d17f7-8f37-4535-961e-518d751be7e8).</span></span>

<span data-ttu-id="18200-108">**Tidak dapat membuka atau mengunduh berkas**</span><span class="sxs-lookup"><span data-stu-id="18200-108">**Unable to open or download a file**</span></span>  

<span data-ttu-id="18200-109">Berkas yang mungkin meng-upload ke Yammer tetapi juga dapat menghubungkan ke berkas di SharePoint online.</span><span class="sxs-lookup"><span data-stu-id="18200-109">A file might upload to Yammer but also be linking to a file in SharePoint Online.</span></span> <span data-ttu-id="18200-110">Untuk memecahkan masalah, pertama-tama Anda harus menentukan lokasi berkas.</span><span class="sxs-lookup"><span data-stu-id="18200-110">To troubleshoot, first you must determine the location of the file.</span></span> <span data-ttu-id="18200-111">Jika file telah diunggah ke heboh, itu akan memiliki URL \*. yammer.com.</span><span class="sxs-lookup"><span data-stu-id="18200-111">If the file has been uploaded to Yammer, it will have a \*.yammer.com URL.</span></span> <span data-ttu-id="18200-112">Pastikan URL dan alamat IP yang diperlukan tidak diblokir.</span><span class="sxs-lookup"><span data-stu-id="18200-112">Ensure that required URLs and IP addresses are unblocked.</span></span> <span data-ttu-id="18200-113">Untuk informasi lebih lanjut, lihat posting blog [menggunakan alamat IP keras kode untuk heboh tidak dianjurkan](https://techcommunity.microsoft.com/t5/yammer-blog/using-hard-coded-ip-addresses-for-yammer-is-not-recommended/ba-p/276592).</span><span class="sxs-lookup"><span data-stu-id="18200-113">For more info, see the blog post [Using hard coded IP addresses for Yammer is not recommended](https://techcommunity.microsoft.com/t5/yammer-blog/using-hard-coded-ip-addresses-for-yammer-is-not-recommended/ba-p/276592).</span></span>

<span data-ttu-id="18200-114">Periksa apakah pengguna yang juga admin global dapat men-download file.</span><span class="sxs-lookup"><span data-stu-id="18200-114">Check whether a user who is also a global admin can download the file.</span></span> <span data-ttu-id="18200-115">Jika file bersifat pribadi, Anda mungkin harus menggunakan mode konten pribadi.</span><span class="sxs-lookup"><span data-stu-id="18200-115">If the file is private, you might have to use Private Content Mode.</span></span> <span data-ttu-id="18200-116">Untuk informasi lebih lanjut, lihat kemudian [memantau konten pribadi di heboh](https://docs.microsoft.com/yammer/manage-security-and-compliance/monitor-private-content).</span><span class="sxs-lookup"><span data-stu-id="18200-116">For more info, see then [Monitor private content in Yammer](https://docs.microsoft.com/yammer/manage-security-and-compliance/monitor-private-content).</span></span>  

<span data-ttu-id="18200-117">**Heboh tingkat jaringan tamu dan file dalam SharePoint online**</span><span class="sxs-lookup"><span data-stu-id="18200-117">**Yammer network-level guests and files in SharePoint Online**</span></span>  

<span data-ttu-id="18200-118">[Tingkat jaringan tamu di heboh](https://docs.microsoft.com/yammer/manage-yammer-users/add-block-or-remove-users#invite-guests) tidak menggunakan AZURE AD B2B dan internal untuk layanan heboh, sehingga mereka tidak dapat mengakses file heboh disimpan di SharePoint.</span><span class="sxs-lookup"><span data-stu-id="18200-118">[Network-level guests in Yammer](https://docs.microsoft.com/yammer/manage-yammer-users/add-block-or-remove-users#invite-guests) do not use Azure AD B2B and are internal to the Yammer service, so they can't access Yammer files stored in SharePoint.</span></span> <span data-ttu-id="18200-119">Membuat eksternal AAD B2B pengguna yang dapat mengakses perpustakaan dokumen di SharePoint online dengan menggunakan identitas tersebut.</span><span class="sxs-lookup"><span data-stu-id="18200-119">Create an external AAD B2B user who can access document libraries in SharePoint Online by using that identity.</span></span> <span data-ttu-id="18200-120">Untuk informasi tentang masa depan Azure AD B2B dukungan tamu di Yammer, lihat [dukungan tamu Business-to-Business (B2B) di Yammer pratinjau-persyaratan pelanggan dan FAQ](https://docs.microsoft.com/yammer/get-started-with-yammer/azure-ad-b2b-guests-yammer).</span><span class="sxs-lookup"><span data-stu-id="18200-120">For information about future Azure AD B2B guest support in Yammer, see [Business-to-business (B2B) Guest support in Yammer Preview - Customer Terms and FAQ](https://docs.microsoft.com/yammer/get-started-with-yammer/azure-ad-b2b-guests-yammer).</span></span>