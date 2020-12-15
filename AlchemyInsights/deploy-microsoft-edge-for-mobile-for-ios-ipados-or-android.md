---
title: Menyebarkan Microsoft Edge untuk ponsel untuk iOS/iPadOS atau Android
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
- "9003919"
- "6974"
ms.openlocfilehash: 98ab637b6ca0f2b3cfa98ae897d6ed1d9f36c3cd
ms.sourcegitcommit: 097a8cabe0d2280af489159789988a0ab532dabb
ms.translationtype: MT
ms.contentlocale: id-ID
ms.lasthandoff: 12/11/2020
ms.locfileid: "49678455"
---
# <a name="deploy-microsoft-edge-for-mobile-for-iosipados-or-android"></a><span data-ttu-id="7482a-102">Menyebarkan Microsoft Edge untuk ponsel untuk iOS/iPadOS atau Android</span><span class="sxs-lookup"><span data-stu-id="7482a-102">Deploy Microsoft Edge for Mobile for iOS/iPadOS or Android</span></span>

<span data-ttu-id="7482a-103">Skenario terpandu yang diringkas di bawah akan membantu Anda menetapkan Microsoft Edge kepada pengguna iOS, iPadOS, dan perangkat Android.</span><span class="sxs-lookup"><span data-stu-id="7482a-103">The guided scenario summarized below will help you assign Microsoft Edge to users of iOS, iPadOS, and Android devices.</span></span> <span data-ttu-id="7482a-104">Setelah Anda menyelesaikan langkah-langkah ini, kebijakan Microsoft Intune akan mengaktifkan fitur berikut Microsoft Edge untuk bisnis:</span><span class="sxs-lookup"><span data-stu-id="7482a-104">After you complete these steps, Microsoft Intune policies will enable the following features of Microsoft Edge for business:</span></span>

- <span data-ttu-id="7482a-105">Identitas ganda</span><span class="sxs-lookup"><span data-stu-id="7482a-105">Dual identity</span></span>
- <span data-ttu-id="7482a-106">Integrasi dengan kebijakan proteksi aplikasi Microsoft Intune</span><span class="sxs-lookup"><span data-stu-id="7482a-106">Integration with Microsoft Intune app protection policy</span></span>
- <span data-ttu-id="7482a-107">Integrasi dengan proksi aplikasi Azure Active Directory</span><span class="sxs-lookup"><span data-stu-id="7482a-107">Integration with Azure Active Directory Application Proxy</span></span>
- <span data-ttu-id="7482a-108">Pintasan Halaman favorit dan Beranda terkelola</span><span class="sxs-lookup"><span data-stu-id="7482a-108">Managed favorites and home page shortcuts</span></span>

> [!NOTE]
> <span data-ttu-id="7482a-109">Jika Anda memblokir pengguna dari perangkat seluler yang didaftarkan, skenario yang dipandu ini tidak akan berfungsi dan pengguna perlu menginstal Microsoft Edge secara mandiri.</span><span class="sxs-lookup"><span data-stu-id="7482a-109">If you blocked users from enrolling mobile devices, this guided scenario will not work and the users will need to install Microsoft Edge on their own.</span></span>

<span data-ttu-id="7482a-110">Untuk menggunakan Microsoft Edge untuk ponsel untuk iOS/iPadOS atau Android, lihat:</span><span class="sxs-lookup"><span data-stu-id="7482a-110">To deploy Microsoft Edge for Mobile for iOS/iPadOS or Android, see:</span></span>

1. [<span data-ttu-id="7482a-111">Tuntutan</span><span class="sxs-lookup"><span data-stu-id="7482a-111">Prerequisites</span></span>](https://go.microsoft.com/fwlink/?linkid=2133027)
2. [<span data-ttu-id="7482a-112">Muka</span><span class="sxs-lookup"><span data-stu-id="7482a-112">Introduction</span></span>](https://go.microsoft.com/fwlink/?linkid=2133520)
3. [<span data-ttu-id="7482a-113">Membahas</span><span class="sxs-lookup"><span data-stu-id="7482a-113">Basics</span></span>](https://go.microsoft.com/fwlink/?linkid=2133421)
4. [<span data-ttu-id="7482a-114">Susunan</span><span class="sxs-lookup"><span data-stu-id="7482a-114">Configuration</span></span>](https://go.microsoft.com/fwlink/?linkid=2133521)
5. [<span data-ttu-id="7482a-115">Mengumpulkan</span><span class="sxs-lookup"><span data-stu-id="7482a-115">Assignments</span></span>](https://go.microsoft.com/fwlink/?linkid=2132869)
6. [<span data-ttu-id="7482a-116">Peninjauan dan pembuatan</span><span class="sxs-lookup"><span data-stu-id="7482a-116">Review and creation</span></span>](https://go.microsoft.com/fwlink/?linkid=2133522)
