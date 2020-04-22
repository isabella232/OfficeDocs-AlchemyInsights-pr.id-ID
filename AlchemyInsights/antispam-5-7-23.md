---
title: AntiSpam-5.7.23
ms.author: pebaum
author: pebaum
manager: mnirkhe
ms.audience: Admin
ms.topic: article
ROBOTS: NOINDEX, NOFOLLOW
localization_priority: Normal
ms.collection: Adm_O365
ms.custom:
- "3156"
- "9001196"
ms.openlocfilehash: 307b738c40c620d057e68eff7d218c8c9b5eb665
ms.sourcegitcommit: 55eff703a17e500681d8fa6a87eb067019ade3cc
ms.translationtype: MT
ms.contentlocale: id-ID
ms.lasthandoff: 04/22/2020
ms.locfileid: "43676500"
---
# <a name="fix-email-delivery-issues-for-error-code-5723"></a><span data-ttu-id="233b4-102">Memperbaiki masalah pengiriman email untuk kode galat 5.7.23</span><span class="sxs-lookup"><span data-stu-id="233b4-102">Fix email delivery issues for error code 5.7.23</span></span>

<span data-ttu-id="233b4-103">Verifikasikan data DNS SPF untuk domain Anda di pemeriksa data SPF atau DNS yang tersedia untuk umum di web.</span><span class="sxs-lookup"><span data-stu-id="233b4-103">Verify the SPF DNS record for your domain at a publicly available SPF or DNS record checker on the web.</span></span>

<span data-ttu-id="233b4-104">Verifikasi bahwa pesan keluar tidak diidentifikasi sebagai spam oleh Microsoft dan diarahkan melalui [Pool pengiriman berisiko tinggi](https://docs.microsoft.com/office365/SecurityCompliance/high-risk-delivery-pool-for-outbound-messages).</span><span class="sxs-lookup"><span data-stu-id="233b4-104">Verify that the outbound message wasn't identified as spam by Microsoft and routed through the [High Risk Delivery Pool](https://docs.microsoft.com/office365/SecurityCompliance/high-risk-delivery-pool-for-outbound-messages).</span></span> <span data-ttu-id="233b4-105">Pesan di Pool pengiriman berisiko tinggi tidak akan lulus pemeriksaan SPF, sehingga tidak akan diterima oleh organisasi email tujuan.</span><span class="sxs-lookup"><span data-stu-id="233b4-105">Messages in the High Risk Delivery Pool won't pass SPF checks, and therefore won't be accepted by the destination email organization.</span></span>

<span data-ttu-id="233b4-106">Jika masalah masih terjadi, Anda mungkin perlu menghubungi admin host surat yang sedang Anda coba untuk mengirim email.</span><span class="sxs-lookup"><span data-stu-id="233b4-106">If the problem persists, you may need to contact the admin of the mail host to which you are attempting to send email.</span></span> <span data-ttu-id="233b4-107">Catat kesalahan eksternal terperinci yang tersedia dalam pesan pentalan.</span><span class="sxs-lookup"><span data-stu-id="233b4-107">Make note of the detailed external error available in the bounce message.</span></span> <span data-ttu-id="233b4-108">Dukungan Microsoft mungkin tidak dapat membantu lebih lanjut.</span><span class="sxs-lookup"><span data-stu-id="233b4-108">Microsoft support may not be able to assist further.</span></span>
