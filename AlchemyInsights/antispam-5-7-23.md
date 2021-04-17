---
title: Antispam - 5.7.23
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
- "3156"
- "9001196"
ms.openlocfilehash: e494e8017f24d65a94d1a7490be4d67c46a2120b
ms.sourcegitcommit: 8bc60ec34bc1e40685e3976576e04a2623f63a7c
ms.translationtype: MT
ms.contentlocale: id-ID
ms.lasthandoff: 04/15/2021
ms.locfileid: "51821414"
---
# <a name="fix-email-delivery-issues-for-error-code-5723"></a><span data-ttu-id="6c7b9-102">Memperbaiki masalah pengiriman email untuk kode kesalahan 5.7.23</span><span class="sxs-lookup"><span data-stu-id="6c7b9-102">Fix email delivery issues for error code 5.7.23</span></span>

<span data-ttu-id="6c7b9-103">Memverifikasi catatan DNS SPF untuk domain Anda di pemeriksa catatan DNS atau SPF yang tersedia untuk publik di web.</span><span class="sxs-lookup"><span data-stu-id="6c7b9-103">Verify the SPF DNS record for your domain at a publicly available SPF or DNS record checker on the web.</span></span>

<span data-ttu-id="6c7b9-104">Verifikasi bahwa pesan keluar tidak diidentifikasi sebagai spam oleh Microsoft dan dirutekan melalui [Kolam Pengiriman Risiko Tinggi.](https://docs.microsoft.com/microsoft-365/security/office-365-security/high-risk-delivery-pool-for-outbound-messages)</span><span class="sxs-lookup"><span data-stu-id="6c7b9-104">Verify that the outbound message wasn't identified as spam by Microsoft and routed through the [High Risk Delivery Pool](https://docs.microsoft.com/microsoft-365/security/office-365-security/high-risk-delivery-pool-for-outbound-messages).</span></span> <span data-ttu-id="6c7b9-105">Pesan dalam Kolam Pengiriman Risiko Tinggi tidak akan lolos pemeriksaan SPF, dan oleh karena itu tidak akan diterima oleh organisasi email tujuan.</span><span class="sxs-lookup"><span data-stu-id="6c7b9-105">Messages in the High Risk Delivery Pool won't pass SPF checks, and therefore won't be accepted by the destination email organization.</span></span>

<span data-ttu-id="6c7b9-106">Jika masalah tetap ada, Anda mungkin perlu menghubungi admin host email tempat Anda mencoba mengirim email.</span><span class="sxs-lookup"><span data-stu-id="6c7b9-106">If the problem persists, you may need to contact the admin of the mail host to which you are attempting to send email.</span></span> <span data-ttu-id="6c7b9-107">Catat kesalahan eksternal mendetail yang tersedia dalam pesan terpental.</span><span class="sxs-lookup"><span data-stu-id="6c7b9-107">Make note of the detailed external error available in the bounce message.</span></span> <span data-ttu-id="6c7b9-108">Dukungan Microsoft mungkin tidak dapat membantu lebih lanjut.</span><span class="sxs-lookup"><span data-stu-id="6c7b9-108">Microsoft support may not be able to assist further.</span></span>
