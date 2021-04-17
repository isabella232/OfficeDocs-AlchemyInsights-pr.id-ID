---
title: Teams mengizinkan atau menonaktifkan video IP
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
- "9002537"
- "5617"
ms.openlocfilehash: 059d7a1ad619e25f14bc6f561693b6fe24355132
ms.sourcegitcommit: 8bc60ec34bc1e40685e3976576e04a2623f63a7c
ms.translationtype: MT
ms.contentlocale: id-ID
ms.lasthandoff: 04/15/2021
ms.locfileid: "51826346"
---
# <a name="teams-allow-or-disable-ip-video"></a><span data-ttu-id="2cd59-102">Teams mengizinkan atau menonaktifkan video IP</span><span class="sxs-lookup"><span data-stu-id="2cd59-102">Teams allow or disable IP video</span></span>

<span data-ttu-id="2cd59-103">**Mengubah atau membuat kebijakan rapat**</span><span class="sxs-lookup"><span data-stu-id="2cd59-103">**Change or create a meeting policy**</span></span>

<span data-ttu-id="2cd59-104">Untuk mengubah atau membuat kebijakan rapat, masuk ke pusat **admin Microsoft Teams > Rapat > Rapat**.</span><span class="sxs-lookup"><span data-stu-id="2cd59-104">To change or create a meeting policy, go to the **Microsoft Teams admin center > Meetings > Meeting policies**.</span></span> <span data-ttu-id="2cd59-105">Pilih kebijakan dari daftar atau klik **Tambahkan**.</span><span class="sxs-lookup"><span data-stu-id="2cd59-105">Select a policy from the list or click **Add**.</span></span> <span data-ttu-id="2cd59-106">Jika membuat kebijakan baru, tambahkan nama dan deskripsi.</span><span class="sxs-lookup"><span data-stu-id="2cd59-106">If you're creating a new policy, add a name and description.</span></span> <span data-ttu-id="2cd59-107">Nama tidak boleh berisi karakter khusus atau lebih panjang dari 64 karakter.</span><span class="sxs-lookup"><span data-stu-id="2cd59-107">The name can't contain special characters or be longer than 64 characters.</span></span> <span data-ttu-id="2cd59-108">Pilih pengaturan Anda, lalu klik **Simpan**.</span><span class="sxs-lookup"><span data-stu-id="2cd59-108">Choose your settings, and then click **Save**.</span></span>

<span data-ttu-id="2cd59-109">Misalnya, katakanlah Anda memiliki banyak pengguna dan Anda ingin membatasi jumlah bandwith yang akan dibutuhkan rapat mereka.</span><span class="sxs-lookup"><span data-stu-id="2cd59-109">For example, say you have many users and you want to limit the amount of bandwidth that their meeting would require.</span></span> <span data-ttu-id="2cd59-110">Anda dapat membuat kebijakan kustom baru bernama "Bandwidth terbatas" dan menonaktifkan pengaturan berikut:</span><span class="sxs-lookup"><span data-stu-id="2cd59-110">You would create a new custom policy named "Limited bandwidth" and disable the following settings:</span></span>

<span data-ttu-id="2cd59-111">Dalam **Audio & video**:</span><span class="sxs-lookup"><span data-stu-id="2cd59-111">Under **Audio & video**:</span></span>

- <span data-ttu-id="2cd59-112">Nonaktifkan Izin perekaman awan.</span><span class="sxs-lookup"><span data-stu-id="2cd59-112">Turn off Allow cloud recording.</span></span>
- <span data-ttu-id="2cd59-113">Nonaktifkan Izin video IP.</span><span class="sxs-lookup"><span data-stu-id="2cd59-113">Turn off Allow IP video.</span></span>

<span data-ttu-id="2cd59-114">Kemudian tetapkan kebijakan ke pengguna.</span><span class="sxs-lookup"><span data-stu-id="2cd59-114">Then assign the policy to the users.</span></span>

<span data-ttu-id="2cd59-115">**Menetapkan kebijakan rapat ke pengguna**</span><span class="sxs-lookup"><span data-stu-id="2cd59-115">**Assign a meeting policy to users**</span></span>

1. <span data-ttu-id="2cd59-116">Di navigasi sebelah kiri pusat admin Microsoft Teams, masuk ke **Pengguna**, lalu klik pengguna.</span><span class="sxs-lookup"><span data-stu-id="2cd59-116">In the left navigation of the Microsoft Teams admin center, go to **Users**, and then click the user.</span></span>
2. <span data-ttu-id="2cd59-117">Pilih pengguna dengan mengklik di bagian sebelah kiri nama pengguna, lalu klik **Edit pengaturan**.</span><span class="sxs-lookup"><span data-stu-id="2cd59-117">Select the user by clicking to the left of the user name, and then click **Edit settings**.</span></span>
3. <span data-ttu-id="2cd59-118">Di **bawah Kebijakan** rapat , pilih kebijakan yang ingin Anda tetapkan lalu klik **Terapkan.**</span><span class="sxs-lookup"><span data-stu-id="2cd59-118">Under **Meeting policy**, select the policy you want to assign and then click **Apply**.</span></span>

<span data-ttu-id="2cd59-119">Untuk informasi selengkapnya, lihat [Mengelola kebijakan rapat di Teams](https://docs.microsoft.com/microsoftteams/meeting-policies-in-teams).</span><span class="sxs-lookup"><span data-stu-id="2cd59-119">For more information, see [Manage meeting policies in Teams](https://docs.microsoft.com/microsoftteams/meeting-policies-in-teams).</span></span>
