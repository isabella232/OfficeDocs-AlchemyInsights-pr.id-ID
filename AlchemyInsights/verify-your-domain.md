---
title: Memverifikasi domain Anda
ms.author: pebaum
author: pebaum
manager: mnirkhe
ms.date: 04/21/2020
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
ms.openlocfilehash: 2c4d8e075d2cf7214b5ef005b856daf7fb0ed53c
ms.sourcegitcommit: 55eff703a17e500681d8fa6a87eb067019ade3cc
ms.translationtype: MT
ms.contentlocale: id-ID
ms.lasthandoff: 04/22/2020
ms.locfileid: "43710446"
---
# <a name="verify-your-domain"></a><span data-ttu-id="14383-102">Memverifikasi domain Anda</span><span class="sxs-lookup"><span data-stu-id="14383-102">Verify your domain</span></span>

 <span data-ttu-id="14383-103">**Catatan mungkin belum diperbarui di internet.**</span><span class="sxs-lookup"><span data-stu-id="14383-103">**The record probably hasn't updated across the Internet.**</span></span>
  
<span data-ttu-id="14383-104">Ini biasanya hanya membutuhkan waktu beberapa menit bagi kita untuk dapat melihat rekor baru, tapi terkadang dapat memakan waktu selama beberapa jam.</span><span class="sxs-lookup"><span data-stu-id="14383-104">It typically only takes a few minutes for us to be able to see the new record, but occasionally it can take as long as a few hours.</span></span> 
  
- <span data-ttu-id="14383-105">Jika sudah lama menunggu, periksa bahwa Anda telah menyalin dan menempelkan nilai yang tepat ke dalam data verifikasi TXT di host DNS Anda.</span><span class="sxs-lookup"><span data-stu-id="14383-105">If you've waited that long already, double-check that you've copied and pasted the exact value into the TXT verification record at your DNS host.</span></span> <span data-ttu-id="14383-106">Salah satu masalah umum adalah tidak termasuk "MS =" bagian dari catatan.</span><span class="sxs-lookup"><span data-stu-id="14383-106">One common issue is not including the "MS=" part of the record.</span></span> <span data-ttu-id="14383-107">Kita membutuhkan itu juga!</span><span class="sxs-lookup"><span data-stu-id="14383-107">We need that too!</span></span>

- <span data-ttu-id="14383-108">Pada beberapa host DNS, Anda harus mengambil langkah ekstra untuk menyimpan file zona (di mana catatan DNS disimpan) sehingga akan diperbarui di internet.</span><span class="sxs-lookup"><span data-stu-id="14383-108">At some DNS hosts, you have to take an extra step to save the zone file (where the DNS record is stored) so that it will update across the Internet.</span></span> <span data-ttu-id="14383-109">Pastikan Anda telah menyimpan perubahan sehingga Microsoft dapat melihat dan memverifikasi rekaman.</span><span class="sxs-lookup"><span data-stu-id="14383-109">Make sure you've saved your changes so Microsoft can see and verify the record.</span></span>
