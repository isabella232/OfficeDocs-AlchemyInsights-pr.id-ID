---
title: Memverifikasi domain Anda
ms.author: pebaum
author: pebaum
manager: mnirkhe
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
ms.openlocfilehash: d30f9b51c0164acd126f214a581ad6cec5eec04e
ms.sourcegitcommit: c6692ce0fa1358ec3529e59ca0ecdfdea4cdc759
ms.translationtype: MT
ms.contentlocale: id-ID
ms.lasthandoff: 09/14/2020
ms.locfileid: "47734309"
---
# <a name="verify-your-domain"></a><span data-ttu-id="89a84-102">Memverifikasi domain Anda</span><span class="sxs-lookup"><span data-stu-id="89a84-102">Verify your domain</span></span>

 <span data-ttu-id="89a84-103">**Catatan mungkin belum diperbarui di seluruh internet.**</span><span class="sxs-lookup"><span data-stu-id="89a84-103">**The record probably hasn't updated across the Internet.**</span></span>
  
<span data-ttu-id="89a84-104">Biasanya hanya memerlukan beberapa menit agar kami dapat melihat catatan baru, tapi terkadang dapat memakan waktu selama beberapa jam.</span><span class="sxs-lookup"><span data-stu-id="89a84-104">It typically only takes a few minutes for us to be able to see the new record, but occasionally it can take as long as a few hours.</span></span> 
  
- <span data-ttu-id="89a84-105">Jika sudah lama menunggu, periksa ulang Apakah Anda telah menyalin dan menempelkan nilai persis ke dalam catatan verifikasi TXT di host DNS Anda.</span><span class="sxs-lookup"><span data-stu-id="89a84-105">If you've waited that long already, double-check that you've copied and pasted the exact value into the TXT verification record at your DNS host.</span></span> <span data-ttu-id="89a84-106">Salah satu masalah umum tidak termasuk "MS =" bagian dari catatan.</span><span class="sxs-lookup"><span data-stu-id="89a84-106">One common issue is not including the "MS=" part of the record.</span></span> <span data-ttu-id="89a84-107">Kami juga membutuhkannya!</span><span class="sxs-lookup"><span data-stu-id="89a84-107">We need that too!</span></span>

- <span data-ttu-id="89a84-108">Di beberapa host DNS, Anda harus mengambil langkah tambahan untuk menyimpan file zona (tempat catatan DNS disimpan) sehingga akan diperbarui di seluruh internet.</span><span class="sxs-lookup"><span data-stu-id="89a84-108">At some DNS hosts, you have to take an extra step to save the zone file (where the DNS record is stored) so that it will update across the Internet.</span></span> <span data-ttu-id="89a84-109">Pastikan Anda telah menyimpan perubahan Anda sehingga Microsoft bisa melihat dan memverifikasi catatan.</span><span class="sxs-lookup"><span data-stu-id="89a84-109">Make sure you've saved your changes so Microsoft can see and verify the record.</span></span>
