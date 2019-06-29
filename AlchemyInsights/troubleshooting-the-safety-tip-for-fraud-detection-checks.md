---
title: Pemecahan masalah tip keselamatan untuk deteksi penipuan cek
ms.author: pebaum
author: pebaum
manager: mnirkhe
ms.date: 1/9/2019
ms.audience: ITPro
ms.topic: article
ms.prod: office-online-server
ROBOTS: NOINDEX, NOFOLLOW
localization_priority: Normal
ms.assetid: 96ebe3c5-66ea-4662-98b7-052c2181c2f3
ms.custom:
- "275"
- "3100004"
ms.openlocfilehash: ab7bd3ec66640d66e5f1ea7c1eeee0a1a9510241
ms.sourcegitcommit: 5fb7a4b28859690020efdea630d03e70cc0e6334
ms.translationtype: MT
ms.contentlocale: id-ID
ms.lasthandoff: 06/28/2019
ms.locfileid: "35353252"
---
# <a name="troubleshooting-the-safety-tip-for-fraud-detection-checks"></a><span data-ttu-id="e4e79-102">Pemecahan masalah tip keselamatan untuk deteksi penipuan cek</span><span class="sxs-lookup"><span data-stu-id="e4e79-102">Troubleshooting the safety tip for fraud detection checks</span></span>

<span data-ttu-id="e4e79-103">Jika Anda mendapatkan tip keselamatan yang mengatakan "pengirim gagal pemeriksaan deteksi penipuan kami dan tidak mungkin yang mereka tampak", kemudian pengirim gagal dalam mewariskan DKIM atau SPF otentikasi cek.</span><span class="sxs-lookup"><span data-stu-id="e4e79-103">If you are getting a safety tip that says "The sender failed our fraud detection checks and may not be who they appear to be", then the sender failed to pass either DKIM or SPF authentication checks.</span></span> <span data-ttu-id="e4e79-104">Metode terbaik untuk memecahkan masalah ini adalah untuk pengirim untuk mengotorisasi sendiri.</span><span class="sxs-lookup"><span data-stu-id="e4e79-104">The best method to resolve this is for the sender to authorize themselves.</span></span> <span data-ttu-id="e4e79-105">Jika pengirim mengirim atas nama Anda, Anda perlu wewenang mereka dengan menambahkan alamat IP pengirim ke record SPF Anda.</span><span class="sxs-lookup"><span data-stu-id="e4e79-105">If the sender is sending on your behalf, you need to authorize them by adding the sender's IP address to your SPF record.</span></span>
  
<span data-ttu-id="e4e79-106">Lihat [pemecahan masalah merah (mencurigakan) safety Tips untuk deteksi penipuan cek](https://blogs.msdn.microsoft.com/tzink/2016/11/02/troubleshooting-the-red-suspicious-safety-tip-for-fraud-detection-checks/) untuk info lebih lanjut.</span><span class="sxs-lookup"><span data-stu-id="e4e79-106">See [Troubleshooting the red (suspicious) safety tip for fraud detection checks](https://blogs.msdn.microsoft.com/tzink/2016/11/02/troubleshooting-the-red-suspicious-safety-tip-for-fraud-detection-checks/) for more info.</span></span>
  
<span data-ttu-id="e4e79-107">Berikut adalah beberapa link yang dapat membantu:</span><span class="sxs-lookup"><span data-stu-id="e4e79-107">Here are some other links that can help:</span></span>
  
- [<span data-ttu-id="e4e79-108">Bagaimana Office 365 menggunakan kerangka kebijakan pengirim (SPF) untuk mencegah spoofing</span><span class="sxs-lookup"><span data-stu-id="e4e79-108">How Office 365 uses sender policy framework (SPF) to prevent spoofing</span></span>](https://docs.microsoft.com/office365/SecurityCompliance/how-office-365-uses-spf-to-prevent-spoofing)

- [<span data-ttu-id="e4e79-109">Mengatur SPF di Office 365 untuk membantu mencegah spoofing</span><span class="sxs-lookup"><span data-stu-id="e4e79-109">Set up SPF in Office 365 to help prevent spoofing</span></span>](https://docs.microsoft.com/office365/SecurityCompliance/set-up-spf-in-office-365-to-help-prevent-spoofing)
