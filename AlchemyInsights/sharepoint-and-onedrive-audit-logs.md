---
title: Laporan log audit SharePoint klasik
ms.author: chrisda
author: chrisda
manager: dansimp
ms.date: ''
ms.audience: ITPro
ms.topic: article
ROBOTS: NOINDEX, NOFOLLOW
localization_priority: Normal
ms.custom:
- "1372"
- "3100005"
ms.assetid: ''
ms.openlocfilehash: af5b3c76b82db13bc89c917247e41fa1d8779b68
ms.sourcegitcommit: d5bf97a0bf0547f36b6da9684ce9f16a13a7749e
ms.translationtype: MT
ms.contentlocale: id-ID
ms.lasthandoff: 09/20/2019
ms.locfileid: "37068026"
---
# <a name="sharepoint-and-onedrive-audit-logs"></a><span data-ttu-id="8dd4c-102">Log audit SharePoint dan OneDrive</span><span class="sxs-lookup"><span data-stu-id="8dd4c-102">SharePoint and OneDrive audit logs</span></span>

<span data-ttu-id="8dd4c-103">**SharePoint dan OneDrive modern terpadu audit log dari kepatuhan**</span><span class="sxs-lookup"><span data-stu-id="8dd4c-103">**SharePoint and OneDrive Modern Unified Audit logs from compliance**</span></span>

- [<span data-ttu-id="8dd4c-104">Mengaktifkan/menonaktifkan pencatatan audit terpadu</span><span class="sxs-lookup"><span data-stu-id="8dd4c-104">Turn on/off Unified Audit Logging</span></span>](https://docs.microsoft.com/office365/securitycompliance/turn-audit-log-search-on-or-off) 

<span data-ttu-id="8dd4c-105">Tidak ada konfigurasi tambahan yang diperlukan dalam SharePoint atau OneDrive.</span><span class="sxs-lookup"><span data-stu-id="8dd4c-105">No additional configuration is required within SharePoint or OneDrive.</span></span>

- <span data-ttu-id="8dd4c-106">Menggunakan pencarian pengelogan audit untuk memeriksa aktivitas file, folder (s), pengguna, izin:</span><span class="sxs-lookup"><span data-stu-id="8dd4c-106">Use audit logging search to check activity of the file(s), folder(s), user(s), permissions:</span></span>

    - [<span data-ttu-id="8dd4c-107">Aktivitas file dan halaman</span><span class="sxs-lookup"><span data-stu-id="8dd4c-107">File and page activities</span></span>](https://docs.microsoft.com/office365/securitycompliance/search-the-audit-log-in-security-and-compliance)
    - [<span data-ttu-id="8dd4c-108">Aktivitas folder</span><span class="sxs-lookup"><span data-stu-id="8dd4c-108">Folder activities</span></span>](https://docs.microsoft.com/office365/securitycompliance/search-the-audit-log-in-security-and-compliance#folder-activities)
    - [<span data-ttu-id="8dd4c-109">Berbagi dan mengakses aktivitas permintaan</span><span class="sxs-lookup"><span data-stu-id="8dd4c-109">Sharing and access request activities</span></span>](https://docs.microsoft.com/office365/securitycompliance/search-the-audit-log-in-security-and-compliance#sharing-and-access-request-activities)
    - [<span data-ttu-id="8dd4c-110">Aktivitas sinkronisasi</span><span class="sxs-lookup"><span data-stu-id="8dd4c-110">Synchronization activities</span></span>](https://docs.microsoft.com/office365/securitycompliance/search-the-audit-log-in-security-and-compliance#synchronization-activities)
    - [<span data-ttu-id="8dd4c-111">Kegiatan administrasi situs</span><span class="sxs-lookup"><span data-stu-id="8dd4c-111">Site administration activities</span></span>](https://docs.microsoft.com/office365/securitycompliance/search-the-audit-log-in-security-and-compliance#site-administration-activities)
- <span data-ttu-id="8dd4c-112">Untuk informasi selengkapnya tentang cara mengambil peristiwa ini, lihat [pencarian audit log](https://docs.microsoft.com/office365/securitycompliance/search-the-audit-log-in-security-and-compliance#search-the-audit-log).</span><span class="sxs-lookup"><span data-stu-id="8dd4c-112">For more information about how to retrieve these events, see [Search the audit log](https://docs.microsoft.com/office365/securitycompliance/search-the-audit-log-in-security-and-compliance#search-the-audit-log).</span></span>

<span data-ttu-id="8dd4c-113">**Log audit klasik SharePoint**</span><span class="sxs-lookup"><span data-stu-id="8dd4c-113">**SharePoint classic Audit logs**</span></span>

<span data-ttu-id="8dd4c-114">Kami bermigrasi SPO warisan audit untuk terpadu audit log (UAL).</span><span class="sxs-lookup"><span data-stu-id="8dd4c-114">We migrated SPO legacy auditing to Unified Audit Log (UAL).</span></span> <span data-ttu-id="8dd4c-115">Ini pada dasarnya berarti bahwa semua SPO warisan audit laporan sekarang akan didukung melalui UAL, dan warisan audit sinyal telah dipindahkan ke UAL.</span><span class="sxs-lookup"><span data-stu-id="8dd4c-115">This essentially means that all SPO legacy audit reports will now be powered through UAL, and the legacy audit signals have been migrated to UAL.</span></span>

<span data-ttu-id="8dd4c-116">Perubahan utama:</span><span class="sxs-lookup"><span data-stu-id="8dd4c-116">Key changes:</span></span>

- <span data-ttu-id="8dd4c-117">Pemangkasan sebagai kemampuan tidak tersedia.</span><span class="sxs-lookup"><span data-stu-id="8dd4c-117">Trimming as a capability is NOT available.</span></span>
- <span data-ttu-id="8dd4c-118">Bagian di mana Anda memilih peristiwa khusus untuk mengaudit tidak tersedia.</span><span class="sxs-lookup"><span data-stu-id="8dd4c-118">The section where you choose specific events to audit is NOT available.</span></span> <span data-ttu-id="8dd4c-119">Silakan lihat [dokumen ini](https://docs.microsoft.com/office365/securitycompliance/search-the-audit-log-in-security-and-compliance) untuk daftar lengkap dari peristiwa yang diaudit yang tersedia secara default.</span><span class="sxs-lookup"><span data-stu-id="8dd4c-119">Please refer to [this document](https://docs.microsoft.com/office365/securitycompliance/search-the-audit-log-in-security-and-compliance) for a complete list of audited events available by default.</span></span>
- <span data-ttu-id="8dd4c-120">Opsi "lokasi" di bawah **laporan kustom** tidak tersedia.</span><span class="sxs-lookup"><span data-stu-id="8dd4c-120">The "Location" option under **Customized reports** is NOT available.</span></span> 
- <span data-ttu-id="8dd4c-121">"Membuka atau men-download dokumen" peristiwa ini tidak tersedia.</span><span class="sxs-lookup"><span data-stu-id="8dd4c-121">“Opening or downloading documents” events is NOT available.</span></span> 

