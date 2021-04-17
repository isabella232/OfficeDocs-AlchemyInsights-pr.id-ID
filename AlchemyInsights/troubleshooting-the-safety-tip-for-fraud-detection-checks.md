---
title: Memecahkan masalah tips keamanan untuk pemeriksaan deteksi penipuan
ms.author: pebaum
author: pebaum
manager: scotv
ms.date: 04/21/2020
ms.audience: ITPro
ms.topic: article
ms.service: o365-administration
ROBOTS: NOINDEX, NOFOLLOW
localization_priority: Normal
ms.assetid: 96ebe3c5-66ea-4662-98b7-052c2181c2f3
ms.custom:
- "275"
- "3100004"
ms.openlocfilehash: 85faa0086935fb7e7132ee9fdced546bafdb344c
ms.sourcegitcommit: 8bc60ec34bc1e40685e3976576e04a2623f63a7c
ms.translationtype: MT
ms.contentlocale: id-ID
ms.lasthandoff: 04/15/2021
ms.locfileid: "51834734"
---
# <a name="troubleshooting-the-safety-tip-for-fraud-detection-checks"></a><span data-ttu-id="5d689-102">Memecahkan masalah tips keamanan untuk pemeriksaan deteksi penipuan</span><span class="sxs-lookup"><span data-stu-id="5d689-102">Troubleshooting the safety tip for fraud detection checks</span></span>

<span data-ttu-id="5d689-103">Jika Anda mendapatkan tips pengamanan yang mengatakan "Pengirim gagal memeriksa pendeteksian penipuan kami dan mungkin bukan siapa mereka yang ditampilkan", pengirim gagal melewati pemeriksaan autentikasi DKIM atau SPF.</span><span class="sxs-lookup"><span data-stu-id="5d689-103">If you are getting a safety tip that says "The sender failed our fraud detection checks and may not be who they appear to be", then the sender failed to pass either DKIM or SPF authentication checks.</span></span> <span data-ttu-id="5d689-104">Metode terbaik untuk mengatasi masalah ini adalah pengirim dapat mengotorisasi dirinya sendiri.</span><span class="sxs-lookup"><span data-stu-id="5d689-104">The best method to resolve this is for the sender to authorize themselves.</span></span> <span data-ttu-id="5d689-105">Jika pengirim mengirim atas nama Anda, Anda perlu mengotorisasi mereka dengan menambahkan alamat IP pengirim ke catatan SPF Anda.</span><span class="sxs-lookup"><span data-stu-id="5d689-105">If the sender is sending on your behalf, you need to authorize them by adding the sender's IP address to your SPF record.</span></span>
  
<span data-ttu-id="5d689-106">Lihat [Memecahkan masalah tips keamanan berwarna merah (mencurigakan) untuk pemeriksaan deteksi](https://blogs.msdn.microsoft.com/tzink/2016/11/02/troubleshooting-the-red-suspicious-safety-tip-for-fraud-detection-checks/) penipuan untuk informasi selengkapnya.</span><span class="sxs-lookup"><span data-stu-id="5d689-106">See [Troubleshooting the red (suspicious) safety tip for fraud detection checks](https://blogs.msdn.microsoft.com/tzink/2016/11/02/troubleshooting-the-red-suspicious-safety-tip-for-fraud-detection-checks/) for more info.</span></span>
  
<span data-ttu-id="5d689-107">Berikut adalah beberapa tautan lain yang dapat membantu:</span><span class="sxs-lookup"><span data-stu-id="5d689-107">Here are some other links that can help:</span></span>
  
- [<span data-ttu-id="5d689-108">Bagaimana Microsoft menggunakan kerangka kebijakan pengirim (SPF) untuk mencegah spoofing</span><span class="sxs-lookup"><span data-stu-id="5d689-108">How Microsoft uses sender policy framework (SPF) to prevent spoofing</span></span>](https://docs.microsoft.com/microsoft-365/security/office-365-security/how-office-365-uses-spf-to-prevent-spoofing)

- [<span data-ttu-id="5d689-109">Menyiapkan SPF untuk membantu mencegah spoofing</span><span class="sxs-lookup"><span data-stu-id="5d689-109">Set up SPF to help prevent spoofing</span></span>](https://docs.microsoft.com/microsoft-365/security/office-365-security/set-up-spf-in-office-365-to-help-prevent-spoofing)
