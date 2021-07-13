---
title: Relay pool keluar
ms.author: pebaum
author: pebaum
manager: scotv
ms.date: 07/08/2021
ms.audience: Admin
ms.topic: article
ms.service: o365-administration
ROBOTS: NOINDEX, NOFOLLOW
localization_priority: Normal
ms.collection: Adm_O365
ms.custom:
- "3000003"
- "12315"
ms.openlocfilehash: b723566a29e0be581b7fdc30332166d5cddbd38f
ms.sourcegitcommit: 270a1ca9c35b50b8be6b06f432c9c90e4090fb57
ms.translationtype: MT
ms.contentlocale: id-ID
ms.lasthandoff: 07/08/2021
ms.locfileid: "53381717"
---
# <a name="outbound-relay-pool"></a><span data-ttu-id="c132d-102">Relay pool keluar</span><span class="sxs-lookup"><span data-stu-id="c132d-102">Outbound relay pool</span></span>

<span data-ttu-id="c132d-103">Microsoft membuat beberapa perubahan pada konfigurasi untuk melakukan relai atau meneruskan email melalui Microsoft 365.</span><span class="sxs-lookup"><span data-stu-id="c132d-103">Microsoft is making some changes to the configuration for relaying or forwarding email through Microsoft 365.</span></span> <span data-ttu-id="c132d-104">Pesan dalam skenario tertentu diteruskan atau diteruskan melalui Microsoft 365 menggunakan kelompok relay khusus.</span><span class="sxs-lookup"><span data-stu-id="c132d-104">Messages in certain scenarios are forwarded or relayed through Microsoft 365 using a special relay pool.</span></span> <span data-ttu-id="c132d-105">Pesan yang dikirim dengan menggunakan relay pool mungkin berakhir di folder email sampah penerima.</span><span class="sxs-lookup"><span data-stu-id="c132d-105">Messages sent by using the relay pool could end up in recipient's junk mail folder.</span></span> <span data-ttu-id="c132d-106">Untuk informasi selengkapnya, lihat [Kolam renang pengiriman keluar](/microsoft-365/security/office-365-security/high-risk-delivery-pool-for-outbound-messages#relay-pool)</span><span class="sxs-lookup"><span data-stu-id="c132d-106">For more information, see [Outbound delivery pools](/microsoft-365/security/office-365-security/high-risk-delivery-pool-for-outbound-messages#relay-pool)</span></span>

<span data-ttu-id="c132d-107">Untuk menghindari skenario menggunakan relay pool, pastikan bahwa pesan yang diteruskan/diteruskan memenuhi salah satu kriteria berikut ini:</span><span class="sxs-lookup"><span data-stu-id="c132d-107">To avoid a scenario using the relay pool, make sure that forwarded/relayed messages meet one of the following criteria:</span></span>

- <span data-ttu-id="c132d-108">Pengirim keluar adalah domain yang diterima dari penyewa.</span><span class="sxs-lookup"><span data-stu-id="c132d-108">The outbound sender is an accepted domain of the tenant.</span></span>
- <span data-ttu-id="c132d-109">Sender Policy Framework (SPF) passes when the message comes to Microsoft 365.</span><span class="sxs-lookup"><span data-stu-id="c132d-109">Sender Policy Framework (SPF) passes when the message comes to Microsoft 365.</span></span>
- <span data-ttu-id="c132d-110">DomainKeys Identified Mail (DKIM) di domain pengirim P2 akan masuk ketika pesan masuk ke Microsoft 365.</span><span class="sxs-lookup"><span data-stu-id="c132d-110">DomainKeys Identified Mail (DKIM) on the P2 sender domain passes when the message comes to Microsoft 365.</span></span>
 
<span data-ttu-id="c132d-111">Pesan yang memenuhi kriteria di atas tidak diteruskan melalui relay pool.</span><span class="sxs-lookup"><span data-stu-id="c132d-111">Messages that meet the above criteria are not relayed through the relay pool.</span></span>

<span data-ttu-id="c132d-112">Jika catatan MX untuk domain Anda di arahkan ke server pihak ketiga atau lokal, gunakan pemfilteran yang disempurnakan untuk memastikan validasi SPF sudah benar untuk email masuk dan untuk menghindari mengirim email melalui relay pool.</span><span class="sxs-lookup"><span data-stu-id="c132d-112">If the MX record for your domain is pointed to a third-party or on-premises server, use enhanced filtering to make sure the SPF validation is correct for inbound email and to avoid sending email through the relay pool.</span></span>

<span data-ttu-id="c132d-113">**Bagaimana kami dapat mengetahui apakah kami terkena dampak dari relay pool?**</span><span class="sxs-lookup"><span data-stu-id="c132d-113">**How can we tell if we're impacted by the relay pool?**</span></span>

<span data-ttu-id="c132d-114">Jika email yang Anda teruskan atau relai menggunakan salah satu kriteria di atas, pesan tidak akan diteruskan melalui relay pool.</span><span class="sxs-lookup"><span data-stu-id="c132d-114">If your forwarded or relayed emails use one of the above criteria, messages won't be relayed through the relay pool.</span></span> <span data-ttu-id="c132d-115">Namun, jika pesan dikirim melalui relay pool, IP server keluar ada dalam rentang 40.95.0.0/16 dan nama server keluar **menyertakan rly** dalam nama.</span><span class="sxs-lookup"><span data-stu-id="c132d-115">However, if a message is sent through a relay pool, the outbound server IP is in the 40.95.0.0/16 range and the outbound server name includes **rly** in the name.</span></span>

