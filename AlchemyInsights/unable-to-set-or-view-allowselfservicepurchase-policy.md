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
ms.openlocfilehash: 587a05cccbc71a970d4bd7723bff0df0c3b64ccc
ms.sourcegitcommit: 2a9d059262c07c33f9a740b3da4e6e3366b2f925
ms.translationtype: MT
ms.contentlocale: id-ID
ms.lasthandoff: 02/20/2020
ms.locfileid: "42158564"
---
# <a name="unable-to-set-or-view-the-allowselfservicepurchase-policy"></a><span data-ttu-id="00ae4-102">Tidak dapat menetapkan atau melihat kebijakan AllowSelfServicePurchase</span><span class="sxs-lookup"><span data-stu-id="00ae4-102">Unable to set or view the AllowSelfServicePurchase policy</span></span>

<span data-ttu-id="00ae4-103">Ketika mencoba untuk menetapkan atau melihat kebijakan AllowSelfServicePurchase, Anda menerima pesan galat berikut:</span><span class="sxs-lookup"><span data-stu-id="00ae4-103">When attempting to set or view the AllowSelfServicePurchase policy, you receive the following error message:</span></span>

<span data-ttu-id="00ae4-104">*HandleError: gagal untuk mengambil kebijakan produk dengan PolicyId ' AllowSelfServicePurchase ', ErrorMessage-yang mendasari sambungan ditutup: galat tak terduga terjadi pada kirim.*</span><span class="sxs-lookup"><span data-stu-id="00ae4-104">*HandleError : Failed to retrieve product policy with PolicyId 'AllowSelfServicePurchase', ErrorMessage - The underlying connection was closed: An unexpected error occurred on a send.*</span></span>

<span data-ttu-id="00ae4-105">Hal ini mungkin karena versi lama Transport Layer Security (TLS).</span><span class="sxs-lookup"><span data-stu-id="00ae4-105">This may be due to an older version of Transport Layer Security (TLS).</span></span> <span data-ttu-id="00ae4-106">Untuk menyambungkan Layanan MSCommerce, Anda harus menggunakan TLS 1,2 atau yang lebih baru.</span><span class="sxs-lookup"><span data-stu-id="00ae4-106">To connect the MSCommerce service, you need to use TLS 1.2 or greater.</span></span>  

<span data-ttu-id="00ae4-107">Cobalah langkah berikut untuk mengaktifkan/menetapkan protokol TLS ke 1,2, verifikasi, dan coba lagi.</span><span class="sxs-lookup"><span data-stu-id="00ae4-107">Try the following steps to enable/set the TLS protocol to 1.2, verify, and retry.</span></span>
 1. <span data-ttu-id="00ae4-108">Pada PowerShell prompt perintah (PS C:\) masukkan perintah berikut ini untuk menetapkan protokol TLS ke versi 1,2:</span><span class="sxs-lookup"><span data-stu-id="00ae4-108">At the PowerShell command prompt (PS C:\) enter the following command to set the TLS protocol to version 1.2:</span></span>

    `[Net.ServicePointManager]::SecurityProtocol = [Net.SecurityProtocolType]::Tls12`

2. <span data-ttu-id="00ae4-109">Verifikasi protokol TLS yang digunakan, dengan perintah berikut:</span><span class="sxs-lookup"><span data-stu-id="00ae4-109">Verify the TLS protocol(s) in use, with the following command:</span></span>

    `[Net.ServicePointManager]::SecurityProtocol` 

3. <span data-ttu-id="00ae4-110">Coba lagi perintah Get atau update sesuai kebutuhan.</span><span class="sxs-lookup"><span data-stu-id="00ae4-110">Retry the Get or Update commands as needed.</span></span>

