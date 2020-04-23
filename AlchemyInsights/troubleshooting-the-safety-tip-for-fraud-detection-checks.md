---
title: Mengatasi masalah tip keselamatan untuk pemeriksaan pendeteksian penipuan
ms.author: pebaum
author: pebaum
manager: mnirkhe
ms.date: 04/21/2020
ms.audience: ITPro
ms.topic: article
ms.prod: office-online-server
ROBOTS: NOINDEX, NOFOLLOW
localization_priority: Normal
ms.assetid: 96ebe3c5-66ea-4662-98b7-052c2181c2f3
ms.custom:
- "275"
- "3100004"
ms.openlocfilehash: 61159391f7a9876750cd7fefc40c54054fb9bec9
ms.sourcegitcommit: 631cbb5f03e5371f0995e976536d24e9d13746c3
ms.translationtype: MT
ms.contentlocale: id-ID
ms.lasthandoff: 04/22/2020
ms.locfileid: "43759515"
---
# <a name="troubleshooting-the-safety-tip-for-fraud-detection-checks"></a><span data-ttu-id="a86d1-102">Mengatasi masalah tip keselamatan untuk pemeriksaan pendeteksian penipuan</span><span class="sxs-lookup"><span data-stu-id="a86d1-102">Troubleshooting the safety tip for fraud detection checks</span></span>

<span data-ttu-id="a86d1-103">Jika Anda mendapatkan tip keselamatan yang berbunyi "pengirim gagal memeriksa deteksi penipuan kami dan mungkin tidak menjadi siapa mereka tampaknya", maka pengirim gagal untuk lulus baik DKIM atau SPF otentikasi cek.</span><span class="sxs-lookup"><span data-stu-id="a86d1-103">If you are getting a safety tip that says "The sender failed our fraud detection checks and may not be who they appear to be", then the sender failed to pass either DKIM or SPF authentication checks.</span></span> <span data-ttu-id="a86d1-104">Metode terbaik untuk menyelesaikan ini adalah untuk pengirim untuk mengotorisasi diri mereka sendiri.</span><span class="sxs-lookup"><span data-stu-id="a86d1-104">The best method to resolve this is for the sender to authorize themselves.</span></span> <span data-ttu-id="a86d1-105">Jika pengirim mengirimkan atas nama Anda, Anda perlu mengotorisasi mereka dengan menambahkan alamat IP pengirim ke data SPF.</span><span class="sxs-lookup"><span data-stu-id="a86d1-105">If the sender is sending on your behalf, you need to authorize them by adding the sender's IP address to your SPF record.</span></span>
  
<span data-ttu-id="a86d1-106">Lihat [mengatasi masalah Tips keamanan merah (mencurigakan) untuk pemeriksaan deteksi penipuan](https://blogs.msdn.microsoft.com/tzink/2016/11/02/troubleshooting-the-red-suspicious-safety-tip-for-fraud-detection-checks/) untuk info lebih lanjut.</span><span class="sxs-lookup"><span data-stu-id="a86d1-106">See [Troubleshooting the red (suspicious) safety tip for fraud detection checks](https://blogs.msdn.microsoft.com/tzink/2016/11/02/troubleshooting-the-red-suspicious-safety-tip-for-fraud-detection-checks/) for more info.</span></span>
  
<span data-ttu-id="a86d1-107">Berikut adalah beberapa link lain yang dapat membantu:</span><span class="sxs-lookup"><span data-stu-id="a86d1-107">Here are some other links that can help:</span></span>
  
- [<span data-ttu-id="a86d1-108">Bagaimana Microsoft menggunakan kerangka kebijakan pengirim (SPF) untuk mencegah spoofing</span><span class="sxs-lookup"><span data-stu-id="a86d1-108">How Microsoft uses sender policy framework (SPF) to prevent spoofing</span></span>](https://docs.microsoft.com/office365/SecurityCompliance/how-office-365-uses-spf-to-prevent-spoofing)

- [<span data-ttu-id="a86d1-109">Menyiapkan SPF untuk membantu mencegah spoofing</span><span class="sxs-lookup"><span data-stu-id="a86d1-109">Set up SPF to help prevent spoofing</span></span>](https://docs.microsoft.com/office365/SecurityCompliance/set-up-spf-in-office-365-to-help-prevent-spoofing)
