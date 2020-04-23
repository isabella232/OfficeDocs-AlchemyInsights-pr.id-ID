---
title: 1554 Winsock galat 10061
ms.author: chrisda
author: chrisda
manager: dansimp
ms.date: 04/21/2020
ms.audience: ITPro
ms.topic: article
ROBOTS: NOINDEX, NOFOLLOW
localization_priority: Normal
ms.custom:
- "1554"
- "9000079"
ms.assetid: caecfa19-86c9-4aa4-9c83-b8a974ce60b9
ms.openlocfilehash: e8f62d97efc937518ef766b45e1747e83b7f99c3
ms.sourcegitcommit: 631cbb5f03e5371f0995e976536d24e9d13746c3
ms.translationtype: MT
ms.contentlocale: id-ID
ms.lasthandoff: 04/22/2020
ms.locfileid: "43766172"
---
# <a name="winsock-error-10061"></a><span data-ttu-id="2abf7-102">Winsock galat 10061</span><span class="sxs-lookup"><span data-stu-id="2abf7-102">Winsock error 10061</span></span>

<span data-ttu-id="2abf7-103">Kode galat ini berarti bahwa Microsoft tidak dapat membuat soket TCP (sambungan) dengan target host.</span><span class="sxs-lookup"><span data-stu-id="2abf7-103">This error code means that Microsoft couldn't establish a TCP socket (connection) with the target host.</span></span> <span data-ttu-id="2abf7-104">Kemungkinan penyebab kesalahan ini adalah masalah dengan konfigurasi firewall Anda.</span><span class="sxs-lookup"><span data-stu-id="2abf7-104">The most likely cause of this error is a problem with your firewall configuration.</span></span> <span data-ttu-id="2abf7-105">Untuk memperbaiki masalah, periksa pengaturan ini:</span><span class="sxs-lookup"><span data-stu-id="2abf7-105">To fix the problem, check these settings:</span></span>

- <span data-ttu-id="2abf7-106">Verifikasi Konfigurasi firewall Anda dengan informasi di [Microsoft 365 URL dan kisaran alamat IP](https://docs.microsoft.com/office365/enterprise/urls-and-ip-address-ranges)</span><span class="sxs-lookup"><span data-stu-id="2abf7-106">Verify your firewall configuration with the information in [Microsoft 365 URLs and IP address ranges](https://docs.microsoft.com/office365/enterprise/urls-and-ip-address-ranges)</span></span>

- <span data-ttu-id="2abf7-107">Jika galat khusus untuk Exchange Online Protection (EOP), Anda harus telah diberitahu sebelumnya untuk mengubah [Alamat IP perlindungan Exchange Online](https://docs.microsoft.com/office365/SecurityCompliance/eop/exchange-online-protection-ip-addresses).</span><span class="sxs-lookup"><span data-stu-id="2abf7-107">If the error is specific to Exchange Online Protection (EOP), you should have been previously notified to a change to the [Exchange Online Protection IP addresses](https://docs.microsoft.com/office365/SecurityCompliance/eop/exchange-online-protection-ip-addresses).</span></span>

- <span data-ttu-id="2abf7-108">Verifikasi bahwa Internet Service Provider (ISP) tidak memblokir Port.</span><span class="sxs-lookup"><span data-stu-id="2abf7-108">Verify that your Internet Service Provider (ISP) isn't blocking the port.</span></span>

- <span data-ttu-id="2abf7-109">Verifikasi host cerdas dan pengaturan server target di konektor Anda.</span><span class="sxs-lookup"><span data-stu-id="2abf7-109">Verify the smart host and target server settings in your connectors.</span></span>

<span data-ttu-id="2abf7-110">Perhatikan bahwa Microsoft 365 tidak memblokir koneksi *masuk* dengan cara ini.</span><span class="sxs-lookup"><span data-stu-id="2abf7-110">Note that Microsoft 365 doesn't block *incoming* connections in this manner.</span></span>
