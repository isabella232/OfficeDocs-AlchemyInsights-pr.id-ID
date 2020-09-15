---
title: Pemecahan masalah Tips keamanan untuk pemeriksaan deteksi penipuan
ms.author: pebaum
author: pebaum
manager: mnirkhe
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
ms.openlocfilehash: e42b498070bf5d9bfc36110667da8cc0fd431524
ms.sourcegitcommit: c6692ce0fa1358ec3529e59ca0ecdfdea4cdc759
ms.translationtype: MT
ms.contentlocale: id-ID
ms.lasthandoff: 09/14/2020
ms.locfileid: "47658413"
---
# <a name="troubleshooting-the-safety-tip-for-fraud-detection-checks"></a><span data-ttu-id="27dbf-102">Pemecahan masalah Tips keamanan untuk pemeriksaan deteksi penipuan</span><span class="sxs-lookup"><span data-stu-id="27dbf-102">Troubleshooting the safety tip for fraud detection checks</span></span>

<span data-ttu-id="27dbf-103">Jika Anda mendapatkan tips keselamatan yang mengatakan "pengirim gagal memeriksa deteksi penipuan kami dan mungkin bukan sebagai siapa mereka terlihat", maka pengirim gagal melewati pemeriksaan autentikasi DKIM atau SPF.</span><span class="sxs-lookup"><span data-stu-id="27dbf-103">If you are getting a safety tip that says "The sender failed our fraud detection checks and may not be who they appear to be", then the sender failed to pass either DKIM or SPF authentication checks.</span></span> <span data-ttu-id="27dbf-104">Metode terbaik untuk mengatasi masalah ini adalah agar pengirim mengotorisasi dirinya.</span><span class="sxs-lookup"><span data-stu-id="27dbf-104">The best method to resolve this is for the sender to authorize themselves.</span></span> <span data-ttu-id="27dbf-105">Jika pengirim mengirim atas nama Anda, Anda perlu mengotorisasi mereka dengan menambahkan alamat IP pengirim ke catatan SPF Anda.</span><span class="sxs-lookup"><span data-stu-id="27dbf-105">If the sender is sending on your behalf, you need to authorize them by adding the sender's IP address to your SPF record.</span></span>
  
<span data-ttu-id="27dbf-106">Lihat [pemecahan masalah Tips keamanan berwarna merah (mencurigakan) untuk pemeriksaan deteksi penipuan](https://blogs.msdn.microsoft.com/tzink/2016/11/02/troubleshooting-the-red-suspicious-safety-tip-for-fraud-detection-checks/) untuk informasi selengkapnya.</span><span class="sxs-lookup"><span data-stu-id="27dbf-106">See [Troubleshooting the red (suspicious) safety tip for fraud detection checks](https://blogs.msdn.microsoft.com/tzink/2016/11/02/troubleshooting-the-red-suspicious-safety-tip-for-fraud-detection-checks/) for more info.</span></span>
  
<span data-ttu-id="27dbf-107">Berikut adalah beberapa tautan lain yang dapat membantu:</span><span class="sxs-lookup"><span data-stu-id="27dbf-107">Here are some other links that can help:</span></span>
  
- [<span data-ttu-id="27dbf-108">Cara Microsoft menggunakan Sender Policy Framework (SPF) untuk mencegah spoofing</span><span class="sxs-lookup"><span data-stu-id="27dbf-108">How Microsoft uses sender policy framework (SPF) to prevent spoofing</span></span>](https://docs.microsoft.com/microsoft-365/security/office-365-security/how-office-365-uses-spf-to-prevent-spoofing)

- [<span data-ttu-id="27dbf-109">Menyiapkan SPF untuk membantu mencegah spoofing</span><span class="sxs-lookup"><span data-stu-id="27dbf-109">Set up SPF to help prevent spoofing</span></span>](https://docs.microsoft.com/microsoft-365/security/office-365-security/set-up-spf-in-office-365-to-help-prevent-spoofing)
