---
title: Laporan log audit SharePoint klasik
ms.author: chrisda
author: chrisda
manager: dansimp
ms.date: 04/21/2020
ms.audience: ITPro
ms.topic: article
ROBOTS: NOINDEX, NOFOLLOW
localization_priority: Normal
ms.custom:
- "1372"
- "3100005"
ms.assetid: ''
ms.openlocfilehash: 0aedb549f11db54d3cd480671fb0767c60680ad3
ms.sourcegitcommit: bc7d6f4f3c9f7060d073f5130e1ec856e248d020
ms.translationtype: MT
ms.contentlocale: id-ID
ms.lasthandoff: 06/02/2020
ms.locfileid: "44509603"
---
# <a name="sharepoint-and-onedrive-audit-logs"></a><span data-ttu-id="0e4ea-102">Log audit SharePoint dan OneDrive</span><span class="sxs-lookup"><span data-stu-id="0e4ea-102">SharePoint and OneDrive audit logs</span></span>

## <a name="sharepoint-classic-audit-logs"></a><span data-ttu-id="0e4ea-103">Log audit klasik SharePoint</span><span class="sxs-lookup"><span data-stu-id="0e4ea-103">SharePoint classic Audit logs</span></span>

<span data-ttu-id="0e4ea-104">SPO warisan audit bermigrasi ke log audit terpadu (UAL).</span><span class="sxs-lookup"><span data-stu-id="0e4ea-104">SPO legacy auditing was migrated to Unified Audit Log (UAL).</span></span> <span data-ttu-id="0e4ea-105">Semua Laporan Audit warisan SPO sekarang akan didukung melalui UAL, dan sinyal audit warisan telah dipindahkan ke UAL.</span><span class="sxs-lookup"><span data-stu-id="0e4ea-105">All SPO legacy audit reports will now be powered through UAL, and the legacy audit signals have been migrated to UAL.</span></span>

<span data-ttu-id="0e4ea-106">Perubahan utama:</span><span class="sxs-lookup"><span data-stu-id="0e4ea-106">Key changes:</span></span>

* <span data-ttu-id="0e4ea-107">Pemangkasan ini tidak tersedia sebagai kemampuan.</span><span class="sxs-lookup"><span data-stu-id="0e4ea-107">Trimming is NOT available as a capability.</span></span>
* <span data-ttu-id="0e4ea-108">Memilih peristiwa tertentu untuk mengaudit tidak tersedia.</span><span class="sxs-lookup"><span data-stu-id="0e4ea-108">Choosing specific events to audit is NOT available.</span></span> <span data-ttu-id="0e4ea-109">Lihat [dokumen ini](https://docs.microsoft.com/microsoft-365/compliance/search-the-audit-log-in-security-and-compliance) untuk daftar lengkap dari peristiwa yang diaudit yang tersedia secara default.</span><span class="sxs-lookup"><span data-stu-id="0e4ea-109">Refer to [this document](https://docs.microsoft.com/microsoft-365/compliance/search-the-audit-log-in-security-and-compliance) for a complete list of audited events available by default.</span></span>
* <span data-ttu-id="0e4ea-110">Opsi **Lokasi** di bawah **laporan kustom** tidak tersedia.</span><span class="sxs-lookup"><span data-stu-id="0e4ea-110">The **Location** option under **Customized reports** is NOT available.</span></span>
* <span data-ttu-id="0e4ea-111">**Membuka atau men-download dokumen** peristiwa opsi ini tidak tersedia.</span><span class="sxs-lookup"><span data-stu-id="0e4ea-111">The **Opening or downloading documents** events option is NOT available.</span></span>

[<span data-ttu-id="0e4ea-112">Mengkonfigurasi pengaturan audit untuk koleksi situs</span><span class="sxs-lookup"><span data-stu-id="0e4ea-112">Configure Audit settings for a site collection</span></span>](https://support.office.com/article/Configure-audit-settings-for-a-site-collection-A9920C97-38C0-44F2-8BCB-4CF1E2AE22D2)

## <a name="sharepoint-and-onedrive-modern-unified-audit-logs-from-compliance"></a><span data-ttu-id="0e4ea-113">SharePoint dan OneDrive modern terpadu audit log dari kepatuhan</span><span class="sxs-lookup"><span data-stu-id="0e4ea-113">SharePoint and OneDrive Modern Unified Audit logs from compliance</span></span>

* [<span data-ttu-id="0e4ea-114">Mengaktifkan/menonaktifkan pencatatan audit terpadu</span><span class="sxs-lookup"><span data-stu-id="0e4ea-114">Turn on/off Unified Audit Logging</span></span>](https://docs.microsoft.com/microsoft-365/compliance/turn-audit-log-search-on-or-off) 

<span data-ttu-id="0e4ea-115">Tidak ada konfigurasi tambahan yang diperlukan dalam SharePoint atau OneDrive.</span><span class="sxs-lookup"><span data-stu-id="0e4ea-115">No additional configuration is required within SharePoint or OneDrive.</span></span>

<span data-ttu-id="0e4ea-116">Menggunakan pencarian pengelogan audit untuk memeriksa aktivitas file, folder (s), pengguna, izin:</span><span class="sxs-lookup"><span data-stu-id="0e4ea-116">Use audit logging search to check activity of the file(s), folder(s), user(s), permissions:</span></span>

* [<span data-ttu-id="0e4ea-117">Aktivitas file dan halaman</span><span class="sxs-lookup"><span data-stu-id="0e4ea-117">File and page activities</span></span>](https://docs.microsoft.com/microsoft-365/compliance/search-the-audit-log-in-security-and-compliance)
* [<span data-ttu-id="0e4ea-118">Aktivitas folder</span><span class="sxs-lookup"><span data-stu-id="0e4ea-118">Folder activities</span></span>](https://docs.microsoft.com/microsoft-365/compliance/search-the-audit-log-in-security-and-compliance#folder-activities)
* [<span data-ttu-id="0e4ea-119">Berbagi dan mengakses aktivitas permintaan</span><span class="sxs-lookup"><span data-stu-id="0e4ea-119">Sharing and access request activities</span></span>](https://docs.microsoft.com/microsoft-365/compliance/search-the-audit-log-in-security-and-compliance#sharing-and-access-request-activities)
* [<span data-ttu-id="0e4ea-120">Aktivitas sinkronisasi</span><span class="sxs-lookup"><span data-stu-id="0e4ea-120">Synchronization activities</span></span>](https://docs.microsoft.com/microsoft-365/compliance/search-the-audit-log-in-security-and-compliance#synchronization-activities)
* [<span data-ttu-id="0e4ea-121">Kegiatan administrasi situs</span><span class="sxs-lookup"><span data-stu-id="0e4ea-121">Site administration activities</span></span>](https://docs.microsoft.com/microsoft-365/compliance/search-the-audit-log-in-security-and-compliance#site-administration-activities)

<span data-ttu-id="0e4ea-122">Untuk informasi selengkapnya tentang cara mengambil peristiwa ini, lihat [pencarian audit log](https://docs.microsoft.com/microsoft-365/compliance/search-the-audit-log-in-security-and-compliance#search-the-audit-log).</span><span class="sxs-lookup"><span data-stu-id="0e4ea-122">For more information about how to retrieve these events, see [Search the audit log](https://docs.microsoft.com/microsoft-365/compliance/search-the-audit-log-in-security-and-compliance#search-the-audit-log).</span></span>
