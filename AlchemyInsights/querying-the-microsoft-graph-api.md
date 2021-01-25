---
title: Kueri API Microsoft graph
ms.author: v-jmathew
author: v-jmathew
manager: scotv
ms.audience: Admin
ms.topic: article
ms.service: o365-administration
ROBOTS: NOINDEX, NOFOLLOW
localization_priority: Normal
ms.collection: Adm_O365
ms.custom:
- "9004345"
- "7846"
ms.openlocfilehash: 527e88c7b3cb1cc4f5535e3b0d2bc4d8d1163336
ms.sourcegitcommit: 029c4697b77ce996d41ca74c4fa86de1bb84bd99
ms.translationtype: MT
ms.contentlocale: id-ID
ms.lasthandoff: 01/25/2021
ms.locfileid: "49974421"
---
# <a name="querying-the-microsoft-graph-api"></a><span data-ttu-id="0783d-102">Kueri API Microsoft graph</span><span class="sxs-lookup"><span data-stu-id="0783d-102">Querying the Microsoft Graph API</span></span>

<span data-ttu-id="0783d-103">Topik ini juga mungkin berlaku untuk pengembang masih menggunakan Azure AD graph API.</span><span class="sxs-lookup"><span data-stu-id="0783d-103">This topic may also apply to developers still using Azure AD Graph API.</span></span> <span data-ttu-id="0783d-104">Namun, **sangat disarankan agar** Anda menggunakan Microsoft graph untuk semua skenario manajemen direktori, identitas, dan akses Anda.</span><span class="sxs-lookup"><span data-stu-id="0783d-104">However, it is **strongly** recommended that you use Microsoft Graph for all your directory, identity, and access management scenarios.</span></span>

<span data-ttu-id="0783d-105">**Masalah autentikasi atau otorisasi**</span><span class="sxs-lookup"><span data-stu-id="0783d-105">**Authentication or authorization issues**</span></span>

- <span data-ttu-id="0783d-106">Jika aplikasi Anda **tidak dapat memperoleh token** untuk menghubungi Microsoft graph, pilih **masalah dengan mendapatkan kategori token Access (autentikasi)** Microsoft graph untuk mendapatkan bantuan dan dukungan yang lebih spesifik tentang topik ini.</span><span class="sxs-lookup"><span data-stu-id="0783d-106">If your app is **unable to acquire tokens** to call Microsoft Graph, pick **Problem with getting an access token (Authentication)** Microsoft Graph category to get more specific help and support on this topic.</span></span>
- <span data-ttu-id="0783d-107">Jika aplikasi Anda **menerima kesalahan otorisasi 401 atau 403** saat memanggil Microsoft graph, pilih kategori Dapatkan Microsoft graph **error (otorisasi) Access ditolak (Authorization)** untuk mendapatkan bantuan dan dukungan yang lebih spesifik tentang topik ini.</span><span class="sxs-lookup"><span data-stu-id="0783d-107">If your app is **receiving 401 or 403 authorization errors** when calling Microsoft Graph, pick the **Getting an access denied error (Authorization)** Microsoft Graph API category to get more specific help and support on this topic.</span></span>

<span data-ttu-id="0783d-108">**Saya ingin menggunakan Microsoft graph, tapi tidak yakin di mana memulai**</span><span class="sxs-lookup"><span data-stu-id="0783d-108">**I want to use Microsoft Graph, but not sure where to start**</span></span>

<span data-ttu-id="0783d-109">Untuk mempelajari selengkapnya tentang Microsoft graph, lihat:</span><span class="sxs-lookup"><span data-stu-id="0783d-109">To learn more about Microsoft Graph, see:</span></span>

