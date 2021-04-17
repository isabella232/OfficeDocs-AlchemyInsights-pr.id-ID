---
title: Tidak dapat mengatur atau menampilkan kebijakan AllowSelfServicePurchase
ms.author: pebaum
author: pebaum
manager: scotv
ms.audience: Admin
ms.topic: article
ms.service: o365-administration
ROBOTS: NOINDEX, NOFOLLOW
localization_priority: Normal
ms.collection: Adm_O365
ms.custom:
- "9001212"
- "3526"
ms.openlocfilehash: 8dac2bdc20905cf37fc30317d9b371bfd755f452
ms.sourcegitcommit: 8bc60ec34bc1e40685e3976576e04a2623f63a7c
ms.translationtype: MT
ms.contentlocale: id-ID
ms.lasthandoff: 04/15/2021
ms.locfileid: "51826094"
---
# <a name="unable-to-set-or-view-the-allowselfservicepurchase-policy"></a><span data-ttu-id="56729-102">Tidak dapat mengatur atau menampilkan kebijakan AllowSelfServicePurchase</span><span class="sxs-lookup"><span data-stu-id="56729-102">Unable to set or view the AllowSelfServicePurchase policy</span></span>

<span data-ttu-id="56729-103">Ketika mencoba mengatur atau menampilkan kebijakan AllowSelfServicePurchase, Anda menerima pesan kesalahan berikut:</span><span class="sxs-lookup"><span data-stu-id="56729-103">When attempting to set or view the AllowSelfServicePurchase policy, you receive the following error message:</span></span>

<span data-ttu-id="56729-104">*HandleError: Gagal mendapatkan kebijakan produk dengan PolicyId 'AllowSelfServicePurchase', ErrorMessage - Koneksi yang mendasari ditutup: Terjadi kesalahan yang tidak terduga pada pengiriman.*</span><span class="sxs-lookup"><span data-stu-id="56729-104">*HandleError : Failed to retrieve product policy with PolicyId 'AllowSelfServicePurchase', ErrorMessage - The underlying connection was closed: An unexpected error occurred on a send.*</span></span>

<span data-ttu-id="56729-105">Hal ini mungkin terjadi karena versi lama Transport Layer Security (TLS).</span><span class="sxs-lookup"><span data-stu-id="56729-105">This may be due to an older version of Transport Layer Security (TLS).</span></span> <span data-ttu-id="56729-106">Untuk menyambungkan layanan MSCommerce, Anda perlu menggunakan TLS 1.2 atau yang lebih besar.</span><span class="sxs-lookup"><span data-stu-id="56729-106">To connect the MSCommerce service, you need to use TLS 1.2 or greater.</span></span>  

<span data-ttu-id="56729-107">Coba langkah-langkah berikut untuk mengaktifkan/mengatur protokol TLS ke 1.2, verifikasi, dan coba lagi.</span><span class="sxs-lookup"><span data-stu-id="56729-107">Try the following steps to enable/set the TLS protocol to 1.2, verify, and retry.</span></span>
 1. <span data-ttu-id="56729-108">Di prompt perintah PowerShell (PS C: \) masukkan perintah berikut ini untuk mengatur protokol TLS ke versi 1.2:</span><span class="sxs-lookup"><span data-stu-id="56729-108">At the PowerShell command prompt (PS C:\) enter the following command to set the TLS protocol to version 1.2:</span></span>

    `[Net.ServicePointManager]::SecurityProtocol = [Net.SecurityProtocolType]::Tls12`

2. <span data-ttu-id="56729-109">Verifikasi protokol TLS yang digunakan, dengan perintah berikut ini:</span><span class="sxs-lookup"><span data-stu-id="56729-109">Verify the TLS protocol(s) in use, with the following command:</span></span>

    `[Net.ServicePointManager]::SecurityProtocol` 

3. <span data-ttu-id="56729-110">Coba lagi perintah Dapatkan atau Perbarui sebagaimana diperlukan.</span><span class="sxs-lookup"><span data-stu-id="56729-110">Retry the Get or Update commands as needed.</span></span>

