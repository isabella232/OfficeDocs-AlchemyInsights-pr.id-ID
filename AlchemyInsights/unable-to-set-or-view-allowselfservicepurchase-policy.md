---
title: Tidak dapat mengatur atau menampilkan kebijakan AllowSelfServicePurchase
ms.author: pebaum
author: pebaum
manager: mnirkhe
ms.audience: Admin
ms.topic: article
ms.service: o365-administration
ROBOTS: NOINDEX, NOFOLLOW
localization_priority: Normal
ms.collection: Adm_O365
ms.custom:
- "9001212"
- "3526"
ms.openlocfilehash: 5ec16b3071f95ef52af2771e95137116222a3c5b
ms.sourcegitcommit: c6692ce0fa1358ec3529e59ca0ecdfdea4cdc759
ms.translationtype: MT
ms.contentlocale: id-ID
ms.lasthandoff: 09/14/2020
ms.locfileid: "47735202"
---
# <a name="unable-to-set-or-view-the-allowselfservicepurchase-policy"></a><span data-ttu-id="56b33-102">Tidak dapat mengatur atau menampilkan kebijakan AllowSelfServicePurchase</span><span class="sxs-lookup"><span data-stu-id="56b33-102">Unable to set or view the AllowSelfServicePurchase policy</span></span>

<span data-ttu-id="56b33-103">Saat mencoba mengatur atau menampilkan kebijakan AllowSelfServicePurchase, Anda menerima pesan kesalahan berikut:</span><span class="sxs-lookup"><span data-stu-id="56b33-103">When attempting to set or view the AllowSelfServicePurchase policy, you receive the following error message:</span></span>

<span data-ttu-id="56b33-104">*Saperkesalahan: gagal untuk mengambil kebijakan produk dengan PolicyId ' AllowSelfServicePurchase ', ErrorMessage-The underlying Connection ditutup: kesalahan yang tidak diharapkan terjadi pada kirim.*</span><span class="sxs-lookup"><span data-stu-id="56b33-104">*HandleError : Failed to retrieve product policy with PolicyId 'AllowSelfServicePurchase', ErrorMessage - The underlying connection was closed: An unexpected error occurred on a send.*</span></span>

<span data-ttu-id="56b33-105">Ini mungkin karena versi lama Transport Layer Security (TLS).</span><span class="sxs-lookup"><span data-stu-id="56b33-105">This may be due to an older version of Transport Layer Security (TLS).</span></span> <span data-ttu-id="56b33-106">Untuk menyambungkan Layanan MSCommerce, Anda harus menggunakan TLS 1,2 atau yang lebih baru.</span><span class="sxs-lookup"><span data-stu-id="56b33-106">To connect the MSCommerce service, you need to use TLS 1.2 or greater.</span></span>  

<span data-ttu-id="56b33-107">Cobalah langkah-langkah berikut untuk mengaktifkan/mengatur protokol TLS ke 1,2, memverifikasi, dan coba lagi.</span><span class="sxs-lookup"><span data-stu-id="56b33-107">Try the following steps to enable/set the TLS protocol to 1.2, verify, and retry.</span></span>
 1. <span data-ttu-id="56b33-108">Pada prompt perintah PowerShell (PS C: \) Masukkan perintah berikut ini untuk mengatur protokol TLS ke versi 1,2:</span><span class="sxs-lookup"><span data-stu-id="56b33-108">At the PowerShell command prompt (PS C:\) enter the following command to set the TLS protocol to version 1.2:</span></span>

    `[Net.ServicePointManager]::SecurityProtocol = [Net.SecurityProtocolType]::Tls12`

2. <span data-ttu-id="56b33-109">Verifikasi protokol TLS yang digunakan, dengan perintah berikut ini:</span><span class="sxs-lookup"><span data-stu-id="56b33-109">Verify the TLS protocol(s) in use, with the following command:</span></span>

    `[Net.ServicePointManager]::SecurityProtocol` 

3. <span data-ttu-id="56b33-110">Coba lagi perintah Dapatkan atau Perbarui sesuai keperluan.</span><span class="sxs-lookup"><span data-stu-id="56b33-110">Retry the Get or Update commands as needed.</span></span>

