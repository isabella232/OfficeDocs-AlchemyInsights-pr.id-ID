---
title: Membuat Hubungan Organisasi agar pengguna Anda dapat berkolaborasi dengan organisasi lain
ms.author: pebaum
author: pebaum
manager: scotv
ms.audience: Admin
ms.topic: article
ms.service: o365-administration
ROBOTS: NOINDEX, NOFOLLOW
localization_priority: Priority
ms.collection: Adm_O365
ms.custom:
- "3800014"
- "898"
ms.openlocfilehash: b595fb87e18a055a7df1ff4c782a93591dd1f024
ms.sourcegitcommit: 8bc60ec34bc1e40685e3976576e04a2623f63a7c
ms.translationtype: MT
ms.contentlocale: id-ID
ms.lasthandoff: 04/15/2021
ms.locfileid: "51816131"
---
# <a name="create-an-organization-relationship-to-allow-your-users-to-collaborate-with-another-organization"></a><span data-ttu-id="1d5bf-102">Membuat Hubungan Organisasi agar pengguna Anda dapat berkolaborasi dengan organisasi lain</span><span class="sxs-lookup"><span data-stu-id="1d5bf-102">Create an Organization Relationship to allow your users to collaborate with another organization</span></span>

1. <span data-ttu-id="1d5bf-103">Dari dasbor pusat admin Microsoft 365, buka **Admin** > **Exchange**.</span><span class="sxs-lookup"><span data-stu-id="1d5bf-103">From the Microsoft 365 admin center dashboard, go to **Admin** > **Exchange**.</span></span>
2. <span data-ttu-id="1d5bf-104">Buka **berbagi** > **organisasi**.</span><span class="sxs-lookup"><span data-stu-id="1d5bf-104">Go to **organization** > **sharing**.</span></span>
3. <span data-ttu-id="1d5bf-105">Di **Berbagi Organisasi**, klik **Baru** .</span><span class="sxs-lookup"><span data-stu-id="1d5bf-105">Under **Organization Sharing**, click **New** .</span></span>
4. <span data-ttu-id="1d5bf-106">Di **hubungan organisasi baru**, di dalam kotak **Nama hubungan**, ketikkan nama yang mudah dikenali untuk hubungan organisasi.</span><span class="sxs-lookup"><span data-stu-id="1d5bf-106">In **new organization relationship**, in the **Relationship name** box, type a friendly name for the organization relationship.</span></span>
5. <span data-ttu-id="1d5bf-107">Dalam kotak **Domain yang akan dibagikan**, ketikkan domain untuk Office 365 eksternal atau organisasi lokal Exchange yang Ingin Anda lihat kalendernya.</span><span class="sxs-lookup"><span data-stu-id="1d5bf-107">In the **Domains to share with** box, type the domain for the external Office 365 or Exchange on-premises organization you want to let see your calendars.</span></span> <span data-ttu-id="1d5bf-108">Jika Anda perlu memasukkan lebih dari satu domain, pisahkan nama domain dengan koma.</span><span class="sxs-lookup"><span data-stu-id="1d5bf-108">If you need to enter more than one domain, separate the domain names with a comma.</span></span> <span data-ttu-id="1d5bf-109">Misalnya, contoso.com, service.contoso.com.</span><span class="sxs-lookup"><span data-stu-id="1d5bf-109">For example, contoso.com, service.contoso.com.</span></span>
6. <span data-ttu-id="1d5bf-110">Centang kotak **Aktifkan berbagi informasi bebas/sibuk kalender** untuk mengaktifkan berbagi kalender dengan domain yang Anda daftarkan.</span><span class="sxs-lookup"><span data-stu-id="1d5bf-110">Select the **Enable calendar free/busy information sharing** check box to turn on calendar sharing with the domains you listed.</span></span> <span data-ttu-id="1d5bf-111">Tetapkan tingkat berbagi informasi bebas/sibuk kalender dan tetapkan pengguna mana yang dapat berbagi informasi bebas/sibuk kalender.</span><span class="sxs-lookup"><span data-stu-id="1d5bf-111">Set the sharing level for calendar free/busy information and set which users can share calendar free/busy information.</span></span>  

