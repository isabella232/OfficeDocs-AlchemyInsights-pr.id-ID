---
title: Tentang admin Yammer
ms.author: v-jmathew
author: v-jmathew
manager: scotv
audience: Admin
ms.topic: article
ms.service: o365-administration
ROBOTS: NOINDEX, NOFOLLOW
localization_priority: Normal
ms.collection: Adm_O365
ms.custom:
- "9003221"
- "9714"
ms.openlocfilehash: fd8534d44c44f2ea8e6b0de8c361109915566868
ms.sourcegitcommit: a6ab402f59e5ee1492bcf5ab7f18714fc251717d
ms.translationtype: MT
ms.contentlocale: id-ID
ms.lasthandoff: 03/22/2021
ms.locfileid: "51036716"
---
# <a name="about-yammer-admins"></a><span data-ttu-id="27d05-102">Tentang admin Yammer</span><span class="sxs-lookup"><span data-stu-id="27d05-102">About Yammer admins</span></span>

<span data-ttu-id="27d05-103">**Admin jaringan**</span><span class="sxs-lookup"><span data-stu-id="27d05-103">**Network admins**</span></span>

<span data-ttu-id="27d05-104">Admin global secara otomatis dipromosikan ke peran admin yang diverifikasi dalam jaringan Yammer.</span><span class="sxs-lookup"><span data-stu-id="27d05-104">Global admins are automatically promoted to the Verified Admin role in a Yammer network.</span></span> <span data-ttu-id="27d05-105">Dalam kasus berikut, promosi ini mungkin tidak terjadi dengan benar:</span><span class="sxs-lookup"><span data-stu-id="27d05-105">In the following cases, this promotion may not occur correctly:</span></span>

- <span data-ttu-id="27d05-106">Beberapa jaringan Yammer ada, dan admin sedang masuk ke yang salah.</span><span class="sxs-lookup"><span data-stu-id="27d05-106">Multiple Yammer networks exist, and the admin is being signed into the wrong one.</span></span> <span data-ttu-id="27d05-107">[Konsolidasi jaringan](https://docs.microsoft.com/yammer/configure-your-yammer-network/consolidate-multiple-yammer-networks) diperlukan untuk masuk ke satu jaringan Yammer.</span><span class="sxs-lookup"><span data-stu-id="27d05-107">[Network consolidation](https://docs.microsoft.com/yammer/configure-your-yammer-network/consolidate-multiple-yammer-networks) is required to get to one Yammer network.</span></span>
- <span data-ttu-id="27d05-108">PIM Azure sedang digunakan.</span><span class="sxs-lookup"><span data-stu-id="27d05-108">Azure PIM is being used.</span></span> <span data-ttu-id="27d05-109">Pengguna mungkin tidak dipromosikan ke admin global cukup lama agar promosi dapat terjadi.</span><span class="sxs-lookup"><span data-stu-id="27d05-109">The user may not be promoted to global admin long enough for the promotion to occur.</span></span> <span data-ttu-id="27d05-110">Pembaruan mendatang untuk Yammer mungkin mengatasi masalah ini, tetapi yang paling baik adalah mempromosikan pengguna ke admin global secara manual.</span><span class="sxs-lookup"><span data-stu-id="27d05-110">A future update to Yammer may resolve this issue, but it is best to promote users to global admin manually.</span></span>
- <span data-ttu-id="27d05-111">Masalah sinkronisasi ada pada jaringan Yammer.</span><span class="sxs-lookup"><span data-stu-id="27d05-111">A sync issue exists with the Yammer network.</span></span> <span data-ttu-id="27d05-112">Dalam hal ini, permintaan dukungan akan diperlukan untuk investigasi lebih lanjut.</span><span class="sxs-lookup"><span data-stu-id="27d05-112">In this case a support request will be required for further investigation.</span></span>

<span data-ttu-id="27d05-113">Untuk informasi selengkapnya tentang peran admin Yammer, lihat [mengelola admin yammer](https://docs.microsoft.com/yammer/manage-yammer-users/manage-yammer-admins).</span><span class="sxs-lookup"><span data-stu-id="27d05-113">For more information about Yammer admin roles, see [Manage Yammer admins](https://docs.microsoft.com/yammer/manage-yammer-users/manage-yammer-admins).</span></span>

<span data-ttu-id="27d05-114">**Admin grup**</span><span class="sxs-lookup"><span data-stu-id="27d05-114">**Group admins**</span></span>

<span data-ttu-id="27d05-115">Grup admin untuk grup tersambung Microsoft 365 disinkronkan dengan keanggotaan grup dari Azure AD.</span><span class="sxs-lookup"><span data-stu-id="27d05-115">Group admins for Microsoft 365 connected groups are synced with group membership from Azure AD.</span></span> <span data-ttu-id="27d05-116">Untuk grup besar, sinkronisasi ini dapat memerlukan waktu lama.</span><span class="sxs-lookup"><span data-stu-id="27d05-116">For large groups, this sync can take an extended period.</span></span>
