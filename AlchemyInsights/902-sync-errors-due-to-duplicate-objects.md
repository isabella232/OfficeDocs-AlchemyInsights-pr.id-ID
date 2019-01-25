---
title: 902 (sync kesalahan karena duplikat objek)
ms.author: chrisda
author: chrisda
manager: serdars
ms.date: 5/30/2018
ms.audience: ITPro
ms.topic: article
ROBOTS: NOINDEX, NOFOLLOW
localization_priority: Priority
ms.assetid: 9d9277a5-c825-4512-8d54-7138b2ee0c40
ms.openlocfilehash: f8db233167a5e2b2ef7290438b8e6d92d0dccb1e
ms.sourcegitcommit: e2864efcfb493b6e46b662b746661a61232bdba7
ms.translationtype: MT
ms.contentlocale: id-ID
ms.lasthandoff: 01/24/2019
ms.locfileid: "29475155"
---
# <a name="sync-errors-due-to-duplicate-objects"></a><span data-ttu-id="1928b-102">Galat sinkronisasi karena duplikat objek</span><span class="sxs-lookup"><span data-stu-id="1928b-102">Sync errors due to duplicate objects</span></span>

<span data-ttu-id="1928b-103">Anda mungkin menerima salah satu pesan galat berikut ketika selesai sinkronisasi direktori:</span><span class="sxs-lookup"><span data-stu-id="1928b-103">You might receive one of the following error messages when directory synchronization finishes:</span></span>
  
- <span data-ttu-id="1928b-104">Tidak dapat memperbarui objek ini di Microsoft Online Services karena atribut berikut terkait dengan objek ini memiliki nilai yang sudah mungkin terkait dengan objek lain dalam direktori lokal Anda.</span><span class="sxs-lookup"><span data-stu-id="1928b-104">Unable to update this object in Microsoft Online Services because the following attributes associated with this object have values that may already be associated with another object in your local directory.</span></span>
    
- <span data-ttu-id="1928b-105">Sebuah objek disinkronisasi dengan alamat proxy yang sama sudah ada di direktori Layanan Online Microsoft.</span><span class="sxs-lookup"><span data-stu-id="1928b-105">A synchronized object with the same proxy address already exists in your Microsoft Online Services directory.</span></span>
    
- <span data-ttu-id="1928b-106">Tidak dapat memperbarui objek ini karena atribut berikut terkait dengan objek ini memiliki nilai-nilai yang sudah mungkin terkait dengan objek lain di layanan direktori lokal Anda: UserPrincipalName.</span><span class="sxs-lookup"><span data-stu-id="1928b-106">Unable to update this object because the following attributes associated with this object have values that may already be associated with another object in your local directory services: UserPrincipalName.</span></span>
    
<span data-ttu-id="1928b-107">Untuk mengidentifikasi dan memperbaiki masalah, download dan menjalankan [Alat perbaikan IdFix DirSync kesalahan](https://www.microsoft.com/download/details.aspx?id=36832).</span><span class="sxs-lookup"><span data-stu-id="1928b-107">To identify and fix the issue, download and run the [IdFix DirSync Error Remediation Tool](https://www.microsoft.com/download/details.aspx?id=36832).</span></span>
  
<span data-ttu-id="1928b-108">Untuk informasi lebih lanjut, lihat [KB2647098](https://support.microsoft.com/help/2647098/duplicate-or-invalid-attributes-prevent-directory-synchronization-in-o).</span><span class="sxs-lookup"><span data-stu-id="1928b-108">For more information, see [KB2647098](https://support.microsoft.com/help/2647098/duplicate-or-invalid-attributes-prevent-directory-synchronization-in-o).</span></span>
  

