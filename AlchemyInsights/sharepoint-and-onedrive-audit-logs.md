---
title: Laporan log audit SharePoint klasik
ms.author: chrisda
author: chrisda
manager: dansimp
ms.date: 04/21/2020
ms.audience: ITPro
ms.topic: article
ms.service: o365-administration
ROBOTS: NOINDEX, NOFOLLOW
localization_priority: Normal
ms.custom:
- "1372"
- "3100005"
ms.assetid: ''
ms.openlocfilehash: daf79f8d75ccdff8ad54f0f307648a5832a6bb71
ms.sourcegitcommit: c6692ce0fa1358ec3529e59ca0ecdfdea4cdc759
ms.translationtype: MT
ms.contentlocale: id-ID
ms.lasthandoff: 09/14/2020
ms.locfileid: "47662211"
---
# <a name="sharepoint-and-onedrive-audit-logs"></a><span data-ttu-id="bd4fc-102">Log audit SharePoint dan OneDrive</span><span class="sxs-lookup"><span data-stu-id="bd4fc-102">SharePoint and OneDrive audit logs</span></span>

## <a name="sharepoint-classic-audit-logs"></a><span data-ttu-id="bd4fc-103">Log audit klasik SharePoint</span><span class="sxs-lookup"><span data-stu-id="bd4fc-103">SharePoint classic Audit logs</span></span>

<span data-ttu-id="bd4fc-104">Audit warisan SPO dimigrasikan ke log audit terpadu (UAL).</span><span class="sxs-lookup"><span data-stu-id="bd4fc-104">SPO legacy auditing was migrated to Unified Audit Log (UAL).</span></span> <span data-ttu-id="bd4fc-105">Semua Laporan Audit warisan SPO kini akan didukung melalui UAL, dan sinyal audit warisan telah dimigrasikan ke UAL.</span><span class="sxs-lookup"><span data-stu-id="bd4fc-105">All SPO legacy audit reports will now be powered through UAL, and the legacy audit signals have been migrated to UAL.</span></span>

<span data-ttu-id="bd4fc-106">Perubahan tombol:</span><span class="sxs-lookup"><span data-stu-id="bd4fc-106">Key changes:</span></span>

* <span data-ttu-id="bd4fc-107">Pemangkasan tidak tersedia sebagai kapabilitas.</span><span class="sxs-lookup"><span data-stu-id="bd4fc-107">Trimming is NOT available as a capability.</span></span>
* <span data-ttu-id="bd4fc-108">Memilih acara tertentu untuk diaudit tidak tersedia.</span><span class="sxs-lookup"><span data-stu-id="bd4fc-108">Choosing specific events to audit is NOT available.</span></span> <span data-ttu-id="bd4fc-109">Rujuk ke [dokumen ini](https://docs.microsoft.com/microsoft-365/compliance/search-the-audit-log-in-security-and-compliance) untuk daftar lengkap acara yang diaudit yang tersedia secara default.</span><span class="sxs-lookup"><span data-stu-id="bd4fc-109">Refer to [this document](https://docs.microsoft.com/microsoft-365/compliance/search-the-audit-log-in-security-and-compliance) for a complete list of audited events available by default.</span></span>
* <span data-ttu-id="bd4fc-110">Opsi **Lokasi** di bawah **laporan yang dikustomisasi** tidak tersedia.</span><span class="sxs-lookup"><span data-stu-id="bd4fc-110">The **Location** option under **Customized reports** is NOT available.</span></span>
* <span data-ttu-id="bd4fc-111">Opsi acara **membuka atau mengunduh dokumen** tidak tersedia.</span><span class="sxs-lookup"><span data-stu-id="bd4fc-111">The **Opening or downloading documents** events option is NOT available.</span></span>

[<span data-ttu-id="bd4fc-112">Mengonfigurasi pengaturan audit untuk kumpulan situs</span><span class="sxs-lookup"><span data-stu-id="bd4fc-112">Configure Audit settings for a site collection</span></span>](https://support.office.com/article/Configure-audit-settings-for-a-site-collection-A9920C97-38C0-44F2-8BCB-4CF1E2AE22D2)

## <a name="sharepoint-and-onedrive-modern-unified-audit-logs-from-compliance"></a><span data-ttu-id="bd4fc-113">SharePoint dan OneDrive modern Unified log audit dari kepatuhan</span><span class="sxs-lookup"><span data-stu-id="bd4fc-113">SharePoint and OneDrive Modern Unified Audit logs from compliance</span></span>

* [<span data-ttu-id="bd4fc-114">Mengaktifkan/menonaktifkan pembuatan log audit terpadu</span><span class="sxs-lookup"><span data-stu-id="bd4fc-114">Turn on/off Unified Audit Logging</span></span>](https://docs.microsoft.com/microsoft-365/compliance/turn-audit-log-search-on-or-off) 

<span data-ttu-id="bd4fc-115">Tidak diperlukan konfigurasi tambahan dalam SharePoint atau OneDrive.</span><span class="sxs-lookup"><span data-stu-id="bd4fc-115">No additional configuration is required within SharePoint or OneDrive.</span></span>

<span data-ttu-id="bd4fc-116">Menggunakan pencarian pembuatan log audit untuk memeriksa aktivitas file, folder, pengguna, izin:</span><span class="sxs-lookup"><span data-stu-id="bd4fc-116">Use audit logging search to check activity of the file(s), folder(s), user(s), permissions:</span></span>

* [<span data-ttu-id="bd4fc-117">Aktivitas file dan halaman</span><span class="sxs-lookup"><span data-stu-id="bd4fc-117">File and page activities</span></span>](https://docs.microsoft.com/microsoft-365/compliance/search-the-audit-log-in-security-and-compliance)
* [<span data-ttu-id="bd4fc-118">Aktivitas folder</span><span class="sxs-lookup"><span data-stu-id="bd4fc-118">Folder activities</span></span>](https://docs.microsoft.com/microsoft-365/compliance/search-the-audit-log-in-security-and-compliance#folder-activities)
* [<span data-ttu-id="bd4fc-119">Aktivitas permintaan akses dan berbagi</span><span class="sxs-lookup"><span data-stu-id="bd4fc-119">Sharing and access request activities</span></span>](https://docs.microsoft.com/microsoft-365/compliance/search-the-audit-log-in-security-and-compliance#sharing-and-access-request-activities)
* [<span data-ttu-id="bd4fc-120">Aktivitas sinkronisasi</span><span class="sxs-lookup"><span data-stu-id="bd4fc-120">Synchronization activities</span></span>](https://docs.microsoft.com/microsoft-365/compliance/search-the-audit-log-in-security-and-compliance#synchronization-activities)
* [<span data-ttu-id="bd4fc-121">Aktivitas administrasi situs</span><span class="sxs-lookup"><span data-stu-id="bd4fc-121">Site administration activities</span></span>](https://docs.microsoft.com/microsoft-365/compliance/search-the-audit-log-in-security-and-compliance#site-administration-activities)

<span data-ttu-id="bd4fc-122">Untuk informasi selengkapnya tentang cara mendapatkan kembali acara ini, lihat [mencari log audit](https://docs.microsoft.com/microsoft-365/compliance/search-the-audit-log-in-security-and-compliance#search-the-audit-log).</span><span class="sxs-lookup"><span data-stu-id="bd4fc-122">For more information about how to retrieve these events, see [Search the audit log](https://docs.microsoft.com/microsoft-365/compliance/search-the-audit-log-in-security-and-compliance#search-the-audit-log).</span></span>
