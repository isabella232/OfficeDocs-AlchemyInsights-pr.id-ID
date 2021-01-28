---
title: Log dan pelaporan
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
- "9004331"
- "7727"
ms.openlocfilehash: 7349efb02f8d6ac5d73f6d6cd06eef6308ffe9be
ms.sourcegitcommit: 117c64e1fbcb5eec04f94eadad71423b974e7b14
ms.translationtype: MT
ms.contentlocale: id-ID
ms.lasthandoff: 01/27/2021
ms.locfileid: "50036004"
---
# <a name="logs-and-reporting"></a><span data-ttu-id="fe997-102">Log dan pelaporan</span><span class="sxs-lookup"><span data-stu-id="fe997-102">Logs and Reporting</span></span>

<span data-ttu-id="fe997-103">[Tanya jawab umum pelaporan Azure Active Directory](https://docs.microsoft.com/azure/active-directory/active-directory-reporting-faq) jawaban tanya jawab umum tentang pelaporan Azure Active Directory (Azure AD).</span><span class="sxs-lookup"><span data-stu-id="fe997-103">[Azure Active Directory reporting FAQ](https://docs.microsoft.com/azure/active-directory/active-directory-reporting-faq) answers frequently asked questions about Azure Active Directory (Azure AD) reporting.</span></span> <span data-ttu-id="fe997-104">Untuk informasi selengkapnya, lihat [pelaporan Azure Active Directory](https://docs.microsoft.com/azure/active-directory/reports-monitoring/overview-reports).</span><span class="sxs-lookup"><span data-stu-id="fe997-104">For more information, see [Azure Active Directory reporting](https://docs.microsoft.com/azure/active-directory/reports-monitoring/overview-reports).</span></span>

<span data-ttu-id="fe997-105">**Memecahkan masalah dengan audit**</span><span class="sxs-lookup"><span data-stu-id="fe997-105">**Troubleshooting issues with Audit**</span></span>

1. <span data-ttu-id="fe997-106">Jika Anda mengalami masalah saat melihat beberapa aktivitas audit dan aktivitas yang hilang ada dalam [Daftar](https://docs.microsoft.com/azure/active-directory/reports-monitoring/reference-audit-activities)ini, silakan mengajukan tiket dukungan.</span><span class="sxs-lookup"><span data-stu-id="fe997-106">If you are having issues seeing some audit activities and the missing Activity is in this [list](https://docs.microsoft.com/azure/active-directory/reports-monitoring/reference-audit-activities), please file a support ticket.</span></span>
2. <span data-ttu-id="fe997-107">Jika Anda mengalami masalah dalam melihat setiap log audit dalam penyewa Anda, silakan file tiket dukungan.</span><span class="sxs-lookup"><span data-stu-id="fe997-107">If you are having issues seeing any Audit logs in your tenant, please file a support ticket.</span></span>
3. <span data-ttu-id="fe997-108">Jika aktivitas audit Anda tidak muncul dengan segera di portal Azure, lihat [informasi latensi](https://docs.microsoft.com/azure/active-directory/reports-monitoring/reference-reports-latencies) kami dan file tiket dukungan jika keterlambatan melebihi latensi yang didokumentasikan.</span><span class="sxs-lookup"><span data-stu-id="fe997-108">If your audit activities are not showing up immediately in the Azure Portal, check out our [latency information](https://docs.microsoft.com/azure/active-directory/reports-monitoring/reference-reports-latencies) and file a support ticket if the delay exceeds the documented latency.</span></span>
4. [<span data-ttu-id="fe997-109">Penyimpanan log aktivitas Azure AD</span><span class="sxs-lookup"><span data-stu-id="fe997-109">Azure AD Activity Logs Retention</span></span>](https://docs.microsoft.com/azure/active-directory/reports-monitoring/reference-reports-data-retention)
5. <span data-ttu-id="fe997-110">Jika Anda tidak melihat semua audit untuk rentang tanggal yang Anda pilih, Anda bisa mengunduh hingga baris 250K (diurutkan menurut paling baru) dari masuk dari Azure portal.</span><span class="sxs-lookup"><span data-stu-id="fe997-110">If you don't see all the audit for the date range you selected, you can download up to 250K rows (sorted by most recent) of sign-ins from Azure portal.</span></span> <span data-ttu-id="fe997-111">Untuk informasi selengkapnya, lihat [mengaudit aktivitas unduhan](https://docs.microsoft.com/azure/active-directory/reports-monitoring/quickstart-download-audit-report).</span><span class="sxs-lookup"><span data-stu-id="fe997-111">For more information, see [Audit activities download](https://docs.microsoft.com/azure/active-directory/reports-monitoring/quickstart-download-audit-report).</span></span>

<span data-ttu-id="fe997-112">**Pemecahan masalah dengan masuk**</span><span class="sxs-lookup"><span data-stu-id="fe997-112">**Troubleshooting issues with Sign-ins**</span></span>

1. <span data-ttu-id="fe997-113">Anda hanya bisa melihat 30 hari terakhir data jika Anda memiliki lisensi Azure AD Premium (P1 atau P2) untuk penyewa Anda.</span><span class="sxs-lookup"><span data-stu-id="fe997-113">You can only see the last 30 days of data if you have an Azure AD Premium (P1 or P2) license for your tenant.</span></span>
2. <span data-ttu-id="fe997-114">Masuk hanya tersedia untuk penyewa Premium Azure AD.</span><span class="sxs-lookup"><span data-stu-id="fe997-114">Sign-ins are available only for Azure AD Premium tenants.</span></span> <span data-ttu-id="fe997-115">Ini tidak tersedia untuk penyewa berlisensi gratis atau dasar.</span><span class="sxs-lookup"><span data-stu-id="fe997-115">It's not available for Free or Basic licensed tenants.</span></span>
3. <span data-ttu-id="fe997-116">Jika penyewa Anda memiliki lisensi P1 premium dan Anda tidak bisa melihat proses masuk, lihat [informasi latensi](https://docs.microsoft.com/azure/active-directory/reports-monitoring/reference-reports-latencies) kami dan file tiket dukungan jika keterlambatan melebihi latensi yang didokumentasikan.</span><span class="sxs-lookup"><span data-stu-id="fe997-116">If your tenant has a Premium P1 license and you can't see the sign-ins, check out our [latency information](https://docs.microsoft.com/azure/active-directory/reports-monitoring/reference-reports-latencies) and file a support ticket if the delay exceeds the documented latency.</span></span>
4. <span data-ttu-id="fe997-117">Jika Anda tidak melihat semua masuk untuk rentang tanggal yang Anda pilih, perhatikan bahwa Anda bisa mengunduh hingga 250K baris (diurutkan menurut paling baru) dari masuk dari Azure portal.</span><span class="sxs-lookup"><span data-stu-id="fe997-117">If you don't see all the sign-ins for the date range you selected, note that you can download up to 250K rows (sorted by most recent) of sign-ins from Azure portal.</span></span> <span data-ttu-id="fe997-118">Untuk informasi selengkapnya, lihat [mengunduh aktivitas masuk](https://docs.microsoft.com/azure/active-directory/reports-monitoring/concept-sign-ins#download-sign-in-activities).</span><span class="sxs-lookup"><span data-stu-id="fe997-118">For more information, see [Sign-ins activities download](https://docs.microsoft.com/azure/active-directory/reports-monitoring/concept-sign-ins#download-sign-in-activities).</span></span>

<span data-ttu-id="fe997-119">**Memecahkan masalah laporan keamanan (pengguna berbendera berisiko, masuk berisiko)**</span><span class="sxs-lookup"><span data-stu-id="fe997-119">**Troubleshoot Security Reports (Users Flagged at Risk, Risky Sign-In)**</span></span>

1. [<span data-ttu-id="fe997-120">Pengguna yang ditandai untuk laporan keamanan risiko</span><span class="sxs-lookup"><span data-stu-id="fe997-120">Users flagged for risk security report</span></span>](https://docs.microsoft.com/azure/active-directory/reports-monitoring/concept-user-at-risk)
2. [<span data-ttu-id="fe997-121">Laporan masuk yang berisiko di portal Azure Active Directory</span><span class="sxs-lookup"><span data-stu-id="fe997-121">Risky sign-ins report in the Azure Active Directory portal</span></span>](https://docs.microsoft.com/azure/active-directory/reports-monitoring/concept-risky-sign-ins)
3. [<span data-ttu-id="fe997-122">Kejadian risiko Azure Active Directory</span><span class="sxs-lookup"><span data-stu-id="fe997-122">Azure Active Directory risk events</span></span>](https://docs.microsoft.com/azure/active-directory/reports-monitoring/concept-risk-events)
