---
title: Mengubah Server Nama
ms.author: pebaum
author: pebaum
manager: mnirkhe
ms.date: 04/21/2020
ms.audience: Admin
ms.topic: article
ROBOTS: NOINDEX, NOFOLLOW
localization_priority: Priority
ms.collection: Adm_O365
ms.custom:
- "5"
- "14"
ms.openlocfilehash: 572f8befd84f55cb07a3535852a46e735d3ed620
ms.sourcegitcommit: 55eff703a17e500681d8fa6a87eb067019ade3cc
ms.translationtype: HT
ms.contentlocale: id-ID
ms.lasthandoff: 04/22/2020
ms.locfileid: "43706758"
---
# <a name="update-your-domain-nameservers-to-point-to-microsoft"></a><span data-ttu-id="3501d-102">Memperbarui server nama domain agar mengarah ke Microsoft</span><span class="sxs-lookup"><span data-stu-id="3501d-102">Update your domain nameservers to point to Microsoft</span></span>

<span data-ttu-id="3501d-103">Catatan: Perubahan server nama dapat memakan waktu hingga 48 jam untuk diterapkan.</span><span class="sxs-lookup"><span data-stu-id="3501d-103">Note: Nameserver changes can sometimes take up to 48 hours to propagate.</span></span>
  
<span data-ttu-id="3501d-104">Untuk menyiapkan domain di Microsoft 365, server nama di pendaftar perlu diperbarui.</span><span class="sxs-lookup"><span data-stu-id="3501d-104">To set up your domain in Microsoft 365, the nameservers at your registrar need to be updated.</span></span> <span data-ttu-id="3501d-105">Buat atau edit catatan server nama di pendaftar domain Anda.</span><span class="sxs-lookup"><span data-stu-id="3501d-105">Create or edit your nameserver records at your domain registrar.</span></span>
  
1. <span data-ttu-id="3501d-106">Kunjungi situs web pendaftar domain dan temukan area tempat Anda dapat mengedit server nama.</span><span class="sxs-lookup"><span data-stu-id="3501d-106">Go to your domain registrar's website and find the area where you can edit the nameservers.</span></span>
  
2. <span data-ttu-id="3501d-107">Buat atau edit dua catatan server nama agar sesuai dengan nilai berikut:</span><span class="sxs-lookup"><span data-stu-id="3501d-107">Create or edit two nameserver records to match these values:</span></span>

  - <span data-ttu-id="3501d-108">ns1.bdm.microsoftonline.com</span><span class="sxs-lookup"><span data-stu-id="3501d-108">ns1.bdm.microsoftonline.com</span></span>

  - <span data-ttu-id="3501d-109">ns2.bdm.microsoftonline.com</span><span class="sxs-lookup"><span data-stu-id="3501d-109">ns2.bdm.microsoftonline.com</span></span>

3. <span data-ttu-id="3501d-110">Simpan perubahan.</span><span class="sxs-lookup"><span data-stu-id="3501d-110">Save changes.</span></span>

<span data-ttu-id="3501d-111">Anda juga dapat menemukan instruksi mendetail dalam artikel ini: [Mengubah server nama dengan pendaftar domain apa pun](https://docs.microsoft.com//office365/admin/get-help-with-domains/change-nameservers-at-any-domain-registrar)</span><span class="sxs-lookup"><span data-stu-id="3501d-111">You can also find detailed instructions in this article: [Change nameservers with any domain registrar](https://docs.microsoft.com//office365/admin/get-help-with-domains/change-nameservers-at-any-domain-registrar)</span></span>
  