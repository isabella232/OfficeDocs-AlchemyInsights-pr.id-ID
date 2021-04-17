---
title: Mengubah Server Nama
ms.author: pebaum
author: pebaum
manager: scotv
ms.date: 04/21/2020
ms.audience: Admin
ms.topic: article
ms.service: o365-administration
ROBOTS: NOINDEX, NOFOLLOW
localization_priority: Priority
ms.collection: Adm_O365
ms.custom:
- "5"
- "14"
ms.openlocfilehash: 67680a6fa514d31ccb88cc8691a199cd1f58a402
ms.sourcegitcommit: 8bc60ec34bc1e40685e3976576e04a2623f63a7c
ms.translationtype: HT
ms.contentlocale: id-ID
ms.lasthandoff: 04/15/2021
ms.locfileid: "51818615"
---
# <a name="update-your-domain-nameservers-to-point-to-microsoft"></a><span data-ttu-id="68f24-102">Memperbarui server nama domain agar mengarah ke Microsoft</span><span class="sxs-lookup"><span data-stu-id="68f24-102">Update your domain nameservers to point to Microsoft</span></span>

<span data-ttu-id="68f24-103">Catatan: Perubahan server nama dapat memakan waktu hingga 48 jam untuk diterapkan.</span><span class="sxs-lookup"><span data-stu-id="68f24-103">Note: Nameserver changes can sometimes take up to 48 hours to propagate.</span></span>
  
<span data-ttu-id="68f24-104">Untuk menyiapkan domain di Microsoft 365, server nama di pendaftar perlu diperbarui.</span><span class="sxs-lookup"><span data-stu-id="68f24-104">To set up your domain in Microsoft 365, the nameservers at your registrar need to be updated.</span></span> <span data-ttu-id="68f24-105">Buat atau edit catatan server nama di pendaftar domain Anda.</span><span class="sxs-lookup"><span data-stu-id="68f24-105">Create or edit your nameserver records at your domain registrar.</span></span>
  
1. <span data-ttu-id="68f24-106">Kunjungi situs web pendaftar domain dan temukan area tempat Anda dapat mengedit server nama.</span><span class="sxs-lookup"><span data-stu-id="68f24-106">Go to your domain registrar's website and find the area where you can edit the nameservers.</span></span>
  
2. <span data-ttu-id="68f24-107">Buat atau edit dua catatan server nama agar sesuai dengan nilai berikut:</span><span class="sxs-lookup"><span data-stu-id="68f24-107">Create or edit two nameserver records to match these values:</span></span>

  - <span data-ttu-id="68f24-108">ns1.bdm.microsoftonline.com</span><span class="sxs-lookup"><span data-stu-id="68f24-108">ns1.bdm.microsoftonline.com</span></span>

  - <span data-ttu-id="68f24-109">ns2.bdm.microsoftonline.com</span><span class="sxs-lookup"><span data-stu-id="68f24-109">ns2.bdm.microsoftonline.com</span></span>

3. <span data-ttu-id="68f24-110">Simpan perubahan.</span><span class="sxs-lookup"><span data-stu-id="68f24-110">Save changes.</span></span>

<span data-ttu-id="68f24-111">Anda juga dapat menemukan instruksi mendetail dalam artikel ini: [Mengubah server nama dengan pendaftar domain apa pun](https://docs.microsoft.com/microsoft-365/admin/get-help-with-domains/change-nameservers-at-any-domain-registrar)</span><span class="sxs-lookup"><span data-stu-id="68f24-111">You can also find detailed instructions in this article: [Change nameservers with any domain registrar](https://docs.microsoft.com/microsoft-365/admin/get-help-with-domains/change-nameservers-at-any-domain-registrar)</span></span>
  