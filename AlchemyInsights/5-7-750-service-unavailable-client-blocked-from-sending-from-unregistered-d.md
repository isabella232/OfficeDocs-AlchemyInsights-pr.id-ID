---
title: 1048 Layanan 5.7.750 tidak tersedia. Klien diblokir dari pengiriman dari domain yang tidak terdaftar
ms.author: chrisda
author: chrisda
manager: dansimp
ms.date: 04/21/2020
ms.audience: ITPro
ms.topic: article
ms.service: o365-administration
ROBOTS: NOINDEX, NOFOLLOW
localization_priority: Normal
ms.assetid: 8cf6d70b-9a78-4f04-ac59-7ffcf44ffd22
ms.custom:
- "1048"
- "3100026"
ms.openlocfilehash: 731aa2e155ba3fdaaca7fed9dd51b3e4a3f20f29
ms.sourcegitcommit: c6692ce0fa1358ec3529e59ca0ecdfdea4cdc759
ms.translationtype: MT
ms.contentlocale: id-ID
ms.lasthandoff: 09/14/2020
ms.locfileid: "47664245"
---
# <a name="57750-client-blocked-from-sending-from-unregistered-domain"></a><span data-ttu-id="6b3b5-103">klien 5.7.750 diblokir dari pengiriman dari domain tidak terdaftar</span><span class="sxs-lookup"><span data-stu-id="6b3b5-103">5.7.750 Client blocked from sending from unregistered domain</span></span>

<span data-ttu-id="6b3b5-104">Kesalahan terjadi ketika volume besar pesan dikirim dari domain yang tidak ditetapkan dalam penyewa Anda (ditambahkan sebagai domain diterima dan divalidasi).</span><span class="sxs-lookup"><span data-stu-id="6b3b5-104">The error occurs when a large volume of messages are sent from domains that aren't provisioned in your tenant (added as accepted domains and validated).</span></span>

<span data-ttu-id="6b3b5-105">Untuk menghindari kesalahan ini, Anda bisa menggunakan konektor aliran email berbasis sertifikat di mana domain sertifikat tersebut adalah domain yang tersedia, atau Anda bisa menyediakan semua domain pengirim.</span><span class="sxs-lookup"><span data-stu-id="6b3b5-105">To avoid this error, you can use a certificate-based mail flow connector where the certificate's domain is a provisioned domain, or you can provision all sending domains.</span></span>
