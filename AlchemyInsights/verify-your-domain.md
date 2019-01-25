---
title: Verifikasi domain
ms.author: pebaum
author: pebaum
manager: mnirkhe
ms.date: 4/5/2018
ms.audience: Admin
ms.topic: article
ROBOTS: NOINDEX, NOFOLLOW
localization_priority: Priority
ms.collection: Adm_O365
ms.custom: Adm_O365
ms.assetid: 81fd176b-3d67-4e52-9ab8-d36602412734
ms.openlocfilehash: d37cdae616fabd2813dc7c8074e94b05f0391d20
ms.sourcegitcommit: e2864efcfb493b6e46b662b746661a61232bdba7
ms.translationtype: MT
ms.contentlocale: id-ID
ms.lasthandoff: 01/24/2019
ms.locfileid: "29475072"
---
# <a name="verify-your-domain"></a><span data-ttu-id="abadb-102">Verifikasi domain</span><span class="sxs-lookup"><span data-stu-id="abadb-102">Verify your domain</span></span>

 <span data-ttu-id="abadb-103">**Catatan mungkin belum diperbarui di Internet.**</span><span class="sxs-lookup"><span data-stu-id="abadb-103">**The record probably hasn't updated across the Internet.**</span></span>
  
<span data-ttu-id="abadb-104">Biasanya hanya membutuhkan waktu beberapa menit bagi kita untuk dapat melihat catatan baru, tapi kadang-kadang dapat mengambil selama beberapa jam.</span><span class="sxs-lookup"><span data-stu-id="abadb-104">It typically only takes a few minutes for us to be able to see the new record, but occasionally it can take as long as a few hours.</span></span> 
  
- <span data-ttu-id="abadb-p101">Jika Anda telah menunggu yang lama sudah, periksa bahwa Anda menyalin dan menyisipkan nilai yang tepat ke TXT verifikasi catatan di host DNS Anda. Salah satu masalah umum tidak termasuk "MS =" bagian dari catatan. Kita perlu yang terlalu!</span><span class="sxs-lookup"><span data-stu-id="abadb-p101">If you've waited that long already, double-check that you've copied and pasted the exact value into the TXT verification record at your DNS host. One common issue is not including the "MS=" part of the record. We need that too!</span></span>
    
- <span data-ttu-id="abadb-p102">Di beberapa host DNS, Anda harus mengambil langkah ekstra untuk menyimpan file zona (mana DNS record disimpan) sehingga ini akan memperbarui seluruh Internet. Pastikan Anda telah disimpan perubahan sehingga Office 365 dapat melihat dan memverifikasi catatan.</span><span class="sxs-lookup"><span data-stu-id="abadb-p102">At some DNS hosts, you have to take an extra step to save the zone file (where the DNS record is stored) so that it will update across the Internet. Make sure you've saved your changes so Office 365 can see and verify the record.</span></span>
    

