---
title: Membuat grup
ms.author: pebaum
author: pebaum
manager: mnirkhe
ms.audience: Admin
ms.topic: article
ms.service: o365-administration
ROBOTS: NOINDEX, NOFOLLOW
localization_priority: Normal
ms.collection: Adm_O365
ms.custom:
- "9003234"
- "7230"
ms.openlocfilehash: b8cb3f1de991bfe7197607d5e8964a018e31c122
ms.sourcegitcommit: 35e2c122d8a838d98d1f0851c29b16282261580f
ms.translationtype: MT
ms.contentlocale: id-ID
ms.lasthandoff: 11/17/2020
ms.locfileid: "49088906"
---
# <a name="create-a-group"></a><span data-ttu-id="20287-102">Membuat grup</span><span class="sxs-lookup"><span data-stu-id="20287-102">Create a group</span></span>

<span data-ttu-id="20287-103">Topik ini menguraikan pembuatan grup.</span><span class="sxs-lookup"><span data-stu-id="20287-103">This topic describes group creation.</span></span>

<span data-ttu-id="20287-104">**Izin untuk membuat grup**</span><span class="sxs-lookup"><span data-stu-id="20287-104">**Permission to Create a Group**</span></span>

<span data-ttu-id="20287-105">Pastikan Anda memiliki wewenang untuk membuat grup baru.</span><span class="sxs-lookup"><span data-stu-id="20287-105">Ensure you are authorized to create a new group.</span></span> <span data-ttu-id="20287-106">Administrator global dapat menonaktifkan pembuatan grup di portal Azure atau panel akses.</span><span class="sxs-lookup"><span data-stu-id="20287-106">Global administrators can disable group creation in the Azure portal or Access Panel.</span></span> <span data-ttu-id="20287-107">Anda mungkin memerlukan administrator untuk membuat grup baru untuk Anda, atau untuk memberi izin yang sesuai.</span><span class="sxs-lookup"><span data-stu-id="20287-107">You may need an administrator to create the new group for you, or to give you appropriate permissions.</span></span>

<span data-ttu-id="20287-108">**Mengelola izin pembuatan grup**</span><span class="sxs-lookup"><span data-stu-id="20287-108">**Manage Group creation permissions**</span></span>

1. <span data-ttu-id="20287-109">Administrator global dapat mengelola izin pembuatan grup (untuk alasan keamanan yang terkait) atau grup 365 Office yang dibuat di portal Azure atau panel akses, dengan memilih "pengguna dapat membuat grup keamanan di portal Azure" atau "pengguna dapat membuat grup Office 365 di portal Azure" di **semua grup**  >  **Umum (pengaturan)**.</span><span class="sxs-lookup"><span data-stu-id="20287-109">Global administrators can manage group creation permissions (for security-related reasons) or Office 365 groups created in the Azure portal or Access Panel, by choosing "Users can create security groups in Azure portals" or "Users can create Office 365 groups in Azure portals" options in **All groups** > **General (Settings)**.</span></span>
2. <span data-ttu-id="20287-110">Anda juga bisa membatasi pembuatan grup untuk memilih grup pengguna jika Anda memiliki lisensi Premium Azure Active Directory P1.</span><span class="sxs-lookup"><span data-stu-id="20287-110">You can also restrict group creation to select a group of users if you have an Azure Active Directory P1 Premium license.</span></span>

<span data-ttu-id="20287-111">**Menonaktifkan pemberitahuan Selamat datang untuk anggota grup Office 365 baru**</span><span class="sxs-lookup"><span data-stu-id="20287-111">**Disabling welcome notification for new Office 365 group members**</span></span>

<span data-ttu-id="20287-112">Pemberitahuan sambutan yang dikirimkan kepada pengguna yang ditambahkan ke grup Office 365 dapat dinonaktifkan dengan mengatur **Unifiedgroupwelcomemessagediaktifkan** ke false di PowerShell.</span><span class="sxs-lookup"><span data-stu-id="20287-112">The welcome notification sent to users who are added to Office 365 groups can be disabled by setting **UnifiedGroupWelcomeMessageEnabled** to False in Powershell.</span></span> <span data-ttu-id="20287-113">Pelajari tentang pengaturan ini [di sini](https://docs.microsoft.com/powershell/module/exchange/set-unifiedgroup?view=exchange-ps&preserve-view=true).</span><span class="sxs-lookup"><span data-stu-id="20287-113">Learn about this setting [here](https://docs.microsoft.com/powershell/module/exchange/set-unifiedgroup?view=exchange-ps&preserve-view=true).</span></span>

