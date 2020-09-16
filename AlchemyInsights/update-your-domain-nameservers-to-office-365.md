---
title: Memperbarui server nama domain agar mengarah ke Microsoft
ms.author: pebaum
author: CrystalThomasMS
ms.date: 04/21/2020
ms.audience: ITPro
ms.topic: article
ms.service: o365-administration
ROBOTS: NOINDEX, NOFOLLOW
localization_priority: Normal
ms.assetid: 5d38b331-a0e8-4937-8bda-4f8f715e1976
ms.custom:
- "6"
- "14"
ms.openlocfilehash: 7322fa640f6d043f057c8b7a5e06a18dcd10eec5
ms.sourcegitcommit: c6692ce0fa1358ec3529e59ca0ecdfdea4cdc759
ms.translationtype: MT
ms.contentlocale: id-ID
ms.lasthandoff: 09/14/2020
ms.locfileid: "47734914"
---
# <a name="update-your-domain-nameservers-to-point-to-microsoft"></a><span data-ttu-id="01b6b-102">Memperbarui server nama domain agar mengarah ke Microsoft</span><span class="sxs-lookup"><span data-stu-id="01b6b-102">Update your domain nameservers to point to Microsoft</span></span>

<span data-ttu-id="01b6b-103">Catatan: Perubahan server nama dapat memakan waktu hingga 48 jam untuk diterapkan.</span><span class="sxs-lookup"><span data-stu-id="01b6b-103">Note: Nameserver changes can sometimes take up to 48 hours to propagate.</span></span>
  
<span data-ttu-id="01b6b-104">Untuk menyiapkan domain Anda dengan Microsoft, nameserver di pencatat perlu diperbarui.</span><span class="sxs-lookup"><span data-stu-id="01b6b-104">To set up your domain with Microsoft, the nameservers at your registrar need to be updated.</span></span> <span data-ttu-id="01b6b-105">Buat atau edit catatan server nama di pendaftar domain Anda.</span><span class="sxs-lookup"><span data-stu-id="01b6b-105">Create or edit your nameserver records at your domain registrar.</span></span>
  
1. <span data-ttu-id="01b6b-106">Kunjungi situs web pendaftar domain dan temukan area tempat Anda dapat mengedit server nama.</span><span class="sxs-lookup"><span data-stu-id="01b6b-106">Go to your domain registrar's website and find the area where you can edit the nameservers.</span></span>

2. <span data-ttu-id="01b6b-107">Buat atau edit dua catatan server nama agar sesuai dengan nilai berikut:</span><span class="sxs-lookup"><span data-stu-id="01b6b-107">Create or edit two nameserver records to match these values:</span></span>

  - <span data-ttu-id="01b6b-108">ns1.bdm.microsoftonline.com</span><span class="sxs-lookup"><span data-stu-id="01b6b-108">ns1.bdm.microsoftonline.com</span></span>

  - <span data-ttu-id="01b6b-109">ns2.bdm.microsoftonline.com</span><span class="sxs-lookup"><span data-stu-id="01b6b-109">ns2.bdm.microsoftonline.com</span></span>

3. <span data-ttu-id="01b6b-110">Simpan perubahan.</span><span class="sxs-lookup"><span data-stu-id="01b6b-110">Save changes.</span></span>

<span data-ttu-id="01b6b-111">Anda juga dapat menemukan instruksi mendetail di artikel ini: [mengubah nameserver untuk menyiapkan Microsoft 365 dengan pencatat domain apa pun](https://docs.microsoft.com/microsoft-365/admin/get-help-with-domains/change-nameservers-at-any-domain-registrar)</span><span class="sxs-lookup"><span data-stu-id="01b6b-111">You can also find detailed instructions in this article: [Change nameservers to set up Microsoft 365 with any domain registrar](https://docs.microsoft.com/microsoft-365/admin/get-help-with-domains/change-nameservers-at-any-domain-registrar)</span></span>
  