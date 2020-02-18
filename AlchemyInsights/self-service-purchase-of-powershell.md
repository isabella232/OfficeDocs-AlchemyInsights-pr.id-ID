---
title: Pembelian layanan mandiri dari PowerShell
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
- "3516"
ms.openlocfilehash: 5e47e08e3309b3d58908e10ee06021da00f230bb
ms.sourcegitcommit: cb9505f9eca032af3a4194c68d18c91789365690
ms.translationtype: MT
ms.contentlocale: id-ID
ms.lasthandoff: 02/16/2020
ms.locfileid: "42091717"
---
# <a name="self-service-purchase-of-powershell"></a><span data-ttu-id="9e311-102">Pembelian layanan mandiri dari PowerShell</span><span class="sxs-lookup"><span data-stu-id="9e311-102">Self-service purchase of PowerShell</span></span>

<span data-ttu-id="9e311-103">Untuk menggunakan modul MSCommerce PowerShell, Anda harus menginstalnya pada perangkat Windows 10 dengan TLS 1,2 (izin administrator lokal diperlukan).</span><span class="sxs-lookup"><span data-stu-id="9e311-103">To use the MSCommerce PowerShell module, you need to install it on a Windows 10 device with TLS 1.2 (local administrator permissions required).</span></span>  <span data-ttu-id="9e311-104">Impor dan Sambungkan ke modul MSCommerce.</span><span class="sxs-lookup"><span data-stu-id="9e311-104">Import and connect to the MSCommerce module.</span></span>  <span data-ttu-id="9e311-105">Saat diminta untuk masuk, Anda akan perlu menggunakan kredensial peran admin global atau penagihan.</span><span class="sxs-lookup"><span data-stu-id="9e311-105">When prompted to log in, you will need to use Global or Billing Admin role credentials.</span></span>  

<span data-ttu-id="9e311-106">Jika Anda tidak memiliki TLS 1,2, Anda mungkin menerima galat berikut saat mencoba untuk mendapatkan atau memperbarui kebijakan:</span><span class="sxs-lookup"><span data-stu-id="9e311-106">If you don't have TLS 1.2, you may receive the following error when attempting to get or update the policy:</span></span>

<span data-ttu-id="9e311-107">*ErrorMessage-sambungan utama ditutup: galat tak terduga terjadi pada kirim*.</span><span class="sxs-lookup"><span data-stu-id="9e311-107">*ErrorMessage -The underlying connection was closed: An unexpected error occurred on a send*.</span></span>



