---
title: Menyebarkan Microsoft Edge ke iOS, iPadOS, dan Android
ms.author: v-smandalika
author: v-smandalika
manager: dansimp
ms.date: 02/10/2021
ms.audience: Admin
ms.topic: article
ms.service: o365-administration
ROBOTS: NOINDEX, NOFOLLOW
localization_priority: Priority
ms.collection: Adm_O365
ms.custom:
- "8241"
- "9004604"
ms.openlocfilehash: 524e87ab57e29823361053093708c83831f19687
ms.sourcegitcommit: 03378c78eadac5d950802dcbacc328bca3314032
ms.translationtype: MT
ms.contentlocale: id-ID
ms.lasthandoff: 02/10/2021
ms.locfileid: "50194520"
---
# <a name="deploy-microsoft-edge-to-ios-ipados-and-android"></a><span data-ttu-id="751d6-102">Menyebarkan Microsoft Edge ke iOS, iPadOS, dan Android</span><span class="sxs-lookup"><span data-stu-id="751d6-102">Deploy Microsoft Edge to iOS, iPadOS, and Android</span></span>

<span data-ttu-id="751d6-103">Skenario terpandu yang diringkas di bawah akan membantu Anda menetapkan Microsoft Edge kepada pengguna iOS, iPadOS, dan perangkat Android.</span><span class="sxs-lookup"><span data-stu-id="751d6-103">The guided scenario summarized below will help you assign Microsoft Edge to users of iOS, iPadOS, and Android devices.</span></span>

> [!NOTE]
> <span data-ttu-id="751d6-104">Jika Anda memblokir pengguna dari perangkat seluler yang didaftarkan, skenario yang dipandu ini tidak akan berfungsi dan pengguna perlu menginstal Microsoft Edge secara mandiri.</span><span class="sxs-lookup"><span data-stu-id="751d6-104">If you blocked users from enrolling mobile devices, this guided scenario won't work and the users will need to install Microsoft Edge on their own.</span></span>

<span data-ttu-id="751d6-105">Skenario terpandu melibatkan langkah-langkah berikut:</span><span class="sxs-lookup"><span data-stu-id="751d6-105">The guided scenario involves the following steps:</span></span>

1. [<span data-ttu-id="751d6-106">Tuntutan</span><span class="sxs-lookup"><span data-stu-id="751d6-106">Prerequisites</span></span>](https://docs.microsoft.com/mem/intune/fundamentals/guided-scenarios-edge#prerequisites)
2. [<span data-ttu-id="751d6-107">Muka</span><span class="sxs-lookup"><span data-stu-id="751d6-107">Introduction</span></span>](https://docs.microsoft.com/mem/intune/fundamentals/guided-scenarios-edge#step-1---introduction)
3. [<span data-ttu-id="751d6-108">Membahas</span><span class="sxs-lookup"><span data-stu-id="751d6-108">Basics</span></span>](https://docs.microsoft.com/mem/intune/fundamentals/guided-scenarios-edge#step-2---basics)
4. [<span data-ttu-id="751d6-109">Susunan</span><span class="sxs-lookup"><span data-stu-id="751d6-109">Configuration</span></span>](https://docs.microsoft.com/mem/intune/fundamentals/guided-scenarios-edge#step-3---configuration)
5. [<span data-ttu-id="751d6-110">Mengumpulkan</span><span class="sxs-lookup"><span data-stu-id="751d6-110">Assignments</span></span>](https://docs.microsoft.com/mem/intune/fundamentals/guided-scenarios-edge#step-4---assignments)
6. [<span data-ttu-id="751d6-111">Peninjauan dan pembuatan</span><span class="sxs-lookup"><span data-stu-id="751d6-111">Review and creation</span></span>](https://docs.microsoft.com/mem/intune/fundamentals/guided-scenarios-edge#step-5---review--create)

<span data-ttu-id="751d6-112">Setelah Anda menyelesaikan langkah-langkah dalam skenario terpandu, kebijakan Microsoft Intune akan mengaktifkan fitur Microsoft Edge untuk bisnis berikut ini:</span><span class="sxs-lookup"><span data-stu-id="751d6-112">After you complete the steps in the guided scenario, Microsoft Intune policies will enable the following features of Microsoft Edge for business:</span></span>

- <span data-ttu-id="751d6-113">Identitas ganda</span><span class="sxs-lookup"><span data-stu-id="751d6-113">Dual identity</span></span>
- <span data-ttu-id="751d6-114">Integrasi dengan kebijakan proteksi aplikasi Microsoft Intune</span><span class="sxs-lookup"><span data-stu-id="751d6-114">Integration with Microsoft Intune app protection policy</span></span>
- <span data-ttu-id="751d6-115">Integrasi dengan proksi aplikasi Azure Active Directory</span><span class="sxs-lookup"><span data-stu-id="751d6-115">Integration with Azure Active Directory Application Proxy</span></span>
- <span data-ttu-id="751d6-116">Pintasan Halaman favorit dan Beranda terkelola</span><span class="sxs-lookup"><span data-stu-id="751d6-116">Managed favorites and home page shortcuts</span></span>
