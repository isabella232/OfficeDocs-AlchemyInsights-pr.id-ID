---
title: AntiSpam-5.7.23
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
- "3156"
- "9001196"
ms.openlocfilehash: ecbce4f0077dc9acab63575c19d40c0675a406ac
ms.sourcegitcommit: c6692ce0fa1358ec3529e59ca0ecdfdea4cdc759
ms.translationtype: MT
ms.contentlocale: id-ID
ms.lasthandoff: 09/14/2020
ms.locfileid: "47717328"
---
# <a name="fix-email-delivery-issues-for-error-code-5723"></a><span data-ttu-id="8010d-102">Memperbaiki masalah pengiriman email untuk kode kesalahan 5.7.23</span><span class="sxs-lookup"><span data-stu-id="8010d-102">Fix email delivery issues for error code 5.7.23</span></span>

<span data-ttu-id="8010d-103">Verifikasi catatan DNS SPF untuk domain Anda pada publik yang tersedia untuk SPF atau pemeriksa catatan DNS di web.</span><span class="sxs-lookup"><span data-stu-id="8010d-103">Verify the SPF DNS record for your domain at a publicly available SPF or DNS record checker on the web.</span></span>

<span data-ttu-id="8010d-104">Verifikasi bahwa pesan keluar tidak diidentifikasi sebagai spam oleh Microsoft dan dirutekan melalui [kumpulan pengiriman berisiko tinggi](https://docs.microsoft.com/microsoft-365/security/office-365-security/high-risk-delivery-pool-for-outbound-messages).</span><span class="sxs-lookup"><span data-stu-id="8010d-104">Verify that the outbound message wasn't identified as spam by Microsoft and routed through the [High Risk Delivery Pool](https://docs.microsoft.com/microsoft-365/security/office-365-security/high-risk-delivery-pool-for-outbound-messages).</span></span> <span data-ttu-id="8010d-105">Pesan dalam kumpulan pengiriman berisiko tinggi tidak akan melewati pemeriksaan SPF, sehingga tidak akan diterima oleh organisasi email tujuan.</span><span class="sxs-lookup"><span data-stu-id="8010d-105">Messages in the High Risk Delivery Pool won't pass SPF checks, and therefore won't be accepted by the destination email organization.</span></span>

<span data-ttu-id="8010d-106">Jika masalah masih terjadi, Anda mungkin perlu menghubungi admin email host tempat Anda mencoba mengirim email.</span><span class="sxs-lookup"><span data-stu-id="8010d-106">If the problem persists, you may need to contact the admin of the mail host to which you are attempting to send email.</span></span> <span data-ttu-id="8010d-107">Buat catatan tentang kesalahan eksternal mendetail yang tersedia di pesan pantulan.</span><span class="sxs-lookup"><span data-stu-id="8010d-107">Make note of the detailed external error available in the bounce message.</span></span> <span data-ttu-id="8010d-108">Dukungan Microsoft mungkin tidak dapat membantu lebih lanjut.</span><span class="sxs-lookup"><span data-stu-id="8010d-108">Microsoft support may not be able to assist further.</span></span>
