---
title: Memverifikasi domain Anda
ms.author: pebaum
author: pebaum
manager: scotv
ms.date: 04/21/2020
ms.audience: Admin
ms.topic: article
ms.service: o365-administration
ROBOTS: NOINDEX, NOFOLLOW
localization_priority: Normal
ms.collection: Adm_O365
ms.custom:
- "47"
- "48"
- "8"
ms.assetid: 81fd176b-3d67-4e52-9ab8-d36602412734
ms.openlocfilehash: 4a34de7fa2aaaae365cf4562d31590d4b5fb7544
ms.sourcegitcommit: 8bc60ec34bc1e40685e3976576e04a2623f63a7c
ms.translationtype: MT
ms.contentlocale: id-ID
ms.lasthandoff: 04/15/2021
ms.locfileid: "51770994"
---
# <a name="verify-your-domain"></a><span data-ttu-id="7874b-102">Memverifikasi domain Anda</span><span class="sxs-lookup"><span data-stu-id="7874b-102">Verify your domain</span></span>

 <span data-ttu-id="7874b-103">**Catatan mungkin belum diperbarui di seluruh Internet.**</span><span class="sxs-lookup"><span data-stu-id="7874b-103">**The record probably hasn't updated across the Internet.**</span></span>
  
<span data-ttu-id="7874b-104">Biasanya hanya membutuhkan beberapa menit agar kami bisa melihat catatan baru, tetapi terkadang bisa memakan waktu hingga beberapa jam.</span><span class="sxs-lookup"><span data-stu-id="7874b-104">It typically only takes a few minutes for us to be able to see the new record, but occasionally it can take as long as a few hours.</span></span> 
  
- <span data-ttu-id="7874b-105">Jika sudah menunggu lama, periksa kembali apakah Anda telah menyalin dan menempelkan nilai yang tepat ke catatan verifikasi TXT di host DNS Anda.</span><span class="sxs-lookup"><span data-stu-id="7874b-105">If you've waited that long already, double-check that you've copied and pasted the exact value into the TXT verification record at your DNS host.</span></span> <span data-ttu-id="7874b-106">Masalah yang sering terjadi adalah, bagian "MS=" dari catatan tidak menyertakannya.</span><span class="sxs-lookup"><span data-stu-id="7874b-106">One common issue is not including the "MS=" part of the record.</span></span> <span data-ttu-id="7874b-107">Kami juga memerlukannya!</span><span class="sxs-lookup"><span data-stu-id="7874b-107">We need that too!</span></span>

- <span data-ttu-id="7874b-108">Di beberapa host DNS, Anda harus melakukan langkah tambahan untuk menyimpan file zona (tempat catatan DNS disimpan) agar diperbarui di seluruh internet.</span><span class="sxs-lookup"><span data-stu-id="7874b-108">At some DNS hosts, you have to take an extra step to save the zone file (where the DNS record is stored) so that it will update across the Internet.</span></span> <span data-ttu-id="7874b-109">Pastikan Anda telah menyimpan perubahan sehingga Microsoft dapat melihat dan memverifikasi catatan.</span><span class="sxs-lookup"><span data-stu-id="7874b-109">Make sure you've saved your changes so Microsoft can see and verify the record.</span></span>
