---
title: Verifikasi domain
ms.author: pebaum
author: pebaum
manager: mnirkhe
ms.date: 4/5/2018
ms.audience: Admin
ms.topic: article
ROBOTS: NOINDEX, NOFOLLOW
localization_priority: Normal
ms.collection: Adm_O365
ms.custom:
- "47"
- "48"
- "8"
ms.assetid: 81fd176b-3d67-4e52-9ab8-d36602412734
ms.openlocfilehash: 3dd96a9731cfd75882dd3bb397005b19d471c882
ms.sourcegitcommit: 1d98db8acb9959aba3b5e308a567ade6b62da56c
ms.translationtype: MT
ms.contentlocale: id-ID
ms.lasthandoff: 08/22/2019
ms.locfileid: "36531362"
---
# <a name="verify-your-domain"></a><span data-ttu-id="1aff0-102">Verifikasi domain</span><span class="sxs-lookup"><span data-stu-id="1aff0-102">Verify your domain</span></span>

 <span data-ttu-id="1aff0-103">**Catatan mungkin belum diperbarui di Internet.**</span><span class="sxs-lookup"><span data-stu-id="1aff0-103">**The record probably hasn't updated across the Internet.**</span></span>
  
<span data-ttu-id="1aff0-104">Biasanya hanya membutuhkan waktu beberapa menit bagi kita untuk dapat melihat catatan baru, tapi kadang-kadang dapat mengambil selama beberapa jam.</span><span class="sxs-lookup"><span data-stu-id="1aff0-104">It typically only takes a few minutes for us to be able to see the new record, but occasionally it can take as long as a few hours.</span></span> 
  
- <span data-ttu-id="1aff0-105">Jika Anda telah menunggu yang lama sudah, periksa bahwa Anda menyalin dan menyisipkan nilai yang tepat ke TXT verifikasi catatan di host DNS Anda.</span><span class="sxs-lookup"><span data-stu-id="1aff0-105">If you've waited that long already, double-check that you've copied and pasted the exact value into the TXT verification record at your DNS host.</span></span> <span data-ttu-id="1aff0-106">Salah satu masalah umum tidak termasuk "MS =" bagian dari catatan.</span><span class="sxs-lookup"><span data-stu-id="1aff0-106">One common issue is not including the "MS=" part of the record.</span></span> <span data-ttu-id="1aff0-107">Kita perlu yang terlalu!</span><span class="sxs-lookup"><span data-stu-id="1aff0-107">We need that too!</span></span>

- <span data-ttu-id="1aff0-108">Di beberapa host DNS, Anda harus mengambil langkah ekstra untuk menyimpan file zona (mana DNS record disimpan) sehingga ini akan memperbarui seluruh Internet.</span><span class="sxs-lookup"><span data-stu-id="1aff0-108">At some DNS hosts, you have to take an extra step to save the zone file (where the DNS record is stored) so that it will update across the Internet.</span></span> <span data-ttu-id="1aff0-109">Pastikan Anda telah disimpan perubahan sehingga Office 365 dapat melihat dan memverifikasi catatan.</span><span class="sxs-lookup"><span data-stu-id="1aff0-109">Make sure you've saved your changes so Office 365 can see and verify the record.</span></span>
