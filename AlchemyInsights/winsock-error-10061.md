---
title: kesalahan Winsock 1554 10061
ms.author: chrisda
author: chrisda
manager: dansimp
ms.date: 04/21/2020
ms.audience: ITPro
ms.topic: article
ms.service: o365-administration
ROBOTS: NOINDEX, NOFOLLOW
localization_priority: Normal
ms.custom:
- "1554"
- "9000079"
ms.assetid: caecfa19-86c9-4aa4-9c83-b8a974ce60b9
ms.openlocfilehash: 4f8007bd8ccb4666260c75fdca15dd0b14eb4e96
ms.sourcegitcommit: c6692ce0fa1358ec3529e59ca0ecdfdea4cdc759
ms.translationtype: MT
ms.contentlocale: id-ID
ms.lasthandoff: 09/14/2020
ms.locfileid: "47698865"
---
# <a name="winsock-error-10061"></a><span data-ttu-id="dd9cd-102">Kesalahan Winsock 10061</span><span class="sxs-lookup"><span data-stu-id="dd9cd-102">Winsock error 10061</span></span>

<span data-ttu-id="dd9cd-103">Kode kesalahan ini berarti Microsoft tidak dapat membuat soket TCP (koneksi) dengan host target.</span><span class="sxs-lookup"><span data-stu-id="dd9cd-103">This error code means that Microsoft couldn't establish a TCP socket (connection) with the target host.</span></span> <span data-ttu-id="dd9cd-104">Kemungkinan penyebab kesalahan ini adalah masalah dengan konfigurasi firewall Anda.</span><span class="sxs-lookup"><span data-stu-id="dd9cd-104">The most likely cause of this error is a problem with your firewall configuration.</span></span> <span data-ttu-id="dd9cd-105">Untuk memperbaiki masalah tersebut, periksa pengaturan ini:</span><span class="sxs-lookup"><span data-stu-id="dd9cd-105">To fix the problem, check these settings:</span></span>

- <span data-ttu-id="dd9cd-106">Memverifikasi Konfigurasi firewall Anda dengan informasi dalam [URL dan rentang alamat IP Microsoft 365](https://docs.microsoft.com/office365/enterprise/urls-and-ip-address-ranges)</span><span class="sxs-lookup"><span data-stu-id="dd9cd-106">Verify your firewall configuration with the information in [Microsoft 365 URLs and IP address ranges](https://docs.microsoft.com/office365/enterprise/urls-and-ip-address-ranges)</span></span>

- <span data-ttu-id="dd9cd-107">Jika kesalahan tersebut khusus untuk Exchange Online Protection (EOP), Anda seharusnya telah diberitahu sebelumnya untuk mengubah [Alamat IP proteksi Exchange Online](https://docs.microsoft.com/office365/SecurityCompliance/eop/exchange-online-protection-ip-addresses).</span><span class="sxs-lookup"><span data-stu-id="dd9cd-107">If the error is specific to Exchange Online Protection (EOP), you should have been previously notified to a change to the [Exchange Online Protection IP addresses](https://docs.microsoft.com/office365/SecurityCompliance/eop/exchange-online-protection-ip-addresses).</span></span>

- <span data-ttu-id="dd9cd-108">Verifikasi bahwa penyedia layanan internet (ISP) Anda tidak memblokir Port.</span><span class="sxs-lookup"><span data-stu-id="dd9cd-108">Verify that your Internet Service Provider (ISP) isn't blocking the port.</span></span>

- <span data-ttu-id="dd9cd-109">Verifikasi pengaturan server Smart host dan target di konektor Anda.</span><span class="sxs-lookup"><span data-stu-id="dd9cd-109">Verify the smart host and target server settings in your connectors.</span></span>

<span data-ttu-id="dd9cd-110">Perhatikan bahwa Microsoft 365 tidak memblokir koneksi *masuk* dengan cara ini.</span><span class="sxs-lookup"><span data-stu-id="dd9cd-110">Note that Microsoft 365 doesn't block *incoming* connections in this manner.</span></span>
