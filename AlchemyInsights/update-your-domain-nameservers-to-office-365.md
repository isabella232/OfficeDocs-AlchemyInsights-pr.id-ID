---
title: Memperbarui server nama domain Anda menjadi Office 365
ms.author: v-crytho
author: CrystalThomasMS
ms.date: 5/3/2018
ms.audience: ITPro
ms.topic: article
ROBOTS: NOINDEX, NOFOLLOW
localization_priority: Normal
ms.assetid: 5d38b331-a0e8-4937-8bda-4f8f715e1976
ms.custom:
- "6"
- "14"
ms.openlocfilehash: 23d49c734148739ede0d5e5b53430a42b606c831
ms.sourcegitcommit: a256e8680379c006287ae30996763051c4d9ff85
ms.translationtype: MT
ms.contentlocale: id-ID
ms.lasthandoff: 09/04/2019
ms.locfileid: "36742182"
---
# <a name="update-your-domain-nameservers-to-office-365"></a><span data-ttu-id="f4761-102">Memperbarui server nama domain Anda menjadi Office 365</span><span class="sxs-lookup"><span data-stu-id="f4761-102">Update your domain nameservers to Office 365</span></span>

<span data-ttu-id="f4761-103">Catatan: Perubahan server nama dapat memakan waktu hingga 48 jam untuk diterapkan.</span><span class="sxs-lookup"><span data-stu-id="f4761-103">Note: Nameserver changes can sometimes take up to 48 hours to propagate.</span></span>
  
<span data-ttu-id="f4761-104">Untuk menyiapkan domain di Office 365, server nama pada pendaftar Anda perlu diperbarui.</span><span class="sxs-lookup"><span data-stu-id="f4761-104">To set up your domain in Office 365, the nameservers at your registrar need to be updated.</span></span> <span data-ttu-id="f4761-105">Buat atau edit catatan server nama di pendaftar domain Anda.</span><span class="sxs-lookup"><span data-stu-id="f4761-105">Create or edit your nameserver records at your domain registrar.</span></span>
  
1. <span data-ttu-id="f4761-106">Kunjungi situs web pendaftar domain dan temukan area tempat Anda dapat mengedit server nama.</span><span class="sxs-lookup"><span data-stu-id="f4761-106">Go to your domain registrar's website and find the area where you can edit the nameservers.</span></span>

2. <span data-ttu-id="f4761-107">Buat atau edit dua catatan server nama agar sesuai dengan nilai berikut:</span><span class="sxs-lookup"><span data-stu-id="f4761-107">Create or edit two nameserver records to match these values:</span></span>

  - <span data-ttu-id="f4761-108">ns1.bdm.microsoftonline.com</span><span class="sxs-lookup"><span data-stu-id="f4761-108">ns1.bdm.microsoftonline.com</span></span>

  - <span data-ttu-id="f4761-109">ns2.bdm.microsoftonline.com</span><span class="sxs-lookup"><span data-stu-id="f4761-109">ns2.bdm.microsoftonline.com</span></span>

3. <span data-ttu-id="f4761-110">Simpan perubahan.</span><span class="sxs-lookup"><span data-stu-id="f4761-110">Save changes.</span></span>

<span data-ttu-id="f4761-111">Anda juga dapat menemukan instruksi mendetail dalam artikel ini: [Mengubah server nama untuk menyiapkan Office 365 dengan pendaftar domain apa pun](https://docs.microsoft.com/office365/admin/get-help-with-domains/change-nameservers-at-any-domain-registrar)</span><span class="sxs-lookup"><span data-stu-id="f4761-111">You can also find detailed instructions in this article: [Change nameservers to set up Office 365 with any domain registrar](https://docs.microsoft.com/office365/admin/get-help-with-domains/change-nameservers-at-any-domain-registrar)</span></span>
  