<span data-ttu-id="1d5bf-112">Untuk menetapkan tingkat akses bebas/sibuk, pilih salah satu hal berikut ini:</span><span class="sxs-lookup"><span data-stu-id="1d5bf-112">To set the free/busy access level, select one of the following:</span></span>

- <span data-ttu-id="1d5bf-113">**Informasi bebas/sibuk kalender yang dilengkapi dengan waktu saja**</span><span class="sxs-lookup"><span data-stu-id="1d5bf-113">**Calendar free/busy information with time only**</span></span>
- <span data-ttu-id="1d5bf-114">**Kalender informasi bebas/sibuk yang dilengkapi dengan waktu, subjek, dan lokasi**</span><span class="sxs-lookup"><span data-stu-id="1d5bf-114">**Calendar free/busy with time, subject, and location**</span></span>  

 <span data-ttu-id="1d5bf-115">Untuk menetapkan pengguna yang akan berbagi informasi bebas/sibuk kalender, pilih salah satu hal berikut ini:</span><span class="sxs-lookup"><span data-stu-id="1d5bf-115">To set which users will share calendar free/busy information, select one of the following:</span></span>

- <span data-ttu-id="1d5bf-116">**Orang-orang di organisasi Anda**</span><span class="sxs-lookup"><span data-stu-id="1d5bf-116">**Everyone in your organization**</span></span>
- <span data-ttu-id="1d5bf-117">**Grup keamanan tertentu**</span><span class="sxs-lookup"><span data-stu-id="1d5bf-117">**A specified security group**</span></span>  

<span data-ttu-id="1d5bf-118">Klik **telusuri** untuk memilih grup keamanan dari daftar, lalu klik **ok**.</span><span class="sxs-lookup"><span data-stu-id="1d5bf-118">Click **browse** to pick the security group from a list, then click **ok**.</span></span>

<span data-ttu-id="1d5bf-119">Klik **simpan** untuk membuat hubungan organisasi.</span><span class="sxs-lookup"><span data-stu-id="1d5bf-119">Click **save** to create the organization relationship.</span></span>  

<span data-ttu-id="1d5bf-120">**Catatan:** Konfigurasi lintas penyewa tidak mendukung kontak pribadi untuk pencarian bebas/sibuk.</span><span class="sxs-lookup"><span data-stu-id="1d5bf-120">**Note:** Cross-tenant configurations do not support personal contacts for free/busy lookup.</span></span> <span data-ttu-id="1d5bf-121">Kontak harus disertakan dalam daftar alamat global agar pencarian bebas/sibuk dapat berfungsi.</span><span class="sxs-lookup"><span data-stu-id="1d5bf-121">Contacts must be included in the global address list for free/busy lookup to work.</span></span>

<span data-ttu-id="1d5bf-122">**Untuk pemahaman menyeluruh tentang topik ini, silakan baca:**</span><span class="sxs-lookup"><span data-stu-id="1d5bf-122">**For full understanding of this topic please read:**</span></span>

- [<span data-ttu-id="1d5bf-123">Membuat hubungan organisasi di Exchange Online</span><span class="sxs-lookup"><span data-stu-id="1d5bf-123">Create an organization relationship in Exchange Online</span></span>](https://docs.microsoft.com/exchange/sharing/organization-relationships/create-an-organization-relationship)
- [<span data-ttu-id="1d5bf-124">Mengubah hubungan organisasi di Exchange Online</span><span class="sxs-lookup"><span data-stu-id="1d5bf-124">Modify an organization relationship in Exchange Online</span></span>](https://docs.microsoft.com/exchange/sharing/organization-relationships/modify-an-organization-relationship)
- [<span data-ttu-id="1d5bf-125">Menghapus hubungan organisasi di Exchange Online</span><span class="sxs-lookup"><span data-stu-id="1d5bf-125">Remove an organization relationship in Exchange Online</span></span>](https://docs.microsoft.com/exchange/sharing/organization-relationships/remove-an-organization-relationship)
