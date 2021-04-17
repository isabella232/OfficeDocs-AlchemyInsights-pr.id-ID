---
title: Membuat grup
ms.author: pebaum
author: pebaum
manager: scotv
ms.audience: Admin
ms.topic: article
ms.service: o365-administration
ROBOTS: NOINDEX, NOFOLLOW
localization_priority: Normal
ms.collection: Adm_O365
ms.custom:
- "9003234"
- "7230"
ms.openlocfilehash: ec74b7c098d302d3bdeb5a412fad41efe7b82b98
ms.sourcegitcommit: 8bc60ec34bc1e40685e3976576e04a2623f63a7c
ms.translationtype: MT
ms.contentlocale: id-ID
ms.lasthandoff: 04/15/2021
ms.locfileid: "51816359"
---
# <a name="create-a-group"></a><span data-ttu-id="391a2-102">Membuat grup</span><span class="sxs-lookup"><span data-stu-id="391a2-102">Create a group</span></span>

<span data-ttu-id="391a2-103">Topik ini menjelaskan pembuatan grup.</span><span class="sxs-lookup"><span data-stu-id="391a2-103">This topic describes group creation.</span></span>

<span data-ttu-id="391a2-104">**Izin untuk Membuat Grup**</span><span class="sxs-lookup"><span data-stu-id="391a2-104">**Permission to Create a Group**</span></span>

<span data-ttu-id="391a2-105">Pastikan Anda memiliki wewenang untuk membuat grup baru.</span><span class="sxs-lookup"><span data-stu-id="391a2-105">Ensure you are authorized to create a new group.</span></span> <span data-ttu-id="391a2-106">Administrator global dapat menonaktifkan pembuatan grup di portal Azure atau Panel Akses.</span><span class="sxs-lookup"><span data-stu-id="391a2-106">Global administrators can disable group creation in the Azure portal or Access Panel.</span></span> <span data-ttu-id="391a2-107">Anda mungkin memerlukan administrator untuk membuat grup baru untuk Anda, atau memberi Anda izin yang tepat.</span><span class="sxs-lookup"><span data-stu-id="391a2-107">You may need an administrator to create the new group for you, or to give you appropriate permissions.</span></span>

<span data-ttu-id="391a2-108">**Mengelola izin pembuatan Grup**</span><span class="sxs-lookup"><span data-stu-id="391a2-108">**Manage Group creation permissions**</span></span>

1. <span data-ttu-id="391a2-109">Administrator global dapat mengelola izin pembuatan grup (untuk alasan terkait keamanan) atau grup Office 365 yang dibuat di portal Azure atau Panel Access, dengan memilih "Pengguna dapat membuat grup keamanan di portal Azure" atau "Pengguna dapat membuat grup Office 365 di portal Azure" di opsi Semua grup Umum  >  **(Pengaturan).**</span><span class="sxs-lookup"><span data-stu-id="391a2-109">Global administrators can manage group creation permissions (for security-related reasons) or Office 365 groups created in the Azure portal or Access Panel, by choosing "Users can create security groups in Azure portals" or "Users can create Office 365 groups in Azure portals" options in **All groups** > **General (Settings)**.</span></span>
2. <span data-ttu-id="391a2-110">Anda juga dapat membatasi pembuatan grup untuk memilih grup pengguna jika memiliki lisensi Azure Active Directory P1 Premium.</span><span class="sxs-lookup"><span data-stu-id="391a2-110">You can also restrict group creation to select a group of users if you have an Azure Active Directory P1 Premium license.</span></span>

<span data-ttu-id="391a2-111">**Menonaktifkan pemberitahuan selamat datang untuk anggota grup Office 365 baru**</span><span class="sxs-lookup"><span data-stu-id="391a2-111">**Disabling welcome notification for new Office 365 group members**</span></span>

<span data-ttu-id="391a2-112">Pemberitahuan selamat datang yang dikirimkan kepada pengguna yang ditambahkan ke grup Office 365 bisa dinonaktifkan dengan menyetel **UnifiedGroupWelcomeMessageEnabled** ke False di Powershell.</span><span class="sxs-lookup"><span data-stu-id="391a2-112">The welcome notification sent to users who are added to Office 365 groups can be disabled by setting **UnifiedGroupWelcomeMessageEnabled** to False in Powershell.</span></span> <span data-ttu-id="391a2-113">Pelajari tentang pengaturan ini di [sini](https://docs.microsoft.com/powershell/module/exchange/set-unifiedgroup?view=exchange-ps&preserve-view=true).</span><span class="sxs-lookup"><span data-stu-id="391a2-113">Learn about this setting [here](https://docs.microsoft.com/powershell/module/exchange/set-unifiedgroup?view=exchange-ps&preserve-view=true).</span></span>

