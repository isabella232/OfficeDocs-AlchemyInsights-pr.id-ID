---
title: Tidak dapat menetapkan atau melihat kebijakan AllowSelfServicePurchase
ms.author: pebaum
author: pebaum
manager: mnirkhe
ms.audience: Admin
ms.topic: article
ROBOTS: NOINDEX, NOFOLLOW
localization_priority: Normal
ms.collection: Adm_O365
ms.custom:
- "9001212"
- "3526"
ms.openlocfilehash: a9b6e36e8034e71b3e72c49e3cc68a126ef97aca
ms.sourcegitcommit: cb9505f9eca032af3a4194c68d18c91789365690
ms.translationtype: MT
ms.contentlocale: id-ID
ms.lasthandoff: 02/16/2020
ms.locfileid: "42091718"
---
# <a name="unable-to-set-or-view-the-allowselfservicepurchase-policy"></a><span data-ttu-id="45711-102">Tidak dapat menetapkan atau melihat kebijakan AllowSelfServicePurchase</span><span class="sxs-lookup"><span data-stu-id="45711-102">Unable to set or view the AllowSelfServicePurchase policy</span></span>

<span data-ttu-id="45711-103">Ketika mencoba untuk menetapkan atau melihat kebijakan AllowSelfServicePurchase, Anda menerima pesan galat berikut:</span><span class="sxs-lookup"><span data-stu-id="45711-103">When attempting to set or view the AllowSelfServicePurchase policy, you receive the following error message:</span></span>

<span data-ttu-id="45711-104">*HandleError: gagal untuk mengambil kebijakan produk dengan PolicyId ' AllowSelfServicePurchase ', ErrorMessage-yang mendasari sambungan ditutup: galat tak terduga terjadi pada kirim.*</span><span class="sxs-lookup"><span data-stu-id="45711-104">*HandleError : Failed to retrieve product policy with PolicyId 'AllowSelfServicePurchase', ErrorMessage - The underlying connection was closed: An unexpected error occurred on a send.*</span></span>

<span data-ttu-id="45711-105">Hal ini mungkin karena versi lama Transport Layer Security (TLS).</span><span class="sxs-lookup"><span data-stu-id="45711-105">This may be due to an older version of Transport Layer Security (TLS).</span></span> <span data-ttu-id="45711-106">Untuk menyambungkan Layanan MSCommerce, Anda harus menggunakan TLS 1,2 atau yang lebih baru.</span><span class="sxs-lookup"><span data-stu-id="45711-106">To connect the MSCommerce service, you need to use TLS 1.2 or greater.</span></span>  

<span data-ttu-id="45711-107">Cobalah langkah berikut untuk mengaktifkan/menetapkan protokol TLS ke 1,2, verifikasi, dan coba lagi.</span><span class="sxs-lookup"><span data-stu-id="45711-107">Try the following steps to enable/set the TLS protocol to 1.2, verify, and retry.</span></span>
 1. <span data-ttu-id="45711-108">Pada PowerShell prompt perintah (PS C:\) masukkan perintah berikut ini untuk menetapkan protokol TLS ke versi 1,2:</span><span class="sxs-lookup"><span data-stu-id="45711-108">At the PowerShell command prompt (PS C:\) enter the following command to set the TLS protocol to version 1.2:</span></span>

    <span data-ttu-id="45711-109">\[Net. ServicePointManager]:: SecurityProtocol = \[net. SecurityProtocolType]:: Tls12</span><span class="sxs-lookup"><span data-stu-id="45711-109">\[Net.ServicePointManager]::SecurityProtocol = \[Net.SecurityProtocolType]::Tls12</span></span>

2. <span data-ttu-id="45711-110">Verifikasi protokol TLS yang digunakan, dengan perintah berikut:</span><span class="sxs-lookup"><span data-stu-id="45711-110">Verify the TLS protocol(s) in use, with the following command:</span></span>

    <span data-ttu-id="45711-111">\[Net. ServicePointManager]:: SecurityProtocol</span><span class="sxs-lookup"><span data-stu-id="45711-111">\[Net.ServicePointManager]::SecurityProtocol</span></span> 

3. <span data-ttu-id="45711-112">Coba lagi perintah Get atau update sesuai kebutuhan.</span><span class="sxs-lookup"><span data-stu-id="45711-112">Retry the Get or Update commands as needed.</span></span>