- [<span data-ttu-id="0783d-110">Gambaran Umum Microsoft graph</span><span class="sxs-lookup"><span data-stu-id="0783d-110">Overview of Microsoft Graph</span></span>](https://docs.microsoft.com/graph/overview)
- [<span data-ttu-id="0783d-111">Gambaran umum manajemen identitas dan akses di Microsoft graph</span><span class="sxs-lookup"><span data-stu-id="0783d-111">Overview of Identity and Access Management in Microsoft Graph</span></span>](https://docs.microsoft.com/graph/azuread-identity-access-management-concept-overview)
- [<span data-ttu-id="0783d-112">Membuat aplikasi Microsoft graph yang mulai</span><span class="sxs-lookup"><span data-stu-id="0783d-112">Getting started building Microsoft Graph apps</span></span>](https://docs.microsoft.com/graph/)
- <span data-ttu-id="0783d-113">**Microsoft graph Explorer** -uji Microsoft graph api dalam penyewa atau penyewa demo Anda</span><span class="sxs-lookup"><span data-stu-id="0783d-113">**Microsoft Graph Explorer** - Test Microsoft Graph APIs in your tenant or a demo tenant</span></span>

<span data-ttu-id="0783d-114">**Saya ingin menggunakan Microsoft graph, tetapi apakah aplikasi ini mendukung api direktori v 1.0 yang diperlukan?**</span><span class="sxs-lookup"><span data-stu-id="0783d-114">**I want to use Microsoft Graph, but does it support the v1.0 directory APIs I need?**</span></span>

<span data-ttu-id="0783d-115">Microsoft graph adalah API yang direkomendasikan untuk direktori, identitas, dan manajemen akses.</span><span class="sxs-lookup"><span data-stu-id="0783d-115">Microsoft Graph is the recommended API for directory, identity, and access management.</span></span> <span data-ttu-id="0783d-116">Namun, masih ada beberapa celah di antara apa yang dimungkinkan di Azure AD graph dan Microsoft graph.</span><span class="sxs-lookup"><span data-stu-id="0783d-116">However, there are still a few gaps between what is possible in Azure AD Graph and Microsoft Graph.</span></span> <span data-ttu-id="0783d-117">Tinjau artikel berikut, yang menyoroti perbedaan paling terkini untuk membantu pilihan Anda:</span><span class="sxs-lookup"><span data-stu-id="0783d-117">Review the following articles, which highlight the most up-to-date differences to assist in your choice:</span></span>

- [<span data-ttu-id="0783d-118">Perbedaan tipe sumber daya antara grafik Azure AD dan Microsoft graph</span><span class="sxs-lookup"><span data-stu-id="0783d-118">Resource type differences between Azure AD Graph and Microsoft Graph</span></span>](https://docs.microsoft.com/graph/migrate-azure-ad-graph-resource-differences)
- [<span data-ttu-id="0783d-119">Perbedaan properti antara Azure AD graph dan Microsoft graph</span><span class="sxs-lookup"><span data-stu-id="0783d-119">Property differences between Azure AD Graph and Microsoft Graph</span></span>](https://docs.microsoft.com/graph/migrate-azure-ad-graph-property-differences)
- [<span data-ttu-id="0783d-120">Perbedaan metode antara Azure AD dan Microsoft graph</span><span class="sxs-lookup"><span data-stu-id="0783d-120">Method differences between Azure AD and Microsoft Graph</span></span>](https://docs.microsoft.com/graph/migrate-azure-ad-graph-method-differences)

<span data-ttu-id="0783d-121">**Saat saya meminta objek *pengguna* , banyak propertinya yang hilang**</span><span class="sxs-lookup"><span data-stu-id="0783d-121">**When I query the *user* object, many of its properties are missing**</span></span>

<span data-ttu-id="0783d-122">`GET https://graph.microsoft.com/v1.0/users` hanya mengembalikan 11 properti, karena Microsoft graph otomatis memilih sekumpulan properti *pengguna* default untuk dikembalikan.</span><span class="sxs-lookup"><span data-stu-id="0783d-122">`GET https://graph.microsoft.com/v1.0/users` only returns 11 properties, as Microsoft Graph auto-selects a default set of *user* properties to return.</span></span> <span data-ttu-id="0783d-123">Jika Anda memerlukan properti *pengguna* lain, gunakan $Select untuk memilih properti yang diperlukan aplikasi Anda.</span><span class="sxs-lookup"><span data-stu-id="0783d-123">If you need other *user* properties, use $select to pick the properties your application needs.</span></span> <span data-ttu-id="0783d-124">Cobalah di **Microsoft graph Explorer** terlebih dahulu.</span><span class="sxs-lookup"><span data-stu-id="0783d-124">Try it out in **Microsoft Graph Explorer** first.</span></span>

<span data-ttu-id="0783d-125">**Beberapa nilai properti pengguna *kosong* meskipun saya tahu bahwa mereka sudah siap**</span><span class="sxs-lookup"><span data-stu-id="0783d-125">**Some user property values are *null* even though I know they are set**</span></span>

<span data-ttu-id="0783d-126">Penjelasan yang paling mungkin adalah bahwa aplikasi telah diberikan *pengguna. ReadBasic. All* permission.</span><span class="sxs-lookup"><span data-stu-id="0783d-126">The most likely explanation is that the application had been granted the *User.ReadBasic.All* permission.</span></span> <span data-ttu-id="0783d-127">Hal ini memungkinkan aplikasi untuk membaca serangkaian properti pengguna, mengembalikan semua properti lain sebagai null meskipun telah ditetapkan sebelumnya.</span><span class="sxs-lookup"><span data-stu-id="0783d-127">This allows the application to read a limited set of user properties, returning all other properties as null even if they have been previously set.</span></span> <span data-ttu-id="0783d-128">Coba Berikan izin kepada *pengguna aplikasi. baca. All* .</span><span class="sxs-lookup"><span data-stu-id="0783d-128">Try granting the application *User.Read.All* permission instead.</span></span>

<span data-ttu-id="0783d-129">Untuk informasi selengkapnya, lihat [izin pengguna Microsoft graph](https://docs.microsoft.com/graph/permissions-reference#user-permissions).</span><span class="sxs-lookup"><span data-stu-id="0783d-129">For more information, see [Microsoft Graph user permissions](https://docs.microsoft.com/graph/permissions-reference#user-permissions).</span></span>

<span data-ttu-id="0783d-130">**Saya mengalami masalah dalam menggunakan parameter kueri OData untuk memfilter data dalam permintaan saya**</span><span class="sxs-lookup"><span data-stu-id="0783d-130">**I'm having trouble using OData query parameters to filter data in my requests**</span></span>

<span data-ttu-id="0783d-131">Sementara Microsoft graph mendukung berbagai parameter kueri OData, banyak parameter tersebut yang tidak sepenuhnya didukung oleh layanan direktori (sumber daya yang mewarisi dari *Directoryobject*) di Microsoft graph.</span><span class="sxs-lookup"><span data-stu-id="0783d-131">While Microsoft Graph supports a wide range of the OData query parameters, many of those parameters are not fully supported by directory services (resources that inherit from *directoryObject*) in Microsoft Graph.</span></span> <span data-ttu-id="0783d-132">Batasan yang sama yang ada di grafik Azure AD tetap ada untuk sebagian besar di Microsoft graph:</span><span class="sxs-lookup"><span data-stu-id="0783d-132">The same limitations that were present in Azure AD Graph persist for the most part in Microsoft Graph:</span></span>

1. <span data-ttu-id="0783d-133">**Tidak didukung**: $count, $Search, dan $filter nilai *null* atau *not null*</span><span class="sxs-lookup"><span data-stu-id="0783d-133">**Not supported**: $count, $search, and $filter on *null* or *not null* values</span></span>
2. <span data-ttu-id="0783d-134">**Tidak didukung**: $filter pada properti tertentu (lihat topik sumber daya properti yang dapat difilter)</span><span class="sxs-lookup"><span data-stu-id="0783d-134">**Not supported**: $filter on certain properties (see resource topics on which properties are filterable)</span></span>
3. <span data-ttu-id="0783d-135">**Tidak didukung**: paging, pemfilteran, dan pengurutan pada saat yang sama</span><span class="sxs-lookup"><span data-stu-id="0783d-135">**Not supported**: paging, filtering, and sorting at the same time</span></span>
4. <span data-ttu-id="0783d-136">**Tidak didukung**: pemfilteran pada hubungan.</span><span class="sxs-lookup"><span data-stu-id="0783d-136">**Not supported**: filtering on a relationship.</span></span> <span data-ttu-id="0783d-137">Misalnya-Temukan semua anggota grup teknik yang ada di Inggris.</span><span class="sxs-lookup"><span data-stu-id="0783d-137">For example - find all members of the engineering group that are in the UK.</span></span>
5. <span data-ttu-id="0783d-138">**Dukungan parsial**: $orderby pada *pengguna* (DisplayName dan userPrincipalName saja) dan *grup*</span><span class="sxs-lookup"><span data-stu-id="0783d-138">**Partial support**: $orderby on *user* (displayName and userPrincipalName only) and *group*</span></span>
6. <span data-ttu-id="0783d-139">**Dukungan parsial**: $filter (hanya mendukung dukungan *EQ*, *startswith*, *or*, *and*, dan terbatas *apa pun*), $Expand (memperluas hubungan satu objek mengembalikan semua hubungan, tapi memperluas kumpulan hubungan objek)</span><span class="sxs-lookup"><span data-stu-id="0783d-139">**Partial support**: $filter (supports only *eq*, *startswith*, *or*, *and*, and limited *any*) support, $expand (expanding a single object's relationships returns all relationships, but expanding a collection of objects' relationships is limited)</span></span>

<span data-ttu-id="0783d-140">Untuk informasi selengkapnya, lihat [mengkustomisasi respons dengan parameter kueri](https://docs.microsoft.com/graph/query-parameters).</span><span class="sxs-lookup"><span data-stu-id="0783d-140">For more information, see [Customize responses with query parameters](https://docs.microsoft.com/graph/query-parameters).</span></span>

<span data-ttu-id="0783d-141">**API yang saya panggil tidak berfungsi-di mana saya bisa melakukan lebih banyak pengujian?**</span><span class="sxs-lookup"><span data-stu-id="0783d-141">**The API I'm calling doesn't work - where can I do more testing?**</span></span>

<span data-ttu-id="0783d-142">**Microsoft graph Explorer** -uji Microsoft graph api di penyewa Anda atau penyewa demo dan juga lihat **kueri sampel** di Microsoft graph Explorer.</span><span class="sxs-lookup"><span data-stu-id="0783d-142">**Microsoft Graph Explorer** - Test Microsoft Graph APIs in your tenant or a demo tenant and also check out the **sample queries** in Microsoft Graph Explorer.</span></span>

<span data-ttu-id="0783d-143">**Saat saya meminta data sepertinya saya mendapatkan kumpulan data yang tidak lengkap kembali**</span><span class="sxs-lookup"><span data-stu-id="0783d-143">**When I query for data it seems like I get an incomplete data set back**</span></span>

<span data-ttu-id="0783d-144">Jika Anda membuat kueri kumpulan (seperti *pengguna*), Microsoft graph menggunakan batas halaman sisi server sehingga hasilnya selalu dikembalikan dengan ukuran halaman default.</span><span class="sxs-lookup"><span data-stu-id="0783d-144">If you are querying a collection (like *users*), Microsoft Graph uses server-side page limits so results are always returned with a default page-size.</span></span> <span data-ttu-id="0783d-145">Aplikasi Anda harus selalu menunggu untuk menelusuri kumpulan yang dikembalikan dari layanan.</span><span class="sxs-lookup"><span data-stu-id="0783d-145">Your app should always expect to page through collections returned from the service.</span></span>

<span data-ttu-id="0783d-146">Untuk informasi selengkapnya, lihat:</span><span class="sxs-lookup"><span data-stu-id="0783d-146">For more information, see:</span></span>

- [<span data-ttu-id="0783d-147">Praktik terbaik Microsoft graph</span><span class="sxs-lookup"><span data-stu-id="0783d-147">Microsoft Graph best practices</span></span>](https://docs.microsoft.com/graph/best-practices-concept)
- [<span data-ttu-id="0783d-148">Paging data Microsoft graph di aplikasi Anda</span><span class="sxs-lookup"><span data-stu-id="0783d-148">Paging Microsoft Graph data in your app</span></span>](https://docs.microsoft.com/graph/paging)

<span data-ttu-id="0783d-149">**Aplikasi saya terlalu lambat dan juga mengalami kelambatan. Penyempurnaan apa yang bisa saya lakukan?**</span><span class="sxs-lookup"><span data-stu-id="0783d-149">**My app is too slow and is also getting throttled. What improvements can I make?**</span></span>

<span data-ttu-id="0783d-150">Bergantung pada skenario Anda, ada berbagai opsi yang berbeda yang Anda inginkan untuk membuat aplikasi Anda lebih performant, dan dalam beberapa kasus, tidak rentan mengalami kelambatan oleh layanan (saat Anda membuat terlalu banyak panggilan).</span><span class="sxs-lookup"><span data-stu-id="0783d-150">Depending on your scenario, there are a variety of different options at your disposal to make your application more performant, and in some cases, less prone to being throttled by the service (when you are making too many calls).</span></span>

<span data-ttu-id="0783d-151">Untuk mempelajari selengkapnya, lihat:</span><span class="sxs-lookup"><span data-stu-id="0783d-151">To learn more, see:</span></span>

- [<span data-ttu-id="0783d-152">Praktik terbaik Microsoft graph</span><span class="sxs-lookup"><span data-stu-id="0783d-152">Microsoft Graph best practices</span></span>](https://docs.microsoft.com/graph/best-practices-concept)
- [<span data-ttu-id="0783d-153">Permintaan pengelompokan</span><span class="sxs-lookup"><span data-stu-id="0783d-153">Batching requests</span></span>](https://docs.microsoft.com/graph/json-batching)
- [<span data-ttu-id="0783d-154">Lacak perubahan melalui Delta query</span><span class="sxs-lookup"><span data-stu-id="0783d-154">Track changes through delta query</span></span>](https://docs.microsoft.com/graph/delta-query-overview)
- [<span data-ttu-id="0783d-155">Dapatkan pemberitahuan perubahan melalui webhooks</span><span class="sxs-lookup"><span data-stu-id="0783d-155">Get notified of changes through webhooks</span></span>](https://docs.microsoft.com/graph/webhooks)
- [<span data-ttu-id="0783d-156">Panduan pembatasan</span><span class="sxs-lookup"><span data-stu-id="0783d-156">Throttling guidance</span></span>](https://docs.microsoft.com/graph/throttling)

<span data-ttu-id="0783d-157">**Di mana saya bisa menemukan informasi selengkapnya tentang kesalahan dan masalah yang diketahui?**</span><span class="sxs-lookup"><span data-stu-id="0783d-157">**Where can I find more information on errors and known issues?**</span></span>

- [<span data-ttu-id="0783d-158">Informasi respons kesalahan Microsoft graph</span><span class="sxs-lookup"><span data-stu-id="0783d-158">Microsoft Graph error response information</span></span>](https://docs.microsoft.com/graph/errors)
- [<span data-ttu-id="0783d-159">Masalah yang diketahui dengan Microsoft graph</span><span class="sxs-lookup"><span data-stu-id="0783d-159">Known issues with Microsoft Graph</span></span>](https://docs.microsoft.com/graph/known-issues)

<span data-ttu-id="0783d-160">**Di mana saya dapat memeriksa status ketersediaan dan konektivitas Layanan?**</span><span class="sxs-lookup"><span data-stu-id="0783d-160">**Where can I check status of service availability and connectivity?**</span></span>

<span data-ttu-id="0783d-161">Ketersediaan layanan dan konektivitas layanan yang mendasari yang bisa diakses melalui Microsoft graph bisa berdampak pada ketersediaan dan kinerja keseluruhan Microsoft graph.</span><span class="sxs-lookup"><span data-stu-id="0783d-161">The service availability and connectivity of the underlying services that can be accessed through Microsoft Graph can impact the overall availability and performance of Microsoft Graph.</span></span>

- <span data-ttu-id="0783d-162">Untuk kesehatan layanan direktori aktif Azure, Periksa status layanan **identitas + keamanan** yang tercantum di [halaman status Azure](https://azure.microsoft.com/status/).</span><span class="sxs-lookup"><span data-stu-id="0783d-162">For Azure Active Directory service health, check the status of **Security + Identity** services listed in the [Azure status page](https://azure.microsoft.com/status/).</span></span>
- <span data-ttu-id="0783d-163">Untuk layanan Office yang berkontribusi ke Microsoft graph, Periksa status layanan yang tercantum di [dasbor Kesehatan Layanan Office](https://portal.office.com/adminportal/home#/servicehealth).</span><span class="sxs-lookup"><span data-stu-id="0783d-163">For Office services that contribute to Microsoft Graph, check the status of services listed in the [Office Service Health Dashboard](https://portal.office.com/adminportal/home#/servicehealth).</span></span>